# Diagnostic Scorecard & Interview Framework

## The Diagnostic Scorecard

Rate each layer 1-5 based on health signals and warning signs.

| Layer | Health Signals (→5) | Warning Signs (→1) | Score |
|-------|--------------------|--------------------|-------|
| **Customers** | Can identify 100+ prospects by name; have budget; bought similar solutions | Struggle to find prospects; no budget; never bought software | ___ |
| **Problem** | Customers describe problem unprompted; top-5 priority; spending on alternatives | Only mention when prompted; low priority; free workarounds | ___ |
| **Solution** | Customers say "10x better"; "very disappointed" without it; recommend to others | "Nice to have"; wouldn't miss it; don't recommend | ___ |
| **Technology** | Reliable, fast, scalable; team can maintain; enables solution effectively | Buggy, slow, doesn't scale; team struggles; constrains solution | ___ |
| **Growth** | Positive CAC:LTV; scalable channels; healthy retention metrics | CAC > LTV; no scalable channels; high churn | ___ |

**Scoring Guide:**
- **5:** Strong evidence of health
- **4:** Mostly healthy with minor concerns
- **3:** Mixed signals, unclear
- **2:** Significant concerns
- **1:** Clearly broken

**Interpretation:**
- Lowest-scoring layer is the biggest problem
- Fix from the bottom up — broken foundation makes higher layers irrelevant
- If multiple layers score low, focus on the lowest one first

---

## Diagnostic Questions by Symptom

### "We can't get users to sign up"

Ask in order, starting from the bottom:

1. **Customer Layer Check:** Are we reaching people who actually buy solutions like ours?
   - Do they have budget authority?
   - Have they bought similar products before?
   - Are we reaching decision-makers or users without buying power?

2. **Problem Layer Check:** Is the problem urgent enough to drive action?
   - When we describe the problem, do prospects lean in or tune out?
   - Are they actively searching for solutions?
   - Would they be willing to pay for a solution?

3. **Solution Layer Check:** Does our solution resonate?
   - Do prospects understand our value proposition quickly?
   - Do they see us as meaningfully better than alternatives?
   - Is there friction in signup or trial process?

4. **Growth Layer Check:** Are we reaching prospects effectively?
   - In channels where customers spend time?
   - Messaging aligned with how customers describe the problem?
   - Targeting accurate?

### "Users sign up but don't engage"

1. **Problem Layer Check:** Did we attract them with the right problem?
   - Marketing promise match product reality?
   - Problem actually urgent for them?
   - Right customers, or attracted wrong segment?

2. **Solution Layer Check:** Does product deliver on the promise?
   - Can users get to value quickly (time-to-value)?
   - Product intuitive or confusing?
   - Does using it actually solve the problem?

3. **Technology Layer Check:** Technical issues blocking engagement?
   - Product reliable and fast?
   - Bugs or friction points?
   - Works across devices/contexts?

### "We're growing but not making money"

1. **Customer Layer Check:** Targeting customers who can pay?
   - Segment willing and able to pay our price?
   - Attracting freeloaders who'll never convert?
   - Budget for this type of solution?

2. **Problem Layer Check:** Problem valuable enough?
   - How much is it costing customers?
   - Willing to pay or only use free alternatives?
   - "Nice to have" vs. "must have"?

3. **Solution Layer Check:** Solution justify the price?
   - Value clearly worth what we charge?
   - Customers getting enough value to retain?
   - Free alternatives "good enough"?

### "We can't retain users"

1. **Problem Layer Check:** Is this a recurring problem?
   - One-time event or ongoing need?
   - Need us continuously or occasionally?
   - Solved the problem so well they don't need us anymore?

2. **Solution Layer Check:** Ongoing value?
   - Value after initial use?
   - Helping achieve goals repeatedly?
   - Product gets better with use or stale?

3. **Technology Layer Check:** Product quality driving churn?
   - Bugs or performance issues?
   - Reliably works when needed?
   - Shipping improvements or stagnating?

4. **Growth Layer Check:** Attracted wrong users?
   - Churning users ideal customers or wrong segment?
   - Marketing promises misaligned with reality?
   - Measuring the right cohorts?

