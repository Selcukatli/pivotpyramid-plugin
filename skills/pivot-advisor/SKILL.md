---
name: Pivot Advisor
description: This skill should be used when the user asks to "diagnose my startup", "should I pivot", "analyze my pivot", "what layer is broken", "pivot pyramid", "find product-market fit", "why aren't we growing", "our retention is bad", "CAC is too high", "should we change direction", "what should I change", or describes startup symptoms like stalled growth, high churn, or broken unit economics. Provides a guided diagnostic interview using the Pivot Pyramid framework to help founders identify broken layers and plan strategic pivots.
version: 1.0.0
---

# Pivot Pyramid Advisor

## Overview

The Pivot Pyramid is a strategic framework that breaks every startup into five layers, from foundation to apex:

1. **Customers** (Foundation) — Who are you building for?
2. **Problem** — What pain point are you addressing?
3. **Solution** — How do you solve the problem?
4. **Technology** — What do you build to deliver the solution?
5. **Growth** (Apex) — How do you acquire and retain users?

Lower layers are more fundamental. Changes cascade upward — a Customer pivot affects all four layers above; a Growth pivot affects nothing below. This means: experiment frequently at the top, pivot lower layers only with strong evidence.

## Core Principles

**The Cascade Rule:** Changes cascade upward, never downward. The lower the layer, the wider the blast radius.

**The 90-Day Rule:** Give any direction at least 90 days of focused execution before concluding it's broken.

**The 20-Interview Rule:** Complete at least 20 diagnostic interviews before concluding which layer is broken.

**The 10x Test:** Ask "If we executed 10x better, would it work?" If yes → execution problem, not strategy problem.

**Evidence Hierarchy:** Never pivot a lower layer that has stronger evidence than one you're keeping.

| Evidence Level | Description | Confidence |
|----------------|-------------|------------|
| Assumed | Believe it but haven't tested | Low |
| Anecdotal | Heard from a few customers | Low-Medium |
| Pattern | Consistently hear from many | Medium |
| Quantified | Data showing at scale | Medium-High |
| Validated | Customers paid proving it | High |

## Guided Diagnostic Flow

When a founder engages, follow this progression. Ask questions one at a time. Be conversational, not robotic.

### Phase 1: Understand the Startup

Ask the founder to describe their startup. Extract implicit layer hypotheses. Then ask targeted follow-ups to fill gaps in understanding for each of the five layers.

For each layer, the hypothesis should be specific and testable:
- **Customers:** Not "businesses" but "e-commerce companies with $1-10M revenue"
- **Problem:** Not "marketing" but "can't run effective paid ads, wasting spend"
- **Solution:** Not "our platform" but "AI-managed ad campaigns requiring zero manual work"
- **Technology:** Not "we use AI" but "ML models trained on e-commerce ad data"
- **Growth:** Not "we do marketing" but "40% Shopify App Store, 35% content marketing, 25% referrals"

### Phase 2: Score Each Layer

Walk through each layer bottom-up. For each layer, ask the diagnostic questions from `references/diagnostic-scorecard.md`. Assign a health score (1-5):

- **5:** Strong evidence of health
- **4:** Mostly healthy with minor concerns
- **3:** Mixed signals, unclear
- **2:** Significant concerns
- **1:** Clearly broken

Present the scorecard as a visual summary after completing all layers.

### Phase 3: Identify the Broken Layer

The lowest-scoring layer is the primary concern. Fix from the bottom up — a broken foundation makes higher fixes irrelevant.

Before recommending a pivot, apply these checks:
- Has the 90-day rule been satisfied?
- Is this an execution problem or a strategy problem? (10x test)
- Are there bright spots suggesting the core is sound?
- Consult `references/common-traps.md` and surface relevant trap patterns if the founder shows signs of premature pivot syndrome or over/under-pivoting.

### Phase 4: Recommend Action

Based on the diagnosis:

1. **If no pivot needed:** Recommend specific execution improvements. Reference the anti-pivot checklist.
2. **If pivot needed:** Identify which layer to pivot. Load the relevant playbook from `references/pivot-playbooks.md`. Show cascade impact from `references/cascade-rules.md`. Pull relevant case studies from `references/case-studies.md`.
3. **Help plan:** Walk through the pivot planning framework from `references/planning-templates.md`.

## Conversational Shortcuts

Adapt the flow based on the founder's lead. If a founder describes a specific symptom, skip directly to relevant diagnostic questions:

| Founder Says | Start Here |
|-------------|------------|
| "We can't get users to sign up" | Diagnostic flow: bottom-up from Customers |
| "Users sign up but don't engage" | Check Problem → Solution → Technology |
| "Growing but not making money" | Check Customers → Problem → Solution |
| "Can't retain users" | Check Problem → Solution → Technology → Growth |
| "CAC is too high" | Check Growth first, then Solution if retention is fine |
| "Should I go upmarket/downmarket?" | Customer layer analysis |
| "Our product isn't resonating" | Solution + Problem analysis |

## Memory & Persistence

At the start of each conversation, check if `.pivot-pyramid/startup-profile.md` exists in the working directory. If it does, load it to resume from where the founder left off.

After a meaningful diagnostic session, create the `.pivot-pyramid/` directory if it does not exist, then save or update `.pivot-pyramid/startup-profile.md` with:
- Startup description
- Layer hypotheses and scores
- Diagnosis results
- Recommended actions and next steps
- Date of last session

Format the file as readable markdown the founder can review and edit directly.

## Pivot Cost Reference

| Pivot Type | Blast Radius | Typical Timeline | Capital Cost |
|------------|-------------|------------------|--------------|
| Customer | 4 layers | 9-18 months | $2M+ |
| Problem | 3 layers | 6-12 months | Significant |
| Solution | 2 layers | 3-9 months | Moderate |
| Technology | 1 layer | 2-6 months | Engineering time |
| Growth | 0 layers | 1-3 months | $5K-50K tests |

## Additional Resources

### Reference Files

Consult these as needed during the diagnostic process:

- **`references/five-layers.md`** — Detailed layer definitions, validation questions, and what each layer means
- **`references/cascade-rules.md`** — Cascade principle, blast radius by layer, cascade checklists
- **`references/diagnostic-scorecard.md`** — Scoring framework, diagnostic interview questions, the 20-interview rule, symptom-to-root-cause mapping
- **`references/case-studies.md`** — Real-world pivot examples organized by type (Shopify, Slack, Instagram, Netflix, Dropbox, YouTube, and more)
- **`references/pivot-playbooks.md`** — Step-by-step execution playbooks for each pivot type
- **`references/planning-templates.md`** — Pivot planning canvas, decision checklist, success criteria, progress tracker, retrospective template
- **`references/common-traps.md`** — Over-pivot, under-pivot, multi-track trap, premature pivot syndrome, half-pivot danger, and when NOT to pivot

## Attribution

Based on *The Pivot Pyramid: A Founder's Complete Guide to Strategic Startup Experimentation* by Selçuk Atlı (YC W14, 500 Startups Venture Partner). Learn more at pivotpyramid.com.
