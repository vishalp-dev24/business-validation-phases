# MVP Decision Matrix - Phase 3: Solution Validation

## MVP Type Selection Guide

### Decision Tree

```
Is the backend complex/expensive to build?
├── YES → Can humans do the work behind the scenes?
│   ├── YES → Wizard of Oz MVP
│   └── NO → Mechanical Turk MVP (hybrid)
└── NO → Can you manually deliver the value?
    ├── YES → Concierge MVP
    └── NO → Pinocchio (fake product) + smoke test
```

### MVP Type Descriptions

| Type | Best For | Examples | Effort |
|------|----------|----------|--------|
| **Concierge** | High-touch service, complex personalization | Wealthfront (manual portfolios), Food on Table (manual meal plans) | Medium |
| **Wizard of Oz** | Seems automated but isn't | Zappos (store photos), Aardvark (humans as AI) | High |
| **Mechanical Turk** | AI/software simulated by humans | Cardmunch (humans transcribing), IBM Speech-to-Text | Medium |
| **Pinocchio** | Non-functional prototype | Dropbox video, hardware mockups | Low |
| **Smoke Test** | Landing page validation | Buffer pricing test, Pebble Kickstarter | Low |

---

## Concierge MVP Checklist

### Setup

- [ ] Core value proposition defined
- [ ] Manual service process mapped
- [ ] Customer onboarding flow created
- [ ] Service delivery timeline established
- [ ] Pricing structure determined
- [ ] 5-10 target customers identified

### Execution

- [ ] Personal outreach to first customers
- [ ] Manual delivery of service (30-60 min per customer)
- [ ] Daily observation notes taken
- [ ] Customer feedback collected after each interaction
- [ ] Process iterations documented

### Metrics to Track

| Metric | Target | Actual |
|--------|--------|--------|
| Customers served | 10 | |
| Satisfaction score | >8/10 | |
| Willingness to continue | >70% | |
| Referrals generated | >2 | |
| Time per customer | <60 min | |
| Revenue collected | >$X | |

### Lessons Learned Template

**What worked:**
- 
- 

**What didn't work:**
- 
- 

**Customer surprises:**
- 
- 

**Features customers actually want:**
- 
- 

**Automation candidates:**
- 
- 

---

## Wizard of Oz MVP Checklist

### Setup

- [ ] Customer-facing interface built (minimal UI)
- [ ] Backend "wizard" system designed
- [ ] Human operators trained
- [ ] Response time SLAs established
- [ ] Customer communication templates ready
- [ ] Scaling limits defined (max customers)

### Execution

- [ ] Interface launched to limited users
- [ ] Wizards responding to all requests
- [ ] Response time tracked (<X minutes)
- [ ] Quality assurance performed
- [ ] Customer satisfaction monitored
- [ ] Technical requirements documented

### Wizard Operations Log

| Date | Customer | Request | Response Time | Outcome | Notes |
|------|----------|---------|---------------|---------|-------|
| | | | | | |

### Automation Roadmap

After 50 wizard interactions, identify automation opportunities:

| Task | Frequency | Automation Difficulty | Priority |
|------|-----------|----------------------|----------|
| | | | |

---

## Design Sprint - 5 Day Plan

### Day 1: Understand & Define

**Morning - Understand:**
- [ ] Map the problem space
- [ ] Review customer interviews
- [ ] Identify key insights
- [ ] Choose target for sprint

**Afternoon - Define:**
- [ ] Define long-term goal
- [ ] List sprint questions
- [ ] Make a map (user journey)
- [ ] Pick a target (one moment to prototype)

**Deliverable:** Sprint target defined

### Day 2: Sketch

**Morning - Lightning Demos:**
- [ ] Review 3-5 competing solutions
- [ ] Capture good ideas
- [ ] Note what to avoid

**Afternoon - Solution Sketching:**
- [ ] Each person sketches 3+ ideas
- [ ] Crazy 8s exercise (8 ideas in 8 minutes)
- [ ] Final solution sketch (detailed)

**Deliverable:** Solution sketches on wall

### Day 3: Decide

