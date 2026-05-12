# Business Validation Phases

A comprehensive, phase-based framework for validating business ideas from concept to scale. Integrates Y Combinator, Lean Startup, Jobs-to-be-Done, and top VC methodologies into actionable validation workflows.

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Framework](https://img.shields.io/badge/Framework-Multi--Phase-blue)](./SKILL.md)
[![Context](https://img.shields.io/badge/Engineering-Context--Engineered-green)](./templates/context-engineering-prompts.md)

---

## 🎯 What This Is

This framework helps you **avoid building things nobody wants** by providing structured validation checklists and decision criteria for every stage of your startup journey.

> *"Validation must be uncomfortable. If your tests aren't revealing hard truths, you're measuring vanity metrics."*

---

## 📊 Framework by Phase

| Phase | Focus | Primary Framework | Go Threshold |
|-------|-------|-------------------|--------------|
| **1 - Idea/Concept** | Validate interest before building | Pretotyping + Effectuation | >10% ILI |
| **2 - Problem** | Confirm the problem is real and painful | Customer Development + JTBD | 60%+ urgency |
| **3 - Solution** | Test solutions without building | Concierge/Wizard of Oz MVP | 40%+ willing to pay |
| **4 - PMF** | Measure product-market fit | Sean Ellis 40% Test | 40%+ "very disappointed" |
| **5 - Scale** | Validate unit economics | Bessemer's 10 Laws | LTV/CAC > 3 |
| **6 - Expansion** | Build defensible moats | NFX Network Effects | NRR > 100% |

---

## 🚀 Quick Start

### For Founders

1. **Identify your current phase** using the table above
2. **Open the phase-specific template** from `/templates`
3. **Work through the checklist** - be honest about evidence
4. **Make the Go/No-Go decision** with confidence

### For AI Tools (Codex, Hermes, Claude Code)

Use the context engineering prompts in [`templates/context-engineering-prompts.md`](./templates/context-engineering-prompts.md):

- **Chain-of-Thought (CoT)** - Step-by-step structured reasoning
- **Tree-of-Thoughts (ToT)** - Multi-expert panel evaluation
- **ReAct** - Dynamic reasoning with tool use

---

## 📁 Repository Structure

```
business-validation-phases/
├── SKILL.md                              # Complete framework documentation
├── README.md                             # You are here
└── templates/
    ├── pretotyping-checklist.md          # Phase 1: Idea validation
    ├── customer-discovery-guide.md       # Phase 2: Problem interviews
    ├── mvp-decision-matrix.md            # Phase 3: Solution testing
    ├── pmf-measurement.md                # Phase 4: PMF validation
    ├── scale-validation.md               # Phase 5: Unit economics
    ├── expansion-network-effects.md      # Phase 6: Moats & growth
    └── context-engineering-prompts.md    # AI validation patterns
```

---

## 🧠 Frameworks Integrated

### Traditional/Academic
- **Lean Startup** (Eric Ries) - Build-Measure-Learn feedback loops
- **Customer Development** (Steve Blank) - 4-step validation methodology
- **Jobs-to-be-Done** (Clay Christensen) - "People hire products to get jobs done"
- **Design Thinking** (Stanford d.school) - 5-stage human-centered design
- **Effectuation** (Saras Sarasvathy) - Expert entrepreneur decision logic

### VC/Accelerator Frameworks
- **YC Philosophy** - "Make Something People Want"
- **Sequoia Capital** - 4 Terrifying Questions
- **First Round Capital** - The PMF Method (4 levels)
- **Bessemer 10 Laws** - Cloud metrics & 5 C's
- **a16z** - Marketplace 13 Metrics
- **NFX** - 16 Types of Network Effects

### Validation Methods
- **Pretotyping** (Alberto Savoia) - Fake door, video MVPs, ILI metrics
- **MVP Types** - Concierge, Wizard of Oz, Mechanical Turk, Pinocchio
- **Sean Ellis Test** - 40% "very disappointed" threshold
- **AARRR Metrics** (Dave McClure) - Pirate metrics

---

## 💡 Key Principles

1. **Kill ideas fast** if validation fails. Don't fall in love with solutions.
2. **Demand evidence.** Opinions and "interesting" responses don't count.
3. **Founder-problem fit matters.** Founders need authentic insight into the pain.
4. **Niche down aggressively.** The narrow wedge always beats broad markets.
5. **Think 10 years.** Will this be enduring? Will you still care?

---

## 🛠 Usage Examples

### Phase 2: Problem Validation

```markdown
# Customer Interview Script (from templates/customer-discovery-guide.md)

## Question 1: Tell me about the last time you [experienced problem]
→ Look for: Concrete stories, not opinions
→ Red flag: "That sounds interesting" (polite, not urgent)
→ Green flag: "This happens all the time"

## Question 2: What do you currently do to solve this?
→ Look for: Manual workarounds, spreadsheets, expensive solutions
→ Red flag: "Nothing really"
→ Green flag: Spending money/time to work around

Minimum: 40 problem interviews
Target: 60%+ confirm urgent problem
```

### Phase 4: PMF Measurement

```markdown
# Sean Ellis 40% Test (from templates/pmf-measurement.md)

Ask: "How would you feel if you could no longer use [product]?"

□ Very disappointed: ___% (Target: >40%)
□ Somewhat disappointed: ___%
□ Not disappointed: ___%

□ Follow-up: "What's the main reason?"
→ Capture themes: Saves time / Better than X / Essential for workflow
```

### Phase 5: Unit Economics

```markdown
# CAC Payback (from templates/scale-validation.md)

LTV = (ARPU × Gross Margin) / Churn
CAC = Sales & Marketing Spend / New Customers

□ LTV: $_____
□ CAC: $_____
□ LTV/CAC ratio: _____ (Target: >3)
□ Payback period: _____ months (Target: <12)
```

---

## 🎓 Learning Path

### First-Time Founder
1. Start with **Phase 1** - Read `templates/pretotyping-checklist.md`
2. Complete Bird-in-Hand worksheet
3. Run first Fake Door test (48 hours)
4. Move to Phase 2 based on results

### Experienced Founder
1. Jump to your current phase
2. Fill the template gaps
3. Identify your strongest Go signals
4. Focus on weakest validation area

### AI-Assisted Validation
1. Read `templates/context-engineering-prompts.md`
2. Use CoT patterns for single-idea deep dives
3. Use ToT for panel-style evaluation
4. Use ReAct for dynamic research

---

## 🔗 Related Resources

- [Y Combinator Startup Library](https://www.ycombinator.com/library)
- [The Lean Startup](https://theleanstartup.com/) by Eric Ries
- [The Mom Test](http://momtestbook.com/) by Rob Fitzpatrick
- [NFX Network Effects](https://www.nfx.com/post/network-effects-bible/) Bible
- [First Round Review](https://review.firstround.com/)

---

## 🤝 Contributing

This framework synthesizes 25+ years of startup research. If you have:
- New validation case studies
- Framework improvements
- Phase-specific tools
- Context engineering patterns

Open an issue or PR with evidence-backed additions.

---

## 📜 License

MIT License - See [LICENSE](./LICENSE) for details.

---

## 🙏 Acknowledgments

Frameworks synthesized from:
- **Eric Ries** (Lean Startup)
- **Steve Blank** (Customer Development)
- **Clayton Christensen** (Jobs-to-be-Done)
- **Saras Sarasvathy** (Effectuation)
- **Sequoia Capital** (Arc Program)
- **First Round Capital** (PMF Method)
- **Bessemer Venture Partners** (10 Laws)
- **Andreessen Horowitz** (Marketplace Metrics)
- **NFX** (Network Effects Masterclass)

---

<p align="center">
  <b>Validate before building. Build what people want.</b>
</p>

<p align="center">
  ⭐ Star this repo if it helps your startup journey
</p>