---

## The Diagnostic Interview Framework

### Who to Interview (The 20-Interview Rule)

Complete at least 20 diagnostic interviews before concluding which layer is broken:

- **5 churned customers:** Why did they leave?
- **5 never-activated users:** What happened?
- **5 active power users:** Why do they stay? What almost made them leave?
- **5 prospects** (including some who chose competitors or nothing): Why?

### Core Questions by Layer

**Customer Layer Questions:**
- "Tell me about your role and your company."
- "How do you typically discover and evaluate new tools?"
- "Who else is involved in buying decisions like this?"
- "What's your typical budget for tools like this?"

**Problem Layer Questions:**
- "Walk me through the last time you experienced [problem]."
- "How often does this problem come up?"
- "What does it cost you when this problem occurs?"
- "What have you tried before to solve this problem?"
- "How important is solving this relative to other priorities?"

**Solution Layer Questions:**
- "When you first saw our product, what did you expect it to do?"
- "Did it meet that expectation? Where did it fall short?"
- "What would make this product indispensable to you?"
- "Compared to alternatives, what do we do better? Worse?"
- "If our product disappeared tomorrow, how would you feel?"

**Technology/Execution Questions:**
- "Did you encounter any frustrations using the product?"
- "Were there times when the product didn't work as expected?"
- "How would you describe the product's reliability and speed?"

**Growth/Discovery Questions:**
- "How did you first hear about us?"
- "What made you decide to try us?"
- "What almost stopped you from signing up?"

### The "Five Whys" Technique

For any issue, ask "why" five times to find the root cause:

1. "Users aren't engaging with our product."
2. Why? → They don't complete onboarding.
3. Why? → Onboarding asks for too much information.
4. Why? → We need info to personalize the experience.
5. Why? → We assumed personalization was required for value.
6. Why? → Never tested if users could get value without it.

**Root cause:** Solution layer — assumption about personalization creates friction.

### What to Look For in Patterns

- **Repeatability:** Do you hear the same issues repeatedly?
- **Emotional Intensity:** When people mention problems, how emotional are they?
- **Specificity:** Can people describe the problem in detail, or is it vague?
- **Root Cause:** When you ask "why" repeatedly, where do you end up?

After 20 interviews, confidently identify one or two layers as the primary issues.

---

## Misdiagnosis Case Studies

### Thought It Was Growth, Was Actually Customer

**Symptom:** "CAC is too high"
**Initial diagnosis:** Growth layer — optimize channels and messaging
**What they tried:** New landing pages, different ads, hired growth marketer, tested channels
**Result:** CAC improved marginally, acquisition still slow
**Actual diagnosis:** Customer layer — targeting startups without budget for premium tools
**Example:** Superhuman focused on high-volume email power users (execs, VCs) who valued speed. Intercom found SaaS companies with communication budgets.
**Fix:** Change target customer to segment with budget and urgency

### Thought It Was Solution, Was Actually Problem

**Symptom:** "Users sign up but don't engage"
**Initial diagnosis:** Solution layer — simplify onboarding
**What they tried:** Redesigned onboarding 3x, added tooltips, video tutorials
**Result:** Modest activation improvement, still low engagement
**Actual diagnosis:** Problem layer — not urgent enough to drive action
**Example:** Loom pivoted from usability testing (Opentest) to "explain something asynchronously right now" (must-have). Calendly succeeded because scheduling back-and-forth was *immediately* painful.
**Fix:** Reframe from "nice-to-have" to "must-have" with immediate urgency

### Thought It Was Technology, Was Actually Solution

**Symptom:** "Product is slow and unreliable"
**Initial diagnosis:** Technology layer — improve performance
**What they tried:** Rewrote infrastructure, added caching, invested in DevOps
**Result:** Faster product, fewer complaints, but growth didn't improve
**Actual diagnosis:** Solution layer — customers couldn't get value without heavy configuration
**Example:** Segment's breakthrough was open-sourcing analytics.js — one script routing data to many services — which went viral. Zapier made API connections instant and config-free.
**Fix:** Make solution more turnkey — pre-built templates, integrations, default configs