**Morning - Choose:**
- [ ] Review all sketches silently
- [ ] Heat map voting (dots on best ideas)
- [ ] Speed critique (3 min per sketch)
- [ ] Straw poll voting
- [ ] Supervote (decider chooses)

**Afternoon - Storyboard:**
- [ ] Create 10-15 step storyboard
- [ ] Draw prototype scenes
- [ ] Write script for user testing

**Deliverable:** Storyboard complete

### Day 4: Prototype

**All Day - Build:**
- [ ] Assign prototype roles
- [ ] Build realistic facade
- [ ] Create fake data/content
- [ ] Stitch screens together
- [ ] Dry run full test

**Deliverable:** Working prototype (looks real, partially functional)

### Day 5: Test

**All Day - User Tests:**
- [ ] Test with 5 users
- [ ] Record all sessions
- [ ] Take notes using scorecard
- [ ] Debrief as team

**Deliverable:** Test results, validated/invalidated hypotheses

### Sprint Outcome

| Hypothesis | Tested | Result | Next Step |
|------------|--------|--------|-----------|
| | | Validated / Invalidated / Inconclusive | |

---

## Pricing Validation Test

### Price Testing Strategy

Option A: **_$/month** (Low)
Option B: **$_/month** (Medium)  
Option C: **$_/month** (High)

### Test Setup

- [ ] Landing page with pricing table
- [ ] A/B/C traffic split (33% each)
- [ ] Conversion tracking on "Select Plan"
- [ ] 100+ visitors per variant

### Results Matrix

| Variant | Price | Visitors | Clicks | Conv. Rate | Revenue Potential |
|---------|-------|----------|--------|------------|-------------------|
| A | $ | | | | |
| B | $$ | | | | |
| C | $$$ | | | | |

### Willingness to Pay Survey

**Van Westendorp Price Sensitivity Meter:**

Ask customers:
1. At what price would it be so low you'd question quality? $_____
2. At what price is it a bargain? $_____
3. At what price does it start getting expensive? $_____
4. At what price is it too expensive? $_____

**Optimal Price Range:** $_____ - $_____

---

## NPS Survey Template

### Survey Questions

**Question 1:** How likely are you to recommend [product] to a friend or colleague?
- 0-6: Detractor
- 7-8: Passive  
- 9-10: Promoter

**Question 2:** What's the primary reason for your score?
[Open text]

**Question 3:** If you could change one thing, what would it be?
[Open text]

**Question 4:** How disappointed would you be if you could no longer use [product]?
- Very disappointed
- Somewhat disappointed
- Not disappointed
- Don't use it anymore

### Results

| Metric | Score |
|--------|-------|
| NPS (Promoters - Detractors) | |
| Promoter % | |
| Passive % | |
| Detractor % | |
| Very disappointed % | |

---

## Phase 3 Go/No-Go Decision

### Validation Results

**Metrics Summary:**
- Customers served: _____
- NPS score: _____
- Willingness to pay (%) : _____
- Retention (Day 7): _____
- Retention (Day 30): _____

### Success Criteria

- [ ] 40%+ willing to pay/pre-order
- [ ] NPS > 40
- [ ] 30%+ Day 7 retention
- [ ] Validated feature set identified
- [ ] Pricing validated

### Pivot or Persevere?

**Persevere if:**
- [ ] Core value proposition resonates
- [ ] Customers paying/using consistently
- [ ] Clear path to automation
- [ ] Positive word-of-mouth emerging

**Pivot if:**
- [ ] Value proposition unclear to customers
- [ ] Low engagement/willingness to pay
- [ ] Wrong customer segment
- [ ] Solution too complex to deliver

### Decision
**VERDICT:** GO / NO-GO / PIVOT

**Confidence:** _____%

**If GO:**
- Validated features: _____
- Target price: $_____
- Next phase: Product-Market Fit validation
- Build target: _____

**If PIVOT:**
- Pivot type: _____
- New hypothesis: _____

---

*Template version 1.0*
*Based on Lean Startup (Ries) + Design Thinking (d.school)*