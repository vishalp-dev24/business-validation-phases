# Business Validation Phases

A comprehensive, phase-based framework for validating business ideas from concept to scale. Integrates Y Combinator, Lean Startup, Jobs-to-be-Done, and top VC methodologies into actionable validation workflows.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Framework](https://img.shields.io/badge/Framework-Multi--Phase-blue)](./SKILL.md)
[![Context](https://img.shields.io/badge/Engineering-Context--Engineered-green)](./templates/context-engineering-prompts.md)

---

## What This Is

I keep seeing founders spend months building products nobody ends up wanting. This framework exists to stop that. It gives you structured checklists and actual decision criteria for every stage of your startup journey.

Here's the thing about validation: it should hurt a little. If you're not discovering uncomfortable truths about your idea, you're measuring vanity metrics.

---

## Framework by Phase

| Phase | What You Are Doing | Framework to Use | Go Threshold |
|-------|-------------------|------------------|--------------|
| **1 - Idea/Concept** | Testing interest before you build anything | Pretotyping + Effectuation | >10% ILI |
| **2 - Problem** | Confirming the problem actually exists and hurts | Customer Development + JTBD | 60%+ urgency |
| **3 - Solution** | Testing solutions without building them | Concierge/Wizard of Oz MVP | 40%+ willing to pay |
| **4 - PMF** | Measuring product-market fit properly | Sean Ellis 40% Test | 40%+ "very disappointed" |
| **5 - Scale** | Validating unit economics work | Bessemer's 10 Laws | LTV/CAC > 3 |
| **6 - Expansion** | Building moats that last | NFX Network Effects | NRR > 100% |

---

## Quick Start

### For Founders

1. Figure out which phase you are actually in (be honest)
2. Open the matching template in `/templates`
3. Work through the checklist - actually do the work, do not skip steps
4. Make the Go/No-Go decision with real evidence

### For AI Tools

If you are using Codex, Hermes, Claude Code, or similar, grab the context engineering prompts in [`templates/context-engineering-prompts.md`](./templates/context-engineering-prompts.md):

- **Chain-of-Thought (CoT)** - For methodical step-by-step validation
- **Tree-of-Thoughts (ToT)** - When you want multiple perspectives
- **ReAct** - For research-heavy dynamic validation

---

## What Is Inside

```
business-validation-phases/
├── SKILL.md                              # The full framework
├── README.md                             # This file
└── templates/
    ├── pretotyping-checklist.md          # Phase 1
    ├── customer-discovery-guide.md       # Phase 2
    ├── mvp-decision-matrix.md            # Phase 3
    ├── pmf-measurement.md                # Phase 4
    ├── scale-validation.md               # Phase 5
    ├── expansion-network-effects.md      # Phase 6
    └── context-engineering-prompts.md    # AI tooling
```

---

## Where This Comes From

I did not invent these frameworks. I assembled them from people who have actually done this stuff:

### Traditional/Academic
- **Lean Startup** (Eric Ries) - Build-Measure-Learn loops
- **Customer Development** (Steve Blank) - 4-step validation
- **Jobs-to-be-Done** (Clay Christensen) - The "hiring products" frame
- **Design Thinking** (Stanford d.school) - Human-centered design
- **Effectuation** (Saras Sarasvathy) - Expert entrepreneur logic

### VC/Accelerator
- **YC** - "Make Something People Want" (simple but hard)
- **Sequoia Capital** - 4 Terrifying Questions
- **First Round Capital** - 4-level PMF framework
- **Bessemer 10 Laws** - Cloud metrics that actually matter
- **a16z** - 13 metrics for marketplaces
- **NFX** - 16 types of network effects

### Validation Methods
- **Pretotyping** (Alberto Savoia) - Fake doors, videos, ILI
- **MVP Types** - Concierge, Wizard of Oz, Mechanical Turk
- **Sean Ellis Test** - The 40% rule
- **AARRR** (Dave McClure) - Pirate metrics

---

## Principles That Matter

1. **Kill ideas fast.** If validation fails, move on. Do not get attached.
2. **Demand evidence.** "Interesting" is not evidence. Concrete stories are.
3. **Founder-problem fit.** You need authentic insight into the pain.
4. **Niche aggressively.** The narrow wedge beats the broad market.
5. **Think 10 years.** Will you still care? Will it still matter?

---

## Usage Examples

### Phase 2: Problem Validation

From `templates/customer-discovery-guide.md`:

```markdown
# Customer Interview Script

## Question 1: Tell me about the last time you [experienced problem]
- Look for: Concrete stories, not opinions
- Red flag: "That sounds interesting" - polite, not urgent
- Green flag: "This happens all the time"

## Question 2: What do you currently do to solve this?
- Look for: Manual workarounds, spreadsheets, paid solutions
- Red flag: "Nothing really"
- Green flag: They spend money or time working around it

Minimum: 40 problem interviews
Target: 60%+ confirm urgent problem
```

### Phase 4: PMF Measurement

From `templates/pmf-measurement.md`:

```markdown
# Sean Ellis 40% Test

Ask: "How would you feel if you could no longer use [product]?"

- Very disappointed: ___% (Target: >40%)
- Somewhat disappointed: ___%
- Not disappointed: ___%

Follow-up: "What is the main reason?"
- Capture themes: Saves time / Better than X / Essential for workflow
```

### Phase 5: Unit Economics

From `templates/scale-validation.md`:

```markdown
# CAC Payback

LTV = (ARPU × Gross Margin) / Churn
CAC = Sales & Marketing Spend / New Customers

- LTV: $_____
- CAC: $_____
- LTV/CAC ratio: _____ (Target: >3)
- Payback period: _____ months (Target: <12)
```

---

## How to Use This

### First-Time Founder

Start with Phase 1. Read `templates/pretotyping-checklist.md`. Do the Bird-in-Hand worksheet. Run a Fake Door test this week (seriously, 48 hours). Move to Phase 2 if you get >10% ILI.

### Experienced Founder

Skip to wherever you are right now. Fill in the template gaps honestly. Identify your strongest Go signals and your weakest validation area. Fix the weak spot.

### AI-Assisted Validation

Read `templates/context-engineering-prompts.md`. Use CoT for deep dives on single ideas. Use ToT when you want panel-style evaluation. Use ReAct for research-heavy validation.

---

## Related Reading

- [Y Combinator Startup Library](https://www.ycombinator.com/library)
- [The Lean Startup](https://theleanstartup.com/) by Eric Ries
- [The Mom Test](http://momtestbook.com/) by Rob Fitzpatrick - read this if you read nothing else
- [NFX Network Effects Bible](https://www.nfx.com/post/network-effects-bible/)
- [First Round Review](https://review.firstround.com/)

---

## Contributing

This pulls together 25+ years of startup research. If you have:
- Real validation case studies with results
- Framework improvements
- Phase-specific tools
- Better context engineering patterns

Open an issue or PR. Back it with evidence.

---

## License

MIT License - see [LICENSE](./LICENSE).

---

## Acknowledgments

Frameworks from:
- Eric Ries, Steve Blank, Clayton Christensen, Saras Sarasvathy
- Sequoia Capital, First Round Capital, Bessemer, a16z, NFX

---

<p align="center">
  <b>Validate before building. Build what people want.</b>
</p>

<p align="center">
  Star this repo if it helps your startup journey
</p>
