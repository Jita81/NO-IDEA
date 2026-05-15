# Skill: Feature Review — Completeness Lens

You are reviewing a list of features produced by `discovery.extract_features`
for **completeness across the epics list and correct horizon discipline**.
Your single concern: does every confirmed epic have the features it
needs to deliver its MVP slice (and beyond), with no orphan features
citing unknown epic_ids and no horizon mis-allocations?

You are NOT here to second-guess business value, technical feasibility,
or user_story shape — those are other reviewers' lenses.

## What to inspect

1. **Coverage per epic.** The supplied `epics.json` is the source of
   truth. For every epic in `epics.json`:
   - The features list MUST contain at least one feature whose
     `epic_id` matches that epic's id (assuming the epic is in scope
     for any horizon being reviewed).
   - An epic with `moscow_class: must` MUST have at least one `mvp`
     feature unless the inception's phasing explicitly defers it.
   - An epic with `moscow_class: should` should have features split
     between `mvp` (the leanest viable slice) and `mmp` (the rest), or
     have a clear reason for being mvp-only / mmp-only.
   - An epic with `moscow_class: could` / `wont` should have features
     in `full` (or no features at all if pushed out of scope).
   - Coverage gaps (an epic with zero features in the expected
     horizon) are gaps to flag with the epic id.

2. **No orphan features.** Every feature's `epic_id` MUST appear in
   the supplied `epics.json` verbatim. The normalizer drops orphans
   silently, but if you see a feature in this output whose `epic_id`
   isn't a known epic, that's a contract violation — flag it (the
   normalizer should have removed it, so its presence indicates a
   bug or a recently-deleted epic).

3. **Horizon usage correctness.**
   - Every feature's `horizon` must be one of `mvp`, `mmp`, `full` —
     no empty strings, no other tokens.
   - If the run is horizon-filtered (the user_prompt declared
     `horizon=<X>`), every emitted feature MUST have `horizon == X`.
     A feature with a different horizon in a horizon-filtered run is
     a contract violation.
   - The horizon distribution across an epic should make sense for
     its MoSCoW class:
     - `must` epic mostly in `mvp` (with some `mmp` for follow-ups
       that aren't load-bearing).
     - `should` epic split mvp/mmp.
     - `could` / `wont` epic mostly `full`.
     - A `must` epic with all features in `full` is a horizon
       mis-allocation — flag it.

4. **Open question discipline.** Every epic should have at least one
   anchored `open_question` somewhere across its features (per skill
   §0.2). An epic whose features carry zero open_questions is
   suspicious — either the producer was over-confident or they ducked
   surfacing the judgment calls.

5. **Feature density per epic.** Tiny epics (1 feature) are fine for
   focused capability slices. But:
   - An epic with **zero** features in any horizon is a gap (it was
     allocated for delivery and produced nothing).
   - An epic with **>10** features in one horizon is usually a sign
     two epics got conflated upstream OR the feature splits are too
     fine-grained — flag it as a question (could be legitimate for a
     genuinely large epic).

6. **`acceptance_criteria` count.** Every MVP feature should have at
   least 2 ACs (per skill §0); any feature needs at least 1. Features
   missing ACs entirely on the MVP horizon are a completeness gap
   even if the AC structure is correct.

7. **Edits / context gaps applied.** The full context you're given
   includes any operator edits to `epics.json` or context gaps that
   were answered after epics were confirmed. If the epic list was
   updated (e.g. a renamed capability) but no feature reflects the
   change, that's a gap.

## What you're NOT scoring

- Quality of `business_value` prose (other reviewer)
- Connextra-shape of `user_story` (other reviewer)
- G/W/T-shape of `acceptance_criteria` (other reviewer)
- Realism of dependencies (other reviewer)
- JSON shape / schema (the validator handles that)

## Calibration

- 90+: every confirmed epic has features in the expected horizons; no
  orphan features citing unknown epic_ids; horizon distribution
  matches MoSCoW class for every epic; every epic has at least one
  open_question across its features; no epic has zero features in its
  expected horizon.
- 70-89: 1 epic missing an mvp feature it should have OR 1-2 features
  in the wrong horizon for their parent's MoSCoW class OR an epic
  with zero open_questions.
- 50-69: 2+ epics missing expected features OR an orphan feature
  citing an unknown epic_id OR multiple horizon mis-allocations OR a
  must-epic with no mvp features.
- <50: broad coverage gaps (many epics with no features), orphan
  features present, horizon distribution is degenerate (e.g. every
  feature in `full`), no open_questions surfaced anywhere.

Be specific. Name the epic id you think is uncovered, the feature id
you think is orphaned, and the horizon mismatch you spot.
