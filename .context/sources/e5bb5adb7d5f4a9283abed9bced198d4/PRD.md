# Product Requirements Document
## Referral Networking Platform for UK Early-Stage Founders

**Version:** 1.1  
**Date:** 2026-05-15  
**Status:** Draft  
**Scope:** MVP through MMP  
**Source files:** 01-concept-definition, 02-competitor-landscape, 03-market-analysis, 04-pricing-benchmarks, 05-mvp-scope, 06-intake-questionnaire, 07-operator-matching-playbook, 08-mmp-scope

---

## Table of Contents

1. [Product Vision](#1-product-vision)
2. [Market Context](#2-market-context)
3. [Target Users](#3-target-users)
4. [Core Mechanics](#4-core-mechanics)
5. [MVP — Minimum Viable Product](#5-mvp--minimum-viable-product)
6. [MMP — Minimum Marketable Product](#6-mmp--minimum-marketable-product)
7. [The Living Profile](#7-the-living-profile)
8. [Intake Questionnaire](#8-intake-questionnaire)
9. [Matching Engine](#9-matching-engine)
10. [Community Layer](#10-community-layer)
11. [Operator Admin Dashboard](#11-operator-admin-dashboard)
12. [Subscription Model](#12-subscription-model)
13. [Tech Stack](#13-tech-stack)
14. [UI/UX Requirements](#14-uiux-requirements)
15. [Success Criteria](#15-success-criteria)
16. [Out of Scope](#16-out-of-scope)
17. [Open Questions](#17-open-questions)

---

## 1. Product Vision

### The Problem

Most early-stage UK founders are networking with people who can't buy from them — peers at similar stages with no budget and no relevant customer base. Traditional referral networking (BNI and equivalents) is expensive, attendance-heavy, and built for established trades rather than modern digital businesses. Affiliate and referral partnership tools exist, but they assume you already have partners — they don't help you find the right ones.

The result: founders spend significant time and money on networking that doesn't generate revenue.

### The Solution

A UK-focused platform that matches early-stage founders with complementary businesses — not competitors, not random connections — and provides the education and infrastructure to turn those connections into active referral partnerships.

The three-layer model:

1. **Matching layer** — Intelligent intake identifies complementary business pairs based on shared customer profiles, not just sector or geography. The platform surfaces the match and explains specifically why it's commercially valuable.
2. **Community layer** — Structured spaces, peer conversations, and events that make the platform sticky between matches. Members stay for the community and the ongoing relationship, not just the first introduction.
3. **Referral education layer** — The platform teaches members how referral partnerships work: how to structure an arrangement, what to offer a partner, how to make a referral feel natural rather than forced.

### What It Is Not

- A payment processor or affiliate tracking platform — commercial relationships are managed directly between businesses
- A replacement for face-to-face networking
- A direct sales tool or marketplace
- A platform for founders to sell to each other

### Core Value Proposition

> "You're great at what you do. Getting your first customers shouldn't require you to become a salesperson. We match you with businesses that are a genuine fit — so working together feels natural, not forced — and we teach you how the whole thing works."

**The concept in one line:** It's online dating for businesses. You answer a few questions. We find you a match. You decide if you like them.

**The outcome we're solving for:** A new founder's first five customers, within their first 30 days on the platform. Not "better networking" — customers. Real people who engage with the service, pay for it or take the free offer, and leave a testimonial that makes the next referral easier.

**Why this matters:** Most early-stage founders are good at their skill and stuck on everything else. Selling feels awkward. Marketing is confusing. Networking events produce business cards and no customers. This platform removes that pressure by giving founders a warm introduction channel that works — the right businesses, matched for a specific reason, with a clear way to work together.

**Copy authority:** All user-facing copy is governed by `docs/COPY.md`. Read it before writing any landing page, email, intake copy, or UI text.

### Positioning

- **Against generic founder communities:** Commercial focus, intelligent matching, not just peer support
- **Against referral tracking tools:** Helps you find partners first; the platform does not track outcomes (intentionally — commercial arrangements are between members)
- **Against Partners.ai:** Community layer, living profile, referral education, UK-focused, founder and SME audience
- **Tone principle:** The platform positions itself on what it does well — not by comparing against or criticising others. All marketing and product copy speaks positively about the platform's own value.

---

## 2. Market Context

### Market Size

The Global Startup Founders Community Networking Tool Market is valued at USD $1.64 billion (2025), forecast to reach USD $3.36 billion by 2032 at a 16.4% CAGR. UK-specific market size is not published but is a significant subset of the European share.

### UK Demand Signals

- There are approximately 5.5 million small businesses in the UK. Even a narrow slice — businesses actively seeking growth partnerships — represents a large addressable audience.
- 60%+ of solo founders report being overwhelmed managing every aspect of their business alone (Simply Business 2025 Solopreneur Report)
- 75% of VC-funded founders come from advantaged backgrounds; 43% of seed funding goes to teams with elite university connections — creating demand for alternative routes to growth
- Strategic partnerships are increasingly cited as a primary growth lever for SMEs as traditional acquisition channels (paid advertising, cold outreach) become more expensive and less effective
- AI-powered matching and remote-first networking are driving product differentiation in the space

### Competitive Landscape

No single competitor combines intelligent complementary-business matching + referral education + community retention in one product aimed at UK founders and SME owners.

| Dimension | Generic founder community | Partners.ai | PartnerBridge | This platform |
|---|---|---|---|---|
| Matching intelligence | None | Yes (local SMB, US) | Yes (SaaS/tech only) | Yes (complementary business, all sectors, UK) |
| Referral/partnership education | None | None | None | Core feature |
| Deal-structuring guidance | None | None | None | Core feature |
| Community layer | Online forum | None | None | Online + scheduled calls |
| Target user | Any founder | Local service business (US) | SaaS/tech companies | UK founders and SME owners |
| UK focus | Varies | No | Partial | Yes |
| Price (annual) | Free–£360 | Unknown | Unknown | £399–£599 |
| Time commitment | Low | Low | Low | Medium (scheduled touchpoints) |

**Closest competitor to monitor:** Partners.ai. If they add a community layer and UK localisation, they close most of the gap. Timeline unknown.

**Other UK competitors identified:**
- **PartnerBridge** — UK partnership platform exclusively for SaaS/tech companies; focused on software integrations and co-selling. Not a competitor for our audience but worth monitoring for feature direction.
- **Business-Matching.co.uk** — A UK introduction service operating as a manual broker model. Small scale, relationship-based, limited reach. Not tech-enabled.
- **Alignable** (US) — General business referral network. Not available in the UK in any meaningful way.

### Key Risks

1. **Community cold start** — matching quality depends on member volume; small early membership = fewer good matches = lower retention. Mitigation: manual matching at MVP ensures quality over quantity.
2. **Affiliate literacy gap** — many founders don't understand affiliate models. This is an opportunity (education = moat) and an acquisition friction point.
3. **"Cut out the platform" risk** — once two businesses connect, ongoing platform value must come from new introductions, community, and living profile improvements.
4. **Partners.ai expansion** — the closest conceptual competitor moving into UK/community territory.

---

## 3. Target Users

### Primary: UK Founder or SME Owner (Member)

The platform serves UK founder-led businesses across a broader stage range than a single ICP. What unites all primary members is not their revenue stage but their situation: they have a defined customer type, they are actively trying to grow, and they lack a systematic way to find and structure commercial partnerships.

**Core filter:** Does this business serve other businesses, or does it serve consumers who share characteristics with the clients of other businesses in the network? If yes, they are a potential member.

#### ICP Segment A — Early-Stage Founders (Cohort 1 Priority)

- **Stage:** Pre-revenue to ~£10k MRR
- **Profile:** Transitioning a skill into a business — freelancer-to-agency, practitioner-to-practice owner
- **Pain:** Networking with peers who can't afford their services; no budget for enterprise partnership tools; limited understanding of referral and promotional models
- **Behaviour:** Already networking (events, communities, LinkedIn) but not converting relationships into revenue
- **Key outcome they need:** First five customers, proof their business works, confidence to keep going
- **Messaging angle:** "Stop networking with people who can't buy from you. We match you with businesses that already serve your kind of client — and show you how to turn that into a partnership that sends you customers."
- **Geography:** UK-first; London and major cities as initial concentration

**User story:** "I run a bookkeeping practice serving small e-commerce businesses. I keep meeting other bookkeepers and coaches at networking events. I need to find web developers, ad agencies, and logistics consultants who serve the same businesses — people I can refer my clients to and who can refer their clients to me."

#### ICP Segment B — Growing SME Owners (Cohort 2+)

- **Stage:** £10k–£100k+ MRR; past the survival phase, focused on sustainable growth
- **Profile:** Established small business with a clear customer base and proven service, but customer acquisition is still the primary constraint; no dedicated sales team
- **Pain:** Traditional marketing channels are expensive and unpredictable; aware that referral and promotional partnerships could work but don't know how to find or structure them systematically
- **Behaviour:** May have informal referral relationships already; has tried paid ads or agencies with mixed results; looking for lower-cost, higher-trust growth channels
- **Key outcome they need:** A repeatable, low-effort referral channel that runs alongside the business; structured partnerships that generate consistent introductions
- **Messaging angle:** "You've proved the business works. Now build the partnerships that send you clients on autopilot — without a sales team."

**User story:** "I run a HR consultancy with 12 clients and a steady income. I get most of my clients through word of mouth but it's unpredictable. I want to work with accountants and solicitors who serve the same growing SMEs I do — so we can refer each other systematically instead of hoping someone mentions my name."

#### ICP Segment C — Specialist Service Providers in B2B Adjacencies

- **Stage:** Any; consumer-facing businesses that also serve or want to serve business clients
- **Profile:** Photographers, event organisers, caterers, printers, signage, personal trainers offering corporate wellness — businesses whose core market is consumer but who have or want a B2B revenue stream
- **Pain:** B2B clients are higher-value and stickier but harder to find through consumer channels
- **Behaviour:** May already do some corporate work but lack a systematic way to find more; typically not attending startup communities
- **Key outcome they need:** A route into business clients through partnerships with businesses that already have those clients
- **Messaging angle:** "Your best clients are businesses — and the fastest way to find more is through the businesses they already trust."
- **Note:** Segment C is a Cohort 2+ priority. Best introduced once Segments A and B have enough density to generate good matches for them. See `research/09-founding-member-profile.md` for cohort sequencing.

### Messaging and copy by segment

All three segments share the same core product experience. Copy and onboarding should acknowledge that members join at different stages. The platform's universal truth — "you should be working with businesses that already serve your kind of client, but there's no good way to find them" — applies to all three. Tone adjusts slightly:

- Segment A: urgency, proof, getting started ("your first five customers")
- Segment B: efficiency, repeatability, leverage ("a referral system that runs itself")
- Segment C: access, credibility, B2B route ("get in front of businesses through the ones they trust")

All copy must follow `docs/COPY.md`. The segment messaging angles above are inputs to copy, not finished copy.

### Secondary: Operator (Platform Administrator)

- **Role:** Reviews intake submissions, tags member profiles, runs match identification, edits and sends match notifications, manages the community, monitors platform health
- **Context:** Solo or small team at MVP/MMP stage; time is the primary constraint
- **Needs:** Efficient workflow to process intakes and matches without unsustainable time investment; clear view of who is unmatched and how long they've been waiting; ability to override algorithm suggestions

---

## 4. Core Mechanics

### The Three Match Types

Not all partnerships work the same way. The platform supports three distinct types of match. All three are valid at intake and matching stages.

**Terminology note:** The platform uses two naming conventions intentionally. Internal documentation (PRD, research files, operator tools, matching engine) uses the technical terms. Member-facing copy (intake form, match notifications, onboarding, marketing) uses the plain-English labels. Never use "affiliate" in member-facing copy without explanation — most members won't know the term.

| Internal term | Member-facing label | Use in |
|---|---|---|
| Referral | Referral partners | All contexts — no change needed |
| Affiliate | Promotional partners | All member-facing copy and UI |
| Mutual benefit | Mutual-benefit partners | All contexts — no change needed |

**1. Referral (member-facing: Referral partners)** — Each business sends the other's clients. A bookkeeper and a web developer. A personal trainer and a nutritionist. Clients of one are natural prospects for the other. Typically involves a referral fee or reciprocal arrangement agreed between the two businesses directly.

**2. Affiliate (member-facing: Promotional partners)** — One business actively promotes the other — on their website, in their emails, at their premises. Less about one-for-one client swapping; more about one business becoming a visible channel for another. Can be mutual or one-directional.

**3. Mutual benefit (member-facing: Mutual-benefit partners)** — Two businesses that solve each other's problems directly, even if their end customers are unrelated. Example: a street food vendor and a warehouse company with a large car park. The warehouse wants to improve staff morale. The vendor needs a regular lunchtime pitch. Neither is referring in the traditional sense — they just both win by working together.

The mutual-benefit type is the most distinctive and often the most surprising to new members. Use concrete examples of all three when explaining the platform — especially the third. It signals that the matching logic goes beyond the obvious.

**Operator note:** At intake, members describe what kind of partnership they're looking for. Match rationale should specify which type(s) apply to each pairing and why.

### The Matching Loop

```
Member signs up
    ↓
Completes intake questionnaire (matching-critical fields)
    ↓
Operator confirms two matching gates are met:
  (1) Free member referral offer — qualifies as free, discrete, describable
  (2) Partner visibility commitment — physical display and/or online affiliate/partner section
    ↓
Member enters match pool (blocked until both gates confirmed)
    ↓
Operator (MVP) / Algorithm (MMP) identifies match candidates
    ↓
Operator reviews, edits rationale, sends match notification
    ↓
Both members accept → private introduction
    ↓
Members manage referral relationship directly
    ↓
Platform prompts living profile update (90 days)
    ↓
New match candidates surface
```

### Membership Requirements

Every member must have two things confirmed before entering the match pool:

**1. A free member referral offer**
A specific, free, deliverable thing that a member offers exclusively to other members and the clients those members refer. It should be their attraction offer — a review, audit, assessment, or diagnosis: the thin slice of their full service that demonstrates value and gets someone in the door. The trade: the member provides the offer free; the recipient provides a testimonial or review. This builds the social proof that makes partners more confident referring the member over time. The offer must be genuinely free (not discounted), discrete and deliverable (not "a chat"), and describable by a non-expert partner in two sentences.

**2. A partner visibility commitment**
Every member must actively make their partners discoverable to their own client base. The mechanism depends on business type:
- **Physical premises:** Member displays business cards, flyers, or similar partner materials somewhere clients will encounter them (reception, waiting area, desk, noticeboard).
- **Online business:** Member creates a partner or affiliate section on their website listing businesses they work with and recommend.
- **Both:** Member maintains both.

This is not optional. A referral network where partners only refer privately when asked generates significantly less volume than one where partners are actively visible to each other's client bases.

### The Living Profile Mechanic

Intake is a starting point, not a one-time event. The platform periodically resurfaces key questions:
- Has revenue or stage changed?
- Has the ICP shifted?
- Are there new types of partners needed?
- Has the free member referral offer changed or improved?

This keeps match quality high over time and gives members a continuous reason to stay engaged.

### Referral Education

The platform teaches members how referral, promotional, and mutual-benefit arrangements work — not as optional background reading, but as contextual guidance embedded throughout the member journey.

**Member referral offer education** covers: why a free offer generates more referrals than a discounted one, how to structure the testimonial exchange, how to make the offer specific enough that a partner can describe it confidently, and how to use testimonials to build a body of social proof that compounds over time.

**Partnership arrangement education** covers: how to structure a commission or flat-fee arrangement, what rates are typical for different business types, how to set up a physical display of partner materials, how to create a basic online partner/affiliate page, and how to frame an introduction naturally rather than as a sales pitch.

**Deal-structuring guidance** covers the four steps members take when a match accepts:
1. **Start the conversation** — how to approach the first exchange so it feels natural, not transactional. Suggested opening lines and framing for the first message.
2. **Agree the arrangement** — what to decide: which match type applies, what each party will do, what the financial arrangement is (if any), and how formally to document it. Template agreement language for common arrangements.
3. **Make your partner visible** — practical steps for physical display (business cards, flyers, noticeboard) and online presence (partner page template, LinkedIn recommendation wording).
4. **Track it yourself** — the platform does not track referral outcomes; commercial arrangements are managed directly between members. Guidance is provided on how members can track introductions and conversions themselves: a simple shared log, a note in their CRM, or a monthly check-in with their partner. The goal is that both parties know whether the arrangement is working — not that the platform knows.

This education is delivered contextually: at intake (why we ask for these things), at match notification (how to approach the first conversation), and through community resources (guides, examples, templates).

---

## 5. MVP — Minimum Viable Product

### Purpose

The MVP is a learning instrument, not a product launch. It answers three questions:
1. Will UK founders join?
2. Will they complete intake?
3. Will they engage with a match?

Nothing in the MVP exists beyond answering these three questions.

### MVP in Plain English

A no-code stack that lets a founder:
1. Land on a sign-up page and hear about the platform
2. Complete an intake questionnaire
3. Receive a manually curated match with a specific explanation of why it's commercially valuable
4. Be introduced to the matched founder
5. Have somewhere to check in and see other members

No dashboard, no algorithm, no directory, no payments.

### MVP User Journey

**Step 1 — Discovery:** Founder hears about the platform (word of mouth, LinkedIn, community referral). Lands on a simple landing page. Single CTA: "Apply for early access."

**Step 2 — Intake:** Founder completes the intake questionnaire (see Section 8). Responses fed into Airtable. This is the single most important piece of the MVP — quality here determines match quality.

**Step 3 — Operator review:** Operator reads the submission in Airtable, tags the profile with sector and ICP categories, and confirms both matching gates before the member enters the match pool: (1) does the free member referral offer qualify? (genuinely free, discrete deliverable, describable by a partner) and (2) has the member committed to a partner visibility mechanism? If either gate fails, operator contacts the member before proceeding. Only once both are confirmed does the operator cross-reference against existing member profiles to identify potential matches.

**Step 4 — Match notification:** Founder receives a personal email: who the match is, why they're complementary (specific, not generic), and a suggested opening. The matched founder receives the same.

**Step 5 — Introduction:** Both founders accept → introduction email with both CC'd. From here, the commercial relationship is entirely between them.

**Step 6 — Community check-in:** Founder has somewhere to land after the match — Slack workspace or Circle free tier. Lightweight, not a full community product.

### MVP Feature Set

**In scope:**

| Feature | Implementation |
|---|---|
| Landing page (concept + CTA) | Framer or Carrd |
| Intake questionnaire | Typeform or Tally |
| Member database | Airtable |
| Manual match curation | Airtable + operator judgment |
| Match notification (email) | Gmail / Loops |
| Email introduction between matches | Gmail |
| Lightweight community space | Slack (free) or Circle (free tier) |

**Explicitly deferred:**

| Feature | Reason |
|---|---|
| Member-facing dashboard | Not needed to test core loop |
| Member directory | Undermines curated matching as the value |
| Automated/algorithmic matching | Manual matching is the point at this stage |
| Payment / subscription | Validates demand before charging |
| Affiliate tracking | Out of scope by design |
| Living profile re-intake | MMP feature |
| Onboarding email sequences | Manual email sufficient at MVP scale |

### MVP Stack

```
Landing page:    Framer or Carrd
Intake:          Typeform or Tally → Airtable (via Zapier or native integration)
Member DB:       Airtable
Matching:        Manual (operator reviews Airtable, identifies pairs)
Comms:           Gmail for match notifications and introductions
Community:       Slack (free) or Circle (free tier)
Cost:            £0–£50/month (free tiers cover ~100 members)
```

### MVP Success Criteria

| Signal | Target | Notes |
|---|---|---|
| Founders completing intake | 20+ | Enough to make meaningful matches |
| Intake completion rate | >60% | If lower, questionnaire needs shortening |
| Match acceptance rate | >70% | Founder replies positively to match notification |
| Introduction taken (both respond) | >50% | Measures real engagement |
| Qualitative "this is useful" signal | 3+ unprompted | Leading indicator of WTP |

No revenue targets at MVP stage.

### MVP → MMP Transition Triggers

- MVP success criteria hit
- At least 5 MVP members confirm they'd pay
- Operator has validated match quality is maintainable at the 20+ member scale

---

## 6. MMP — Minimum Marketable Product

### Purpose

MMP is the version we charge for. It answers four questions:
1. **Will founders pay?** Is WTP strong enough to convert early-access members to paid subscriptions?
2. **Does matching quality hold at scale?** Can semi-automated matching maintain quality as member count grows?
3. **Does the community layer drive retention?** Do members stay beyond their first match?
4. **Is operator time per member sustainable?** MVP took ~2–4 hours/week for 20 members; MMP must serve 100+ without linear time growth.

### Architecture Decision

**Custom build from the start. No third-party community platform dependency.**

The living profile, matching engine, and community layer are designed as a coherent system. Third-party platforms (Circle, Skool, Slack) are not suited to the profile depth this product requires, and any integration creates UX seams that degrade the member experience at the exact point where trust matters most.

**MVP community layer:** Slack (temporary scaffold — not a platform decision)  
**MMP community layer:** Purpose-built, part of the custom application

```
Custom web application (Next.js)
├── Community layer (spaces, feed, DMs, member directory, events)
├── Member profile system (full living profile, progressive intake)
├── Matching engine (scoring, operator review, rationale, notification)
├── Operator admin dashboard
└── Subscription management (Stripe)
     ↕
Supabase (PostgreSQL + Auth + Realtime + Storage)
     ↕
Stripe (subscriptions, webhooks, Customer Portal)
     ↕
Resend + React Email (transactional email)
     ↕
Vercel (hosting)
```

Members have one login. One interface. Everything — community, profile, matching, notifications — lives in the same application.

### MMP Feature Set

**In scope:**

| Feature | Notes |
|---|---|
| Custom web application | Next.js + Supabase — community, profile, matching, admin in one build |
| Full living profile (85 fields, progressive) | Schema phased over first 60 days |
| Matching-critical fields required at signup | ~12 fields, under 10 minutes |
| Progressive profile enrichment prompts | Contextual, timed, completion-driven |
| 90-day living profile re-intake | Automated prompts on key changing fields |
| Open community spaces (no sector/stage segmentation) | General, Wins, Vent, Problems, Offers, Swap Shop, Education, Admin |
| Member directory (members-only, opt-in contact fields) | Searchable; website, LinkedIn, email, phone — each individually opt-in |
| Members' Offers space | Members post community-specific offers with operator guidance on offer structure |
| Swap Shop space | Skills and services trade; members post what they have and what they need |
| Educational content space | Operator-curated guides, templates, frameworks, recorded sessions |
| Community recognition / badges | Earned via community reactions; 5 levels; displayed on profile and directory card |
| Community feed (per space) | Posts, reactions (incl. weighted "This helped me" / "This solved my problem"), replies |
| Direct messaging | 1:1 and system-initiated |
| Match notification (DM + email) | Both channels always |
| Match acceptance → private shared space | Auto-created on both-party acceptance |
| Background matchmaking (opt-out) | Members do not see the mechanics; opt out via notification preferences |
| Semi-automated match scoring | Algorithm surfaces; operator approves |
| Draft rationale generation | System writes; operator edits |
| Operator admin dashboard | Member DB, match queue, analytics |
| Stripe subscriptions (Growth + Pro) | Monthly and annual, Customer Portal |
| Stripe webhook → access gating | Cancellation triggers access revocation at end of billing period |
| Events (basic) | Operator creates, members RSVP; recordings posted to Education space |

**Deferred to Phase 2:**

| Feature | Reason |
|---|---|
| Fully automated matching (no operator review) | Quality risk until algorithm is well-tuned |
| Referral outcome tracking | Trust layer and member reporting needed first |
| Commission processing between members | Platform creates connections, not transactions |
| White-label / B2B licensing | Parked until direct-to-founder MRR exceeds £5k/month + inbound signal |
| Mobile app | Responsive web sufficient at MMP scale |
| Free tier / freemium | Phase 2 acquisition strategy |
| AI-generated rationale (unreviewed) | Operator review is a quality gate |
| Video hosting | Link to external platforms |
| Course / curriculum builder | Not this product |
| Advanced search (Typesense/Algolia) | Postgres full-text sufficient to ~1,000 members |

### MMP Success Criteria

| Signal | Target | Notes |
|---|---|---|
| Paying members | 50+ | Validates WTP and covers infrastructure |
| MRR | £2,000+ | ~40 Growth or ~25 Pro members |
| Intake → paid conversion | >50% | Of MVP graduates offered MMP access |
| Match acceptance rate | >65% | Maintained from MVP despite semi-automation |
| 90-day retention | >70% | Still paying after 3 months |
| Operator time per member | <30 min/month | Sustainability at 50+ members |
| Profile completion (matching-critical) | >90% | Incomplete profiles degrade match quality |
| Profile completion (enrichment fields) | >50% | Signals engagement with living profile |

### MVP → MMP Transition Checklist

- [ ] MVP success criteria hit
- [ ] At least 5 MVP members confirm they'd pay
- [ ] Supabase schema designed and reviewed
- [ ] Next.js application scaffolded with auth, routing, and role-based access
- [ ] Profile editor built (required fields first, enrichment behind progress prompt)
- [ ] Community layer built: spaces, feed, DMs, notifications
- [ ] Matching engine built: scoring, operator dashboard, rationale generation, notification dispatch
- [ ] Stripe integration complete: Growth + Pro, monthly/annual, webhooks, Customer Portal
- [ ] MVP member data migrated from Airtable → Supabase
- [ ] End-to-end test: signup → intake → match → acceptance → introduction
- [ ] Stripe + access gating failure modes tested
- [ ] At least 5 MVP members converted to paid before launch announcement

---

## 7. The Living Profile

### Philosophy

- **Progressive, not front-loaded.** Members complete essential matching fields on signup (~12 fields, under 10 minutes). Enrichment fields are surfaced progressively over the first 30–60 days via contextual prompts.
- **Members own it.** The profile is the member's asset — a clear, honest picture of their business that is useful to them even independently of matching.
- **Living, not static.** Automated re-intake prompts at 90-day intervals ask about key fields that change: revenue, stage, ICP, offer.
- **Matching-critical fields are flagged.** The profile UI distinguishes [M] matching-critical fields (required at signup) from [E] enrichment fields (valuable context, not required) and [B] business intelligence fields (optional, member-controlled).

### Progressive Completion Model

**Day 0 (signup):** [M] fields only. ~12 fields. Under 10 minutes.

**Days 7–14 (first enrichment prompt):** Customers and Offer & Value sections. Prompt: "Your profile is 40% complete. Complete these sections to improve your match quality."

**Days 30–45 (second enrichment prompt):** Sales & Marketing, Operations, Tech Stack. Prompt: "Members with complete profiles receive 2x more match requests." *(Note: validate this claim against real matching data before using it.)*

**Day 90+ (living profile re-intake):** Automated prompt on key changing fields: annual revenue, growth constraint, ICP, introductory offer, partner types sought.

**Any time:** Member can update any field. Each section has a "Last updated" timestamp. The matching engine re-scores the member against the pool on any [M] field update.

### Full Profile Schema

Fields marked **[M]** are matching-critical (drive the scoring algorithm).  
Fields marked **[E]** are enrichment (valuable context, not required for initial matching).  
Fields marked **[B]** are business intelligence (optional, member-controlled visibility).

#### Section 1: Company

| Field | Type | Priority | Notes |
|---|---|---|---|
| Company name | Text | [M] | Required at signup |
| Website | URL | [E] | Operator due diligence |

#### Section 2: Essential / Matching Core

| Field | Type | Priority | Notes |
|---|---|---|---|
| Primary product/service | Long text | [M] | Required at signup — maps to Q1 of intake |
| Team size (category) | Dropdown | [E] | Just me / 2–5 / 6–20 / 21+ |
| Number of employees | Number | [B] | Optional detail |
| Primary delivery type | Dropdown | [E] | Do it yourself / Done with you / Done for you |
| Primary selling mechanism | Dropdown | [E] | In-person salesperson / Self-checkout / Online salesperson / Online self-checkout |
| Primary advertising mode | Dropdown | [E] | Warm outreach / Cold outreach / Content / Paid ads |
| Primary lead source | Dropdown | [E] | Self / Referrals / Affiliates / Agencies |
| Annual revenue (band) | Dropdown | [M] | Pre-revenue / Under £50k / £50k–£200k / £200k–£500k / £500k+ |
| Monthly revenue (band) | Dropdown | [M] | Maps to Q4d of intake. Pre-revenue / Under £2k / £2k–£5k / £5k–£15k / £15k–£50k / £50k+. **Private — operator and matching engine only. Never shown on member profile or directory.** |
| Biggest growth constraint | Long text | [M] | Feeds matching — a founder constrained by leads matches with someone who has leads to refer |

#### Section 3: Business Profile

| Field | Type | Priority | Notes |
|---|---|---|---|
| Industry / sector | Text | [M] | Required at signup — used for sector tagging |
| Business model | Dropdown | [E] | Recurring / subscription / low-volume high-ticket / high-volume low-ticket / services / one-time |
| Years in business | Number | [E] | Stage signal |
| Legal entity type | Text | [B] | Optional |
| Geography focus | Text | [M] | Required — UK local / national / international |
| Additional notes | Long text | [E] | Freeform context |

#### Section 4: Customers (Matching-Critical)

| Field | Type | Priority | Notes |
|---|---|---|---|
| Ideal Customer Profile (ICP) | Long text | [M] | Required at signup — maps to Q2 of intake. Primary matching field. |
| Customer segments | Long text | [M] | Enrichment pass 1 — sub-segments within ICP |
| Primary pain points | Long text | [M] | What problem does the member solve for their customer? Critical for matching rationale. |
| Top objections | Long text | [E] | What stops customers buying? Useful for partner education. |
| Top decision drivers | Long text | [E] | What makes customers choose them? |
| Total customers | Number | [B] | Optional |
| Average order value | Currency | [B] | Optional |
| Customer acquisition cost | Currency | [B] | Optional |
| Customer lifetime value | Currency | [B] | Optional |
| Monthly churn rate | Percentage | [B] | Optional |
| NPS score | Number | [B] | Optional |

#### Section 5: Offer & Value (Matching-Critical)

| Field | Type | Priority | Notes |
|---|---|---|---|
| Value proposition | Long text | [M] | Required at signup |
| Introductory offer | Long text | [M] | Required at signup — maps to Q4/Q4a of intake |
| Offer builder used | Boolean | [E] | Flag if member used offer builder |
| Offer packages | Long text | [E] | Full range of what they sell |
| Differentiators | Long text | [E] | Why they win over alternatives |
| Proof assets | Long text | [E] | Case studies, testimonials, results |
| Guarantees | Long text | [E] | Risk reduction signals |
| Promotions | Long text | [E] | Current offers — time-sensitive, needs refresh |

#### Section 6: Referral & Partnership (Matching-Critical)

| Field | Type | Priority | Notes |
|---|---|---|---|
| Partnership type preferences | Multi-select | [M] | Maps to Q4c. Referral / Affiliate / Mutual benefit. All selected by default — opt-out model. Hard filter: never propose a match type a member has opted out of. |
| Referral arrangement offered | Multi-select | [M] | Required at signup — maps to Q5. Commission / flat fee / reciprocal / other |
| Referral commission rate | Text | [E] | Specific rate if commission selected |
| What they want referred to them | Long text | [M] | Required at signup — maps to Q6 |
| Past referral experience | Dropdown | [M] | Maps to Q8. Calibrates onboarding depth. |
| Partner types sought | Long text | [M] | What kinds of businesses would make ideal partners? |
| Industries to avoid | Long text | [E] | Conflicts or bad fits |
| LinkedIn | URL | [M] | Required — operator due diligence |

#### Section 7: Sales & Marketing

| Field | Type | Priority | Notes |
|---|---|---|---|
| Primary marketing channel | Text | [E] | Channel complementarity signal |
| Marketing channels (full list) | Long text | [E] | |
| Average deal size | Currency | [B] | |
| Sales cycle length | Number (days) | [B] | |
| Close rate | Percentage | [B] | |
| Monthly leads/visitors | Number | [B] | |
| Monthly new customers | Number | [B] | |
| Conversion rate | Percentage | [B] | |
| Lead-to-customer rate | Percentage | [B] | |
| Messaging angles | Long text | [E] | |
| Competitors | Long text | [E] | Matching exclusion — don't match with a competitor's supplier |

#### Section 8: Operations

| Field | Type | Priority | Notes |
|---|---|---|---|
| Customer acquisition | Long text | [E] | How they currently get customers |
| Customer onboarding | Long text | [E] | |
| Product/service delivery | Dropdown | [B] | Software / Information / Services / Physical products |
| Primary business processes | Long text | [B] | |
| Team structure | Long text | [B] | |
| Workflow stages | Long text | [B] | |
| Vendor dependencies | Long text | [B] | Could surface partner opportunities |
| Operations capacity | Long text | [B] | |

#### Section 9: Financials

| Field | Type | Priority | Notes |
|---|---|---|---|
| Monthly revenue | Currency | [B] | Optional — member discretion |
| Annual revenue (exact) | Currency | [B] | Optional — member discretion |
| Gross margin | Percentage | [B] | |
| Net margin | Percentage | [B] | |
| MRR growth rate | Percentage | [B] | |
| Monthly burn rate | Currency | [B] | |
| Runway (months) | Number | [B] | |
| Cash flow profile | Long text | [B] | |

*Financial fields are optional and sensitive. Surface in a clearly privacy-labelled section — members control visibility.*

#### Section 10: Growth Planning

| Field | Type | Priority | Notes |
|---|---|---|---|
| 12-month revenue goal | Currency | [E] | Ambition level matching signal |
| Main growth channel | Text | [E] | |
| Growth strategy | Long text | [E] | |
| Growth constraints | Long text | [M] | Overlaps with Section 2 "biggest growth constraint" — consolidate at implementation |
| Exit timeline | Text | [B] | Optional |
| Exit goals | Long text | [B] | Optional |
| Funding needed | Currency | [B] | Optional |

#### Section 11: Tech Stack

| Field | Type | Priority | Notes |
|---|---|---|---|
| Financial & accounting tools | Text | [E] | Partner opportunity signal |
| Customer & analytics tools | Text | [E] | |
| Sales tools | Text | [E] | |
| Marketing tools | Text | [E] | |
| Other platforms | Text | [E] | |

#### Section 12: Brand

| Field | Type | Priority | Notes |
|---|---|---|---|
| Brand voice | Long text | [E] | Partner communication calibration |
| Prohibited terms | Long text | [B] | Niche use case |
| Trust signals | Long text | [E] | Accreditations, memberships, press |

#### Section 13: Compliance

| Field | Type | Priority | Notes |
|---|---|---|---|
| Licenses held | Long text | [B] | Relevant for regulated industries (finance, legal, health) |
| Ad restrictions | Long text | [B] | Optional |
| Regulatory notes | Long text | [B] | Optional |

*Compliance section shown conditionally based on industry — relevant to IFAs, mortgage brokers, healthcare providers.*

---

## 8. Intake Questionnaire

### Design Principles

- No jargon — no "ICP", "niche", "affiliate", "conversion". Plain English throughout.
- Every question has an example answer and hint text.
- Quality framing upfront: answers determine match quality.
- Built-in offer creation — if a founder doesn't have a free referral offer, the form walks them through creating one.
- Two matching gates embedded in the form: (1) free member referral offer, (2) partner visibility commitment. Both must be confirmed by the operator before a member enters the match pool.
- Completion target: under 5 minutes with an existing offer; up to 12 minutes with the offer builder and partner visibility questions.
- Format: one question per screen, progress indicator, conversational tone.

### Pre-Form Copy (above the Start button)

> **This isn't a standard sign-up form.**
>
> We use your answers to match you with businesses that are already serving your customers — so when you refer each other, it feels natural rather than forced.
>
> The more specific you are, the better your matches will be. Vague answers produce vague matches. Take 5 minutes and do it properly — it's worth it.
>
> We'll never share your answers publicly. Everything here is used only to find you the right partner.

### Question Set

**Q1 — What your business does**

Label: "What does your business do?"

Hint: "Be specific. 'I'm a marketing consultant' tells us very little. 'I help independent restaurants fill tables during the week using email and social media' tells us everything."

Example: *"I'm a bookkeeper who works with e-commerce businesses turning over £100k–£500k. I help them get their accounts clean, understand their numbers, and stop dreading tax time."*

Type: Long text. Matching use: Offer description + ICP signal.

---

**Q2 — Who your customers are**

Label: "Who do you work with?"

Hint: "Think about your best customers — the ones who are easiest to work with, get the most value, and refer others. Describe them as if you're telling a friend who to introduce you to."

Example: *"Small business owners who've been trading for 2–5 years, usually 3–10 employees, turning over £200k–£1m. They're growing but their admin is a mess and they know it."*

Type: Long text. Matching use: Primary ICP signal. Most important field for matching.

---

**Q3 — Where your business is right now**

Label: "How's business going right now?"

Options (single select):
- Just getting started — working on it but don't have many paying customers yet
- Early days — have paying customers but it's still unpredictable month to month
- Getting traction — things are working, bringing in £5k–£25k a month
- Established — consistently doing £25k+ a month

Type: Multiple choice. Matching use: Stage filter (soft — not a hard block).

---

**Q3b — Current pain / highest priority problem** *(new)*

Label: "What's the biggest challenge in your business right now — the thing keeping you up at night or sitting at the top of your to-do list?"

Hint: "There are no wrong answers. It might be finding customers, cash flow, a skills gap, a specific operational problem, or something else entirely. This helps us connect you with people who might be able to help — or who've been in the same position."

Example: *"I've got a great product but I don't know how to market it without spending a fortune on ads. Every approach I've tried has either cost too much or produced nothing."*

Type: Long text (optional — but strongly encouraged).

Operator use: This field is read at intake and used in two ways: (1) the operator checks whether any existing member could help address this problem — if so, it becomes part of the match rationale; (2) the operator may direct the new member toward relevant educational content, community spaces, or events that address the problem. This field is not used in the automated scoring algorithm but is a qualitative signal for operator judgment.

---

**Q4 — The free member referral offer** *(matching gate 1)*

Every member must have a free offer — a specific, deliverable thing they provide exclusively to other members and the clients those members refer, in exchange for a testimonial or review. This is the trust-building mechanism that gives partners confidence to refer. The offer should be the member's attraction offer: a review, audit, assessment, or diagnosis.

Label: "Do you have a free offer — a short, specific thing you could do for someone to show them the value of working with you?"

Hint: Explains that the offer must be free (not discounted), specific (a review, audit, assessment — not "a chat"), and describable in two sentences. Explains the trade: free offer in exchange for a testimonial.

Options (single select):
- Yes, I have a free offer I can describe → Q4a
- Not yet — I need help shaping one → Offer Builder

**Q4a** (if Yes): "Describe your free offer in a sentence or two." Long text. Operator confirms it qualifies before member enters match pool.

**Offer Builder** (if Not yet): Four-question mini-flow (what quick win can you give, can you offer it free in exchange for a testimonial, make it specific with time/output, give it a working title). Framed as helpful, not as a barrier. Outputs a qualifying offer before continuing.

**Operator gate:** After intake submission, operator confirms (1) the offer is genuinely free, (2) it is a discrete deliverable, and (3) a non-expert partner could describe it in two sentences. Member does not enter the match pool until confirmed.

---

**Q4b — Partner visibility** *(matching gate 2)*

Every member must commit to actively making their partners discoverable to their own client base. Mechanism depends on business type.

Label: "When you partner with another business on here, how would your clients or customers know about them?"

Options (single select):
- I have physical premises — I can display partner materials (cards, flyers) where clients see them
- I'm primarily online — I can add a partner/affiliate section to my website
- Both — I have physical premises and an online presence
- Neither applies → flags for operator review

**Physical branch:** Confirms member will display business cards, flyers, or similar in their premises.

**Online branch:** Confirms member will create a partner or affiliate section on their website (or equivalent — LinkedIn recommendations accepted as interim for members without a website).

**Operator gate:** Operator confirms visibility commitment before member enters match pool. "Neither applies" responses require a follow-up conversation before matching proceeds.

---

**Q4c — Partnership type preferences** *(opt-out, not opt-in)*

The platform supports three types of match: referral, affiliate, and mutual benefit. By default, members are open to all three. This question lets them opt out of any type they don't want — but the framing is deliberately positive. Most members should leave all three selected.

Label: "What kinds of partnerships are you open to?"

Hint: "We find three types of match. Most members keep all three on — you might be surprised what comes up. Untick any you definitely don't want."

Options (multi-select, **all selected by default**):
- ✓ **Referral** — we send each other clients and pay a fee when one converts
- ✓ **Affiliate** — one or both of us promotes the other to our audience or clients
- ✓ **Mutual benefit** — we solve a problem for each other directly, even if our customers are different (e.g. a caterer who sets up at a business's premises)

UX note: Render as toggles or checkboxes, all ticked. The prompt is "untick anything you don't want" — not "select what applies". A member who leaves all three ticked has done the right thing. Opt-out friction keeps the match pool broad.

Operator note: A member who opts out of all three flags for review — this likely means they misunderstood the question.

Matching use: Hard filter — never propose a match type a member has opted out of. Inform rationale framing.

---

**Q4d — Revenue stage** *(private — never shown publicly)*

Revenue stage improves match quality. Early-stage founders often benefit most from other early-stage founders who are in referral-building mode, rather than established businesses who may have little incentive to invest in a new partner. That said, mixed-stage matches can work well — this is a soft signal, not a hard filter.

Label: "Roughly how much is your business bringing in each month right now?"

Hint: "This helps us find the right kind of match for where you are. It's private — no one else on the platform sees this."

Options (single select):
- Nothing yet — I'm still getting started
- Under £2,000 a month
- £2,000–£5,000 a month
- £5,000–£15,000 a month
- £15,000–£50,000 a month
- Over £50,000 a month — I'd rather not say

Privacy note: This field is stored against the member profile but never shown on their public or directory profile. It is visible to the operator in the admin dashboard and used by the matching engine as a soft signal.

Matching use: Soft signal — stage proximity. Not a hard filter. Inform operator rationale.

---

**Q5 — Affiliation offer — what you'd pay a partner who sends you a client**

Every member must have a financial incentive on the table for partners who refer clients to them. Reciprocal-only arrangements are acceptable when both parties agree explicitly, but must not be the only option offered.

Label: "If a partner referred a client to you and that client signed up, what would you pay the partner?"

Hint: Explains that the platform requires a financial offer — percentage of first invoice (10–20% typical), flat finder's fee, or equivalent to the cost of the member's free introductory offer paid to the referring partner.

Options (multi-select):
- A percentage of the first invoice — I'm open to discussing the rate → conditional text for rate
- A flat fee per referral that converts → conditional text for amount
- The full cost of my free introductory offer, paid to the partner when a referral takes it up
- Reciprocal referrals — we agree to actively send each other business, no money changes hands

Reciprocal-only: soft-flagged for operator review. Matching use: Commercial fit filter.

---

**Q6 — What you want a partner to send you**

Label: "What would you want a referral partner to send your way?"

Hint: "Be as specific as you can. The more clearly you describe the right referral, the easier it is for a partner to spot them."

Type: Long text. Matching use: Match direction — cross-referenced against what other members can plausibly refer.

---

**Q7 — Geography**

Label: "Where are your customers, and where are you based?"

Options (single select):
- My customers are mostly local or regional — geography matters
- My customers are across the UK — location doesn't really matter
- My customers are international — location definitely doesn't matter
- It's a mix — both local and national

Type: Multiple choice. Matching use: Geography filter.

---

**Q8 — Referral experience**

Label: "Have you ever been in a referral or partner arrangement with another business before?"

Options (single select):
- Yes, and it worked well — I know how these work
- Yes, but it never really came to anything
- No, but I'm keen to try
- No, and I'm still figuring out if it's right for me

Matching use: Onboarding calibration — determines depth of explanation in match notification.

---

**Q9 — LinkedIn**

Label: "What's your LinkedIn profile URL?"

Hint: "We use this to confirm you're who you say you are. We won't contact you through LinkedIn."

Type: URL. Matching use: Operator due diligence.

---

**Q10 — Anything else** (optional)

Label: "Anything else we should know?"

Hint: "Specific partner types you'd love to find? Industries to avoid? Something that's gone wrong in a past referral arrangement?"

Type: Long text. Matching use: Free-text context for operator.

---

### Form Flow

```
Landing page → Form intro (quality framing) → Language note screen
  → Q1: What you do
  → Q2: Who your customers are
  → Q3: Where you're at
  → Q3b: Biggest current challenge / highest priority problem (optional but encouraged)
  → Q4: Do you have an introductory offer?
       ├── YES → Q4a: Describe it → Q4c
       └── NO/UNSURE → Offer Builder (OB1 → OB2 → OB3) → Q4c
  → Q4c: Partnership types (all selected by default — opt-out)
  → Q4d: Revenue stage (private)
  → Q5: What you'd give a partner
  → Q6: What you want a partner to send you
  → Q7: Where your customers are
  → Q8: Referral experience
  → Q9: LinkedIn
  → Q10: Anything else (optional)
  → Thank you screen
```

### Thank You Screen

> **You're in.**
>
> We review every application personally — no algorithm, just a human being reading what you've written and thinking carefully about who in our community would be a good fit for you.
>
> We'll be in touch within 3 business days with either a match or an update. In the meantime, you'll get a short email from us with a bit more about how the introductions work.
>
> Thanks for taking the time to fill this in properly. It makes a real difference.

---

## 9. Matching Engine

### MVP: Manual Matching

The operator runs the matching loop in Airtable. Four stages:

**Stage 1 — Intake review and gate confirmation:** Read Q1–Q10. Apply ICP tags and sector tag. Then confirm both matching gates:

- **Gate 1 — Free member referral offer:** Does the offer qualify? It must be (a) genuinely free, not discounted, (b) a discrete deliverable — not "a chat" or "a call", and (c) describable by a non-expert partner in two sentences. If it fails, contact the member to refine before proceeding. Tick "Free offer confirmed" in Airtable when satisfied.

- **Gate 2 — Partner visibility commitment:** Has the member committed to displaying partner materials (physical) and/or creating a partner/affiliate section (online)? If they selected "Neither applies" or their commitment is unclear, contact the member to confirm before proceeding. Tick relevant "Partner visibility confirmed" field(s) in Airtable when satisfied.

Only once both gates are ticked does the "Match pool eligible" field become true and the member enter the matching queue. Set match status to `Unmatched`.

**Stage 2 — Match identification:** Run a match pass after every 3–5 new eligible intakes. Work through `Unmatched` members sorted by date joined (oldest first — they've been waiting longest). Apply matching criteria in priority order (see below).

**Matching criteria (priority order):**
1. Customer overlap (required) — shared ICP tags
2. Complementary services (required) — different sector tags; no competitor matches
3. Referral arrangement compatibility (strong signal) — Q5 alignment
4. Stage proximity (soft signal) — Q3 alignment
5. Geography (relevant for local service businesses) — Q7 alignment

**Stage 3 — Match decision:** Pre-send sanity check: Can you explain specifically why these two should meet? Is there a clear referral direction? Is there a plausible offer to anchor the introduction?

Write a one-paragraph match rationale before drafting the email — specific, not template-like.

**Stage 4 — Outreach:** Send match notification to each member separately (they haven't consented to sharing contact details yet). Wait for acceptance. On both-party acceptance, send introduction email with both CC'd.

### MMP: Semi-Automated Matching

When a member completes or updates any [M] profile field, the engine re-scores them against all other unmatched members.

**Pre-condition:** Only members with `match_pool_eligible = true` (both matching gates confirmed) are scored against each other.

**Score = weighted composite (0–100):**

| Signal | Weight | Source fields |
|---|---|---|
| ICP overlap | 30% | ICP, customer segments, primary pain points |
| Sector complementarity | 25% | Industry/sector tag — penalises same-sector matches |
| Offer & referral fit | 20% | Member referral offer, affiliation offer type, what they want referred |
| Stage proximity | 10% | Monthly revenue band, annual revenue band, years in business, team size |
| Partnership type compatibility | 10% | Partnership type preferences — hard exclude if no overlap; soft boost if strong overlap |
| Geography compatibility | 3% | Geography focus |
| Growth constraint alignment | 2% | Biggest growth constraint |

**Pre-score filter:** Partnership type preferences are applied before scoring. If two members share no compatible partnership type (e.g. one has opted out of referral and affiliate, the other only wants referral), they are excluded from each other's candidate pool entirely — no score calculated.

- Candidates scoring ≥60 surfaced to operator as match candidates
- Candidates scoring ≥80 flagged as high-confidence

**Operator review flow (MMP):**
1. Operator sees unmatched members ranked by days waiting (longest first)
2. Top 3 candidates per unmatched member, ranked by score with breakdown
3. Operator can view full profile of any candidate before deciding
4. Operator approves or dismisses (dismissal requires reason — feeds algorithm refinement)
5. On approval: system generates draft match rationale from profile data
6. Operator edits rationale, confirms, sends — notification dispatched as DM + email to both members

**Match notification template (auto-drafted, operator-edited):**

> **[Member B name]** runs **[business name]** — [primary product/service, one sentence].
>
> Here's why I think this is worth your time:
>
> [Rationale — auto-generated from shared ICP, complementary sectors, referral direction. Operator edits for specificity and voice.]
>
> **Their free offer for your clients:** [Member B's free member referral offer — the specific thing they'll do for free for anyone you refer to them, in exchange for a testimonial]  
> **What they'd pay you for a referral:** [Member B's affiliation offer — commission %, flat fee, or equivalent of their free offer cost]  
> **What they're looking for from a partner:** [Member B's "what they want referred" field]
>
> Reply to accept this introduction, or let me know if it's not the right fit.

**Match acceptance flow:**
- Both members accept → system creates private shared space, posts introduction message, notifies both
- One declines → both return to unmatched pool; operator notified, reason logged
- No response after 5 days → operator notified, optional follow-up prompt sent

---

## 10. Community Layer

### Design Principle

The community layer is part of the same application as matching and profiles. It does not need to match Circle or Skool feature-for-feature. It needs to be good at the specific things that matter for this product: structured spaces that reduce noise, a directory that makes members discoverable, direct messaging that supports introductions, and events that drive regular engagement.

The community is deliberately open — members are not segmented by sector or stage within the main spaces. Business is business, and members at different stages and in different sectors all have something to contribute to shared problems, shared wins, and shared concerns. The value of an open community is that a founder at month six learns from a founder at year three in the same conversation. Segmentation is the exception, not the rule — spaces are added where there is a specific need, not as a default structure.

### Required Features at MMP

**Matchmaking (opt-in, background)**

Matching runs as a background process. Members do not see the mechanics — they receive a match notification when the operator identifies a suitable pairing. Members can opt out of receiving further matches via their notification preferences without leaving the community. The matchmaking process is never surfaced as a visible feed or queue to members — it is invisible infrastructure.

**Spaces (structured channels)**

The community uses a small number of open spaces available to all members. Spaces are not auto-assigned by sector or stage — members join the whole community and can post in any space. New spaces are added by operators when a genuine ongoing need exists; spaces are removed or merged if they become inactive.

Default spaces at MMP launch:

| Space | Purpose |
|---|---|
| General | Default landing space — announcements, general discussion, introductions |
| Wins | Celebrating milestones, successful introductions, results from partnerships |
| Vent | A safe space to express frustration, offload stress, say the thing you can't say publicly. Human, honest, low-stakes. |
| Problems | Post a current challenge and get input from the community. No obligation to take advice — just a space to think out loud and hear other perspectives. |
| Offers | Members post the specific offers they are making to the community (see Members' Offers below) |
| Swap Shop | Trade services — post what you have, post what you need. Skills and services only, no cash transactions. |
| Education | Operator-curated content: guides, frameworks, templates, recorded sessions. Members can comment; operators post. |
| Admin / Announcements | Read-only for members. Operator posts platform updates, policy changes, event reminders. |

Spaces are additive — the operator can open new spaces as genuine community need emerges. Spaces can be archived. No space should exist without posts at least weekly at maturity.

Private match spaces — auto-created on both-party acceptance — are listed separately in each member's sidebar, below the main spaces, with a lock icon. Named "FirstName + FirstName — Partnership".

**Member Directory**

A members-only, searchable directory. Members can control which contact fields are visible to other members.

Directory card (visible to all logged-in members):
- Name and business name
- Sector and location
- One-line description (from their profile value proposition)
- Current member referral offer (the free offer — helps members identify who to refer)
- Member since date

Full profile view (on card click):
- All non-private profile fields as set by the member
- Contact details: website URL, LinkedIn URL, email address, phone number — each individually opt-in/opt-out by the member via their privacy settings

Privacy defaults:
- Website: visible by default (low sensitivity)
- LinkedIn: visible by default
- Email: opt-in only (hidden by default; member must explicitly enable)
- Phone: opt-in only (hidden by default; member must explicitly enable)

Members can update their directory visibility at any time from their profile settings. No contact detail is displayed publicly — the directory is members-only.

**Members' Offers Space**

A dedicated space where members post commercial offers available to the community. This is separate from their member referral offer (the free offer used for matching) — it is their broader offer to the community as paying members.

Offer post structure:
- What it is (one-line description)
- Who it's for
- What's included
- Price or terms — see Offer Guidance below
- How to take it up (DM the poster, email, link)

**Offer Guidance (shown to members when posting an offer):**

> **What should my offer look like?**
>
> There's no rule that says community offers have to be free. Here's a simple way to think about it:
>
> **If you're early and building trust:** Consider offering a free or heavily subsidised service to a handful of community members. You get testimonials and case studies. They get real help. Your referral partner can confidently send people your way because there's proof you deliver. Free offers work best when you need social proof more than immediate revenue.
>
> **If you're established and want to generate referrals:** A member discount — even a modest one — gives partners a reason to mention you and gives members a reason to try you. The discount doesn't need to be dramatic. Enough that someone would say "they do a deal for people in this community" is enough. Physical product businesses especially: don't give away below cost. The point is a meaningful gesture, not a loss.
>
> **If you just want to be visible:** Post your standard offer with a note that you're open to conversations. Not every offer needs a price reduction — sometimes just being known is the first step.
>
> The goal is that members and their referral partners feel like this community has something worth sharing. What that looks like for your business is your call.

**Forums / Community Spaces Feed**

Each space has a chronological post feed. Post types:

- Member posts: text, links, questions, images
- System posts: match acceptance announcements (opt-in), member milestones, operator updates — visually distinct from member posts
- Reactions: emoji reactions on any post (minimum: 👍 🙌 💡 ❤️ — expandable)
- Replies: one level of threaded replies per post

The Problems space and Vent space have the same mechanics as other spaces, with a different tone set by framing copy pinned at the top of each:

*Problems space pin:* "Post a problem you're working through and see what the community thinks. No obligation to take advice — sometimes just writing it out helps. Others might have been exactly where you are."

*Vent space pin:* "Sometimes you just need to say it. This is a safe space — what's shared here stays here. No judgement. No advice unless you ask for it."

**Educational Content Space**

The Education space is operator-curated. Operators post:
- Guides (how referral arrangements work, how to structure a partnership deal, how to write a partner visibility page)
- Templates (partner agreement language, referral tracking log, introduction email scripts)
- Recorded sessions (calls and workshops posted post-event)
- Frameworks (matching logic explained, offer builder guidance, deal-structuring steps)

Members can comment on educational posts. Members cannot post original content to the Education space — this keeps the signal-to-noise ratio high and ensures quality. Members can share educational posts into other spaces.

**Swap Shop Space**

A dedicated space for skills and services exchange. Members post what they have (a skill or service they can offer) and what they need. Other members respond if they can help.

Swap post types:
- "I have" post: "I can offer [X service/skill] — I'm looking for [Y in return]"
- "I need" post: "I'm looking for someone who can [X] — I can offer [Y] in return"

Rules (shown as pinned note in the space):
- Skills and services only. No cash transactions through the platform.
- Arrangements are made directly between members. The platform is not party to any agreement.
- Post honestly about what you can provide and what you need.

Examples: a LinkedIn marketing specialist offering their time in exchange for web design help. A copywriter offering content in exchange for bookkeeping. A photographer offering headshots in exchange for HR advice.

**Gamification — Community Recognition**

Members earn recognition for contributing helpfully to the community. This is visible within the community and displayed on member profiles and directory cards.

Recognition is based on community votes — not platform-generated metrics:
- Reactions on posts (each emoji reaction counts as one point)
- A dedicated "This helped me" reaction (weighted higher — counts as 3 points)
- A member marking a reply as "This solved my problem" (weighted highest — counts as 5 points)

Recognition levels (names TBC — to be set by operator before launch):

| Level | Points | Badge |
|---|---|---|
| New member | 0–49 | — |
| Contributor | 50–199 | Bronze badge |
| Trusted member | 200–499 | Silver badge |
| Community pillar | 500–999 | Gold badge |
| Community legend | 1000+ | Platinum badge |

Badge display:
- Shown on directory card next to member name
- Shown on community posts next to avatar
- Shown on member profile under their name

Design note: badges should be understated — a small icon that signals status without dominating the UI. No leaderboard. No public point totals. The goal is recognition for helpfulness, not a points competition.

**Implementation note:** Points do not decay. Badges are cumulative achievements. Members keep their level even if they go quiet for a period — the system rewards contribution, not recency.

**Direct Messaging**

- 1:1 DMs between any two members
- Match notifications delivered as DMs from system account
- Introduction DM thread created on match acceptance (both members added)
- Named private spaces preferred over bare DM threads for match introductions (e.g. "Chris + Sarah — Partnership") — more intentional, easier to find later

**Notifications**

- In-app notifications (bell icon)
- Email digest (daily or weekly — member preference)
- Match notification: always delivered as both in-app DM and email

**Events**

- Operator creates events (group calls, workshops)
- Members RSVP
- Event reminders via notification
- Post-event recording/notes posted to Education space

**Member Onboarding Flow**

- After signup and payment: guided profile completion
- Progress indicator ("Your profile is X% complete")
- Contextual prompts at key completion milestones

### Explicitly Not Building at MMP

- Video hosting (link to Loom/YouTube)
- Course/curriculum builder
- Payment processing between members
- Public-facing community (members-only always)
- Mobile app (responsive web sufficient)

---

## 11. Operator Admin Dashboard

A separate interface (same codebase, different role — not visible to members).

### Member Database

- All members with: name, business, sector, ICP tags, stage, subscription tier, match status, profile completion %, date joined
- Filter by any field
- Full profile view per member
- Manual tag override (operator can correct auto-assigned sector/ICP tags)

### Match Queue

- Unmatched members sorted by days waiting (longest first)
- Match candidate surfacing with scores and breakdown
- Approve / dismiss workflow (dismissal requires a reason)
- Draft rationale editor — plain textarea with auto-draft pre-populated (no rich text editor needed)
- Match history per member

### Living Profile Queue

- Members due for 90-day re-intake prompt
- Members with incomplete profiles (below threshold completion %)
- Manual trigger for individual prompts

### Analytics

- Total members, active subscriptions, MRR, growth rate
- Intake completion rate, profile completion distribution
- Match acceptance rate, introduction taken rate
- 30/60/90-day retention
- Churn rate, cancellation reasons

---

## 12. Subscription Model

### Pricing Philosophy

The price must justify itself quickly. A member who gets one new client introduction in their first month has already covered the cost many times over. Pricing is therefore justified by outcomes — not features. Every feature in the tiers below exists to make a successful match and a productive partnership more likely.

No free tier at MMP. A free tier creates low-commitment profiles that degrade match quality for paying members. Freemium is a phase 2 acquisition strategy, not a launch feature.

Both monthly and annual billing are offered. Annual provides a meaningful discount as a reward for commitment — it is presented as the better-value option at checkout, but monthly is not hidden. Some members, particularly early-stage founders, will need to see results before committing annually.

### Pricing Tiers

#### Growth — £49/month or £399/year (~32% saving)

The entry tier. Designed for founders and SME owners who want to explore partnership-based growth and are willing to invest a modest recurring amount before they've seen results. At £49/month, one new client introduction more than covers the cost.

**Included:**

| Feature | Detail |
|---|---|
| Full living profile | All 85 fields, progressive completion, 90-day re-intake prompts |
| Curated matches | Up to 2 operator-reviewed matches per month |
| Match notifications | Delivered via in-app DM and email — always operator-reviewed, never automated |
| Match acceptance + private space | On both-party acceptance, a private shared space is created for the introduction |
| Community access | Full access to sector spaces, stage spaces, general space, and member directory |
| Referral education content | All guides, templates, and deal-structuring resources |
| Self-paced onboarding | Guided profile completion, contextual prompts, offer builder |
| Events | RSVP access to all operator-run group calls and workshops |

**Match volume rationale:** 2 matches/month is the right ceiling for Growth. More matches before a member has embedded their first partnership reduces quality attention on each. Members who are actively working a current partnership should focus on that before receiving a new one — the living profile re-intake ensures new matches improve over time.

#### Pro — £79/month or £599/year (~37% saving)

For members treating partnership-based growth as a primary channel — not an experiment. The Pro tier is for members who are ready to move fast, want more introductions, and benefit from a more hands-on start.

**Included: everything in Growth, plus:**

| Feature | Detail |
|---|---|
| Priority matching | Pro members are reviewed first in the operator match queue. When the queue is being processed, Pro members are surfaced ahead of Growth members with the same wait time. |
| Higher match volume | Up to 4 operator-reviewed matches per month |
| 1:1 onboarding call | A 30-minute call with the operator after joining — to review the member's profile, refine their free offer, confirm their partner visibility commitment, and set expectations for the first match. Delivered within 7 days of signup. |
| Early feature access | Pro members get access to new platform features before they roll out to Growth |
| Profile review | Operator reviews matching-critical fields within 48 hours of signup and provides written feedback if anything would reduce match quality |

**Pro tier rationale:** The 1:1 onboarding call is the primary differentiator. Members who start with a reviewed, refined profile and a clear free offer get better first matches. The operator time cost (~30 min/member) is justified by the higher subscription revenue and the improvement in match quality data.

### What Each Tier Is Designed to Deliver

Both tiers exist to deliver the same outcome — a member's first (or next) successful commercial partnership. The difference is speed and depth of support.

A Growth member on a clear business with a well-defined ICP and a good free offer should receive a first match within 2–4 weeks and have an accepted introduction within their first month.

A Pro member should have a reviewed profile, a confirmed free offer, and a first match within 2 weeks — with the operator able to explain specifically why that match was made.

### Founding Member Rate

Trial members who join before public launch are offered a founding rate: approximately half the standard Growth tier price, locked in for as long as they remain subscribed. This creates a genuine and compelling reason to join early, and strong retention incentive. The founding rate is disclosed before the trial ends with advance notice and the option to subscribe before the standard rate applies.

### Pricing Anchor

The most direct pricing justification is outcome-based. One new client introduction that converts is worth multiples of the monthly fee. Marketing copy should use real member outcomes where available ("our members report X new introductions in their first 90 days") — see `docs/COPY.md` for copy rules. Do not anchor against other platforms by name.

### Payment Infrastructure

- **Payment:** Stripe subscriptions
- **Self-serve:** Stripe Customer Portal (upgrade, downgrade, cancel)
- **Access gating:** Stripe webhooks → Supabase. Cancellation triggers access revocation at end of billing period.
- **Failure modes to test:** Payment failure, cancellation, upgrade/downgrade, webhook retry

---

## 13. Tech Stack

| Layer | Tool | Rationale |
|---|---|---|
| Frontend | Next.js (React) | Full-stack framework, SSR for SEO, API routes for backend logic |
| Styling | Tailwind CSS | Utility-first, rapid iteration, avoids generic community platform aesthetic |
| Database | Supabase (PostgreSQL) | Open-source, self-hostable, real-time subscriptions for feed/DMs, built-in auth |
| Auth | Supabase Auth | Single login, JWT-based, supports Google social login |
| Payments | Stripe | Subscriptions, webhooks, Customer Portal |
| Email | Resend + React Email | Transactional email with branded templates |
| File storage | Supabase Storage | Profile images, uploaded assets |
| Hosting | Vercel | Next.js optimised, generous free tier, easy scaling |
| Real-time (DMs/feed) | Supabase Realtime | WebSocket-based live updates for messaging and notifications |
| Search | Postgres full-text search (via Supabase) | Member directory and profile search. Comfortable to ~1,000 members; upgrade to Typesense at ~500 members to get ahead of it |
| Intake form (MVP) | Typeform / Tally → Supabase | MVP intake piped in; replaced by native profile editor at MMP |

**Estimated MMP infrastructure cost:** £50–£150/month at launch (Supabase Pro ~£22, Vercel Pro ~£17, Resend free–£15, Stripe 1.5% + 20p per transaction).

**Self-hosting path:** Supabase is open-source and self-hostable. If platform scale makes Supabase pricing a concern, migration to self-hosted is feasible without rewriting application code.

---

## 14. UI/UX Requirements

*This section specifies design requirements for handoff to a designer. The design system is defined in `DESIGN.md` — a Linear-derived dark-canvas system. All token references below (`{colors.*}`, `{typography.*}`, `{spacing.*}`, `{rounded.*}`) map directly to that file. Read DESIGN.md before implementing any component.*

---

### 14.1 Design Principles

**Dark-canvas professional tool, not a social platform.** The product is about generating business revenue. The aesthetic is dense, purposeful, and built around content — specifically the member profile and match data. Avoid the look of Skool, Circle, or generic community SaaS. The Linear marketing canvas (`{colors.canvas}` #010102) is the system anchor — near-pure black with a faint blue tint.

**The product UI is the protagonist.** Following the Linear pattern, every section of the marketing site and every key screen of the product should lead with a high-fidelity capture or representation of the actual product UI. The chrome is a dark frame; the content carries the weight.

**Clarity over cleverness.** Founders are time-poor and sceptical. Every screen communicates its purpose within 3 seconds. No decorative complexity, no atmospheric gradients, no spotlight cards.

**Trust through specificity.** The platform's value depends on trust — members share sensitive business data. Design reinforces this through precision (specific field labels, human-attributed match rationale) not warmth theatre (stock photography, generic reassurance copy).

**Dark canvas IS the whitespace.** Sections separate by surface lift onto `{colors.surface-1}` panels, not by gaps in white. Within panels, `{spacing.lg}` 24px between content blocks; `{spacing.section}` 96px between sections. The 85-field profile is made manageable through section-based progressive disclosure within this rhythm — not by cramming fields into dense lists.

**Restrained gamification only.** The community layer includes recognition badges for helpful contributors (see Section 10). These are understated — a small badge icon next to a member's name, not a leaderboard or points counter. No streak counts, no leaderboard language, no XP bars. The product is not Skool. The distinction: community recognition for genuine helpfulness is earned and quiet; gamification aesthetics as a growth mechanic are not this product.

---

### 14.2 Design System Reference (DESIGN.md)

All implementation must follow `DESIGN.md`. Key constraints summarised here for PRD readers:

**Colour usage rules:**
- `{colors.canvas}` (#010102) — page background; never use `#000000` true black
- `{colors.primary}` (#5e6ad2, lavender-blue) — reserved for: brand mark, primary CTA button, focus rings, link emphasis only. Not a section background or card fill. No second chromatic accent.
- `{colors.surface-1}` through `{colors.surface-4}` — four-step surface ladder carries all hierarchy; never skip levels
- `{colors.semantic-success}` (#27a644) — the only semantic colour; used for status pills and success indicators
- `{colors.ink}` (#f7f8f8) — all headlines and emphasised body
- `{colors.ink-muted}` (#d0d6e0) — secondary type (meta, subheads on hero panels)
- `{colors.ink-subtle}` (#8a8f98) — tertiary type (deselected states, footer)

**Depth model:** Surface ladder + 1px hairline borders. No drop shadows on dark. No atmospheric gradients.

**Typography rules:**
- Display: `SF Pro Display` / Inter (weight 500–600), aggressive negative letter-spacing scaling from -3.0px at 80px
- Body: same family at weight 400, -0.05px tracking
- Eyebrow labels: 13px, weight 500, +0.4px positive tracking — contrast against negative-tracked display marks section taxonomy
- `{typography.mono}` (JetBrains Mono / Geist Mono) reserved for code contexts and status/ID tokens in product UI — not on marketing chrome

**Shape rules:**
- `{rounded.md}` 8px — all buttons and form inputs
- `{rounded.lg}` 12px — pricing cards, feature cards, profile section panels
- `{rounded.xl}` 16px — product screenshot panels
- `{rounded.pill}` — pricing toggles and status badges only
- `{rounded.full}` — avatar circles only
- Never pill-round CTAs

**Button rules:**
- `button-primary`: `{colors.primary}` background, `{typography.button}` 14px/500, padding 8px 14px, `{rounded.md}`
- `button-secondary`: `{colors.surface-1}` background, 1px `{colors.hairline}` border — secondary CTAs ("Sign in")
- `button-tertiary`: canvas background, for tertiary text actions
- Focus ring: 2px `{colors.primary-focus}` outline at 50% opacity on all focused inputs and buttons

**Responsive breakpoints (from DESIGN.md):**

| Name | Width | Key changes |
|---|---|---|
| Desktop-XL | 1440px | Default desktop layout |
| Desktop | 1280px | Card grid 3-up maintained |
| Tablet | 1024px | Card grid 3-up → 2-up |
| Mobile-Lg | 768px | Nav hamburger; pricing comparison → accordion |
| Mobile | 480px | Single-column; display-xl 80px → ~36px |

Touch targets: CTAs ≥40px tap height; form inputs ≥44px on touch.

---

### 14.3 Key Screens

#### Landing Page (Marketing)

**Purpose:** Convert a first-time visitor to apply for early access.

**Surface:** `{colors.canvas}` base with content sections lifting to `{colors.surface-1}` panels.

**Structure:**
- **Top nav** (`top-nav` component): sticky, height 56px, wordmark left, nav links centre, `button-secondary` ("Sign in") + `button-primary` ("Apply for early access") right
- **Hero section:** `{typography.display-xl}` headline with -3.0px letter-spacing; `{typography.body-lg}` subheadline; single `button-primary` CTA; a high-fidelity product UI screenshot (member dashboard or match notification) in a `{rounded.xl}` `product-screenshot-card` panel
- **Problem section:** eyebrow label (`{typography.eyebrow}`, +0.4px tracking) above a `{typography.display-lg}` headline; specific BNI pain point framing; no generic "Are you tired of..." copy
- **How it works:** three `feature-card` tiles on `{colors.surface-1}` — one per layer (Matching / Community / Referral Education); each card leads with a product UI screenshot or illustration, not an icon
- **Social proof:** `testimonial-card` components (32px padding, `{rounded.lg}`); placeholder copy until real testimonials exist
- **Closing CTA:** `cta-banner` (`{colors.surface-1}`, 48px padding, `{rounded.lg}`); `{typography.headline}` heading; `button-primary`
- **Footer:** `footer` component; dense link grid on `{colors.canvas}`; `{typography.caption}` text in `{colors.ink-subtle}`

**No pricing on landing page at MVP.** No FAQ accordion. No second chromatic accent on the page.

**Copy tone:** See `docs/COPY.md` for the full brief. Summary: lead with outcomes (first customers, proof, referral system), speak to the frustration (selling is hard, networking isn't working, marketing is confusing), be specific rather than abstract. The BNI comparison ("half the cost, none of the mandatory weekly meetings") is a legitimate reference point but not the lead — not all readers will know BNI. The lead is the customer problem: you're good at your work and stuck on getting customers. The platform solves that. Never use: "game-changers", "take your business to the next level", "innovative", or any feature-first framing on the hero.

---

#### Intake Form (MVP — Typeform/Tally; MMP — native)

**Purpose:** Collect matching data while qualifying the applicant.

**MVP implementation note:** Typeform/Tally handle their own styling. Apply the DESIGN.md system to the MMP native form only.

**MMP native form requirements:**
- Dark canvas background (`{colors.canvas}`) — one question per screen, full-bleed layout
- Progress indicator: thin `{colors.primary}` lavender bar at top of screen; percentage or step count in `{colors.ink-subtle}`
- Question text: `{typography.display-md}` or `{typography.headline}` depending on length
- Hint text: `{typography.body}` in `{colors.ink-muted}`, always visible below the question — never behind a tooltip
- `text-input` component: `{colors.surface-1}` background, `{rounded.md}`, focus ring `{colors.primary-focus}`; long-text areas get generous line-height
- Multiple choice options: `feature-card` style tiles (`{colors.surface-1}`, `{rounded.lg}`, 1px `{colors.hairline}`) — selected state lifts to `{colors.surface-2}` with `{colors.hairline-strong}` border
- Offer builder branch intro screen: `{colors.surface-1}` panel with `{rounded.lg}`, human-written copy framing it as helpful rather than a detour
- Example answers: styled as `status-badge`-style callouts in `{colors.surface-2}` with `{typography.body-sm}` in `{colors.ink-muted}` — visually distinct from the question
- Thank you screen: `{typography.display-md}` headline; `{typography.body-lg}` body; no confetti, no animations

---

#### Member Dashboard (MMP)

**Purpose:** Primary logged-in screen. Orients the member to what requires action and what's new.

**Layout:** Left sidebar navigation + main content area. Sidebar on `{colors.surface-1}`, main content on `{colors.canvas}`.

**Sidebar:**
- Platform wordmark top
- Nav items: Dashboard, Spaces, Directory, Profile, Matches
- Active state: `{colors.surface-2}` background on nav item, `{colors.ink}` text; inactive: `{colors.ink-subtle}`
- Bottom: member avatar (`{rounded.full}`) + name + subscription tier badge (`status-badge`)

**Main content — priority order:**

1. **Match status card** (if match pending or awaiting acceptance): `feature-card` on `{colors.surface-1}`, lifted to `{colors.surface-2}` to signal urgency. `{colors.primary}` lavender accent on the action CTA only. This is the most visually prominent element when a match is active — do not bury it below community activity.

2. **Profile completion prompt** (if < 90% matching-critical fields complete): `feature-card` on `{colors.surface-1}` with a progress bar. Specific next step copy, not generic. `{colors.semantic-success}` on completion indicators.

3. **Recent community activity**: chronological post summaries from spaces the member is in. `changelog-row` style — `{colors.canvas}` background, 1px `{colors.hairline}` bottom rule between items.

4. **Upcoming events** (if any): compact event card on `{colors.surface-1}`.

**Design constraint:** If no match is pending, the profile completion prompt is the primary action driver. The dashboard should never feel empty — even at zero community activity, the profile prompt and member directory CTA fill the space meaningfully.

---

#### Profile Editor (MMP)

**Purpose:** Member views and updates their living profile across 85 fields, progressively revealed over time.

**Layout:** Full-width main content with left sidebar section navigation.

**Sidebar section navigation:**
- 13 sections listed (Company, Essential, Business Profile, etc.)
- Each section shows: section name + completion indicator (e.g. "4/6 fields complete")
- Active section: `{colors.surface-2}` background, `{colors.ink}` text
- Incomplete sections with [M] fields: `{colors.primary}` lavender dot indicator — these need attention
- Completed sections: `{colors.semantic-success}` checkmark

**Field display within sections:**
- Section header: `{typography.headline}` + last-updated timestamp in `{typography.caption}` / `{colors.ink-subtle}`
- [M] matching-critical fields: `{colors.primary}` lavender label/badge ("Matching") — consistent across all sections. Required for scoring.
- [E] enrichment fields: `{colors.ink-muted}` label ("Enrichment") — valuable but not gating
- [B] business intelligence fields: `{colors.ink-subtle}` label ("Private") — clearly flagged as optional and member-controlled visibility. Financials and compliance sections include a privacy callout: "Only you can see this section."
- Fields rendered as `text-input` components; long-text fields use a `<textarea>` variant with generous line-height (1.6+)
- Stale field prompt: if a field has a "last updated" timestamp >90 days old, show a `status-badge` in `{colors.surface-2}`: "Updated 4 months ago — still accurate?" with an inline edit trigger
- Inline editing: click field value to enter edit mode; auto-save on blur with a brief `{colors.semantic-success}` flash confirmation; no separate Save button required for individual fields

**Profile completion bar:**
- Global progress bar at top of profile (or in the sidebar header)
- Two sub-indicators: Matching-critical % and Enrichment % — displayed separately, not averaged together
- "100% matching-critical" milestone visually celebrated (not with gamification — with a simple `{colors.semantic-success}` completion state and copy: "Your profile is fully optimised for matching")

---

#### Match Notification (In-App DM)

**Purpose:** Deliver the match with enough context for the member to decide.

**Container:** `feature-card` on `{colors.surface-1}`, `{rounded.lg}`, rendered within the DM thread. The system account sends this — styled distinctly from member messages.

**Card structure:**

1. **Eyebrow:** `{typography.eyebrow}` in `{colors.primary}` — "Your match is ready" — the one place lavender appears in the product as a signal
2. **Match identity:** `{typography.headline}` — matched member's name + business name; `{typography.body}` — one-sentence description; sector `status-badge` + stage `status-badge` in `{colors.surface-2}`
3. **Rationale block:** `{colors.surface-2}` inset panel, `{rounded.md}`, `{typography.body}` in `{colors.ink}` — the operator's written rationale. Attributed: `{typography.caption}` in `{colors.ink-subtle}`: "Reviewed and written by the team — not automated."
4. **Three data points** (in a tight 3-column grid or stacked list): "What they offer your clients" / "What they're looking for" / "Their referral arrangement" — `{typography.body-sm}` labels in `{colors.ink-subtle}`, values in `{colors.ink}`
5. **Actions:** `button-primary` ("Accept this introduction") + `button-secondary` ("Not the right fit")
6. **Decline path:** on "Not the right fit" click, a single optional `text-input` appears: "What's missing? (optional)" — one field, no modal, no form. `button-tertiary` to submit.

**Email version:** Plain text only. Same content structure. No HTML design system applied. Operator's voice must come through without distraction.

---

#### Operator Admin — Match Queue

**Purpose:** Operator's primary working screen. Efficiency is the top requirement — triage 10 members without scrolling.

**Layout:** Split-pane. Left pane: member list. Right pane: candidate detail + rationale editor. Both panes on `{colors.surface-1}` against `{colors.canvas}`.

**Left pane — member list:**
- Each row: `changelog-row` style (1px `{colors.hairline}` bottom rule)
- Per row: member name, sector `status-badge`, ICP tags (truncated if >3), days unmatched (integer, shown as `status-badge` in `{colors.surface-2}` — highlight in `{colors.semantic-success}` inverted for urgency if >5 days), profile completion %
- Sorted by days unmatched descending by default
- Click row → right pane loads that member's candidates

**Right pane — candidate detail:**
- Header: selected member's name + key profile summary (ICP, sector, stage, introductory offer)
- Top 3 candidates listed as `feature-card` tiles (`{colors.surface-1}`, `{rounded.lg}`):
  - Score badge (`{rounded.pill}`, `{colors.surface-2}`): composite score out of 100; ≥80 gets `{colors.semantic-success}` tint
  - Score breakdown: five-row table (signal name / weight / this member's score) in `{typography.body-sm}`
  - Quick-view profile excerpt: ICP, introductory offer, referral arrangement, growth constraint
  - `button-secondary` "View full profile" → opens profile in a drawer (not a new page — keep the match queue context)
  - `button-primary` "Approve" + `button-secondary` "Dismiss"
  - Dismiss → inline `status-badge`-style dropdown: reason picker (short list); confirm with `button-tertiary`

**Rationale editor** (below candidate cards):
- `text-input` textarea variant, pre-populated with system draft
- Label: `{typography.eyebrow}` "Match rationale — edit before sending"
- `{typography.body-sm}` in `{colors.ink-subtle}` hint: "This is sent verbatim to both members. Make it specific."
- Character count indicator (soft limit, not hard block)
- `button-primary` "Preview & Send" → confirmation step showing both notification previews side-by-side before final dispatch

---

#### Community Spaces

**Purpose:** Ongoing engagement layer between matches.

**Layout:** Three-column — left sidebar (spaces nav), main feed, right context panel (member list for this space, upcoming events).

**Spaces sidebar:**
- Space name + unread indicator (dot in `{colors.primary}` when unread posts exist)
- Active space: `{colors.surface-2}` background
- Private match spaces listed separately, below sector/stage spaces, with lock icon

**Feed (main column):**
- `{colors.canvas}` background; posts as `feature-card` tiles (`{colors.surface-1}`, `{rounded.lg}`, 24px padding)
- Post: member avatar (`{rounded.full}`, 32px) + name + timestamp in `{colors.ink-subtle}` + body text
- System posts (match announcements, milestones): `{colors.surface-2}` background, `{colors.primary}` eyebrow label — visually distinct but not disruptive
- Reaction row: 3 reaction types max; `status-badge` style counts; `{rounded.pill}`
- Reply thread: indented, same `feature-card` style at reduced padding; one level only
- Post composer: pinned to bottom of feed column; `text-input` textarea + `button-primary` "Post"

**Private match spaces:** auto-named ("Chris + Sarah — Partnership"). Introduction message pinned at top (`{colors.surface-2}` panel, `{rounded.lg}`). Space otherwise identical to sector spaces.

---

#### Member Directory

**Purpose:** Members browse and discover each other.

**Layout:** Search/filter bar at top; `{colors.canvas}` background; card grid below.

**Search + filter bar:** on `{colors.surface-1}`, 56px height; `text-input` search field left; filter pills (`status-badge` style, `{rounded.pill}`) for Sector, Stage, Geography right.

**Member cards:** `feature-card` component (`{colors.surface-1}`, `{rounded.lg}`, 24px padding), 3-up grid at desktop.
- Avatar (`{rounded.full}`, 40px) + name (`{typography.card-title}`) + business name (`{typography.body-sm}`, `{colors.ink-muted}`)
- Sector `status-badge` + stage `status-badge`
- Introductory offer: `{typography.body-sm}` in `{colors.ink}` — the one line that drives DM requests
- Hover state: card lifts to `{colors.surface-2}`, `{colors.hairline-strong}` border

**Profile view (on click):** full-screen drawer over the directory (not a new page). Read-only version of the profile editor layout. `button-secondary` "Send a message" at top — opens DM composer with context pre-filled.

**No cold messaging from directory:** DM composer pre-fills: "I came across your profile in the directory — [message]". Members cannot initiate a blank DM.

---

### 14.4 Interaction Patterns

**Progressive disclosure:** Members never see all 85 fields simultaneously. Section tabs with completion indicators guide exploration. New members see only [M] fields on Day 0 — the other sections exist in the sidebar but are marked "Complete after your first match".

**Contextual prompts:** Profile completion prompts appear within the profile editor, triggered by days since last update or [M] completion below threshold. Never interruptive modals. `status-badge` style inline prompts within the field itself.

**No dead ends:** The offer builder branch and any multi-step flow always has a "Save and come back" path that commits partial progress. No data loss on accidental navigation.

**Confirmation patterns:** Single confirmation step for destructive or irreversible actions (decline a match, cancel subscription). `{colors.surface-2}` inline confirmation, not a modal. Clear consequence copy. No double-confirmation dialogs for routine actions.

**Empty states:** Every feed, list, and queue has a designed empty state using `feature-card` components — not just "No items". Match queue empty: "All members are matched. Check back as new members join." Dashboard with no match pending: show profile completion prompt as the primary action.

**Loading states:** Skeleton screens using `{colors.surface-2}` placeholder blocks for all list and card views. Do not block the UI during match scoring or profile save operations. Brief `{colors.semantic-success}` flash confirmation on successful save — no toast notifications.

**Drawer pattern over new pages:** Profile views, full candidate profiles in the match queue, and DM composers open in drawers that preserve the underlying page context. Drawers use `{colors.surface-1}` background sliding over `{colors.canvas}`, `{colors.hairline}` left border.

---

### 14.5 Accessibility

- WCAG AA compliance as the baseline
- All form fields: visible labels using `{typography.body-sm}` above the input — never rely on placeholder text alone
- Colour is never the sole indicator of status — every `{colors.primary}` lavender indicator is paired with a text label or icon
- Focus states: 2px `{colors.primary-focus}` outline at 50% opacity on all interactive elements — do not suppress default focus rings
- All match and community actions keyboard-navigable (Tab, Enter, Escape for drawers)
- Avatar images: descriptive alt text. System posts: `role="status"` for screen readers.
- Dark canvas: ensure all `{colors.ink}` on `{colors.canvas}` pairings meet 4.5:1 contrast ratio; `{colors.ink-muted}` on `{colors.surface-1}` should be checked at implementation

---

### 14.6 Responsive Behaviour

Follows DESIGN.md breakpoints exactly:

| Breakpoint | Width | Key changes |
|---|---|---|
| Desktop-XL | 1440px | Default; split-pane admin, three-column community |
| Desktop | 1280px | Primary target for all logged-in views |
| Tablet | 1024px | Card grids 3-up → 2-up; community right panel collapses |
| Mobile-Lg | 768px | Nav → hamburger; split-pane admin → single column; pricing → accordion |
| Mobile | 480px | Single-column throughout; display type scales toward display-md |

**Admin dashboard and profile editor:** not fully optimised for mobile at MMP. Show an inline `feature-card` prompt at <768px: "For the best experience, use on a desktop or laptop." Core read flows (DMs, feed, profile view) must work on mobile.

**Product screenshot panels** (`{rounded.xl}`): maintain aspect ratio, never crop. Scale down proportionally.

---

### 14.7 Design Handoff Notes

DESIGN.md is the single source of truth for tokens, components, and rules. Do not introduce colours, type sizes, or component variants not defined there without updating DESIGN.md first.

**Priority 1 — wireframe and prototype before implementation:**

1. **Signup → intake form → thank you** — first impression and conversion event; the offer builder branch needs particular care
2. **Match notification → accept/decline** — the core product moment; the rationale block and action hierarchy must be right
3. **Profile editor — Day 0 (matching-critical fields only)** — high-stakes UX; friction here directly degrades match quality
4. **Operator match queue — split pane → rationale edit → preview → send** — operator efficiency depends on this flow being fast

**Priority 2:**
5. Member dashboard (match status card prominence)
6. Community feed and spaces
7. Member directory + member card grid
8. Operator analytics dashboard
9. Settings, subscription management, notification preferences

**Component implementation order:** Follow the surface ladder — implement canvas and surface-1 base first, then build cards on top, then interactive states. Don't build components out of surface-ladder order.

---

## 15. Success Criteria

### MVP

| Signal | Target |
|---|---|
| Founders completing intake | 20+ |
| Intake completion rate | >60% |
| Match acceptance rate | >70% |
| Introduction taken (both respond) | >50% |
| Qualitative "this is useful" signal | 3+ unprompted |

### MMP

| Signal | Target |
|---|---|
| Paying members | 50+ |
| MRR | £2,000+ |
| Intake → paid conversion | >50% |
| Match acceptance rate | >65% |
| 90-day retention | >70% |
| Operator time per member | <30 min/month |
| Profile completion (matching-critical) | >90% |
| Profile completion (enrichment) | >50% |

---

## 16. Out of Scope

The following are explicitly deferred and not to be designed or built until the stated trigger condition is met:

| Feature | Trigger condition |
|---|---|
| Fully automated matching (no operator review) | Algorithm tuned on ≥200 accepted matches |
| Referral outcome tracking | Trust layer established; member reporting mechanism built |
| Commission processing between members | Out of scope permanently at product level |
| White-label / B2B community licensing | Direct-to-founder MRR exceeds £5k/month AND inbound licensing enquiry received |
| Mobile app | Responsive web validated; mobile usage data shows demand |
| Free tier / freemium | Paying member base >100; acquisition strategy review |
| AI-generated rationale (unreviewed) | Operator review removed only when algorithm quality is independently validated |
| Video hosting | External links sufficient until video engagement data justifies it |
| Course / curriculum builder | Not this product |
| Typesense / Algolia search upgrade | Member count approaches ~500 |

---

## 17. Open Questions

| Question | Status | Notes |
|---|---|---|
| No-code stack selection (Framer vs Carrd, Typeform vs Tally) | Deferred | MVP-stage decision; either works |
| Early adopter community identification | Not started | Where to find the first 20 MVP members |
| Profile completion incentive copy | Needs validation | "2x more match requests" framing proposed; validate against real matching data before using |
| [M] field update → re-scoring latency | Deferred to engineering | Real-time (on save) vs batched (nightly). Real-time is better UX; nightly is simpler. |
| Private shared space: DM thread vs named space | Lean toward named space | "Chris + Sarah — Partnership" is more intentional; confirm at implementation |
| Airtable field map: Decline reason + Decline count | Needs updating | Add `Decline reason` (text) and `Decline count` (number) to the Airtable spec in 06-intake-questionnaire.md |
| Offer builder: embedded vs async email follow-up | Open | Embedded (current design) vs follow-up email template; embedded is higher friction in the form but lower drop-off risk |
| Name/email collection timing | Recommended: landing page | Allows drop-off tracking before form starts |
