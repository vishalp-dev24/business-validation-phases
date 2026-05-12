# Stress Test Findings - business-validation-phases Skill

**Date:** Tuesday, May 12, 2026  
**Tests Run:** 8 complete validations (1 timeout)  
**Total Runtime:** ~120 minutes across all subagents

---

## Critical Issues Found

### 1. DANGEROUS: No Health Tech Warning (SEVERITY: CRITICAL)

**Test:** batch1-test7-anxiety-predictor.md  
**Finding:** Skill treats medical device like photo-sharing app

What happens:
- Validates "AI that predicts anxiety" as if it's a weather app
- Measures signups, not clinical outcomes
- No FDA/regulatory consideration
- No "what if this makes anxiety WORSE?" check

**Real-world risk:** Following this skill for health tech could cause patient harm.

**Required Fix:** Add industry detection with health tech specific warnings:
```markdown
⚠️ REGULATED INDUSTRY DETECTED
This idea involves medical/health claims. Standard validation frameworks
are DANGEROUS here. Additional requirements:
- Clinical evidence (not just interest)
- FDA device classification
- Adverse event monitoring
- IRB approval for testing
- Medical advisor required
```

---

### 2. Hardware Product Blind Spot (SEVERITY: HIGH)

**Tests:** batch1-test3-beverage-chiller.md  
**Finding:** MVP decision tree assumes software

The Pretotyping Checklist only has paths for:
- Complex backend → Wizard of Oz / Mechanical Turk
- Simple product → Fake Door MVP

Missing hardware path:
- Physical product that can't be faked → Functional prototype required
- Manufacturing partners needed
- Timeline 10x longer

**Required Fix:** Add hardware branch to MVP decision tree

---

### 3. Two-Sided Marketplace Complexity Ignored (SEVERITY: HIGH)

**Tests:** batch1-test9-sneaker-auth.md, batch1-test2-storygrandma.md  
**Finding:** Framework validates one side, misses chicken-and-egg

The interview count says "40 customers" but for a marketplace that's theoretically WRONG:
- 40 sellers + 40 buyers + 40 authenticators = 120 interviews
- No liquidity testing guidance
- No fake inventory strategies
- No side-sequencing guidance (which side first?)

**Required Fix:** Detect marketplace ideas and adjust framework

---

### 4. 18 Pain Points in Template Usability (SEVERITY: MEDIUM)

**Tests:** batch1-test8-cannabis-saas.md  
**Finding:** Excellent frameworks, poor execution

- No phase auto-detection (user must choose from 6 phases + 7 templates)
- Template overload creates decision paralysis  
- No scoring rubrics (checklists without "what's good enough")
- Generic interview questions miss industry-specific context

---

### 5. Time Estimates Missing (SEVERITY: MEDIUM)

**All tests** show time per phase but skill has no guidance:
- How long should Phase 1 take?
- What's too fast (probably wrong) vs too slow (probably stuck)?

---

## Stress Test Results by Test

| Test | Idea | Result | Key Finding |
|------|------|--------|-------------|
| test2-storygrandma.md | Storytelling marketplace | PASS (7/10) | Founder identity problem - skill assumes real founder |
| test3-beverage-chiller.md | Hardware chiller | PASS (7.6/10) | Hardware assumptions don't fit |
| test4-carbon-consultants.md | B2B marketplace | PASS (9.2/10) | Best case - fits naturally |
| test5-receipt-recipes.md | Consumer app | PASS (7.4/10) | Missing app-specific templates |
| test6-construction-safety.md | B2B AI | PASS (8/10) | Solid framework, minor gaps |
| test7-anxiety-predictor.md | Health AI | **DANGEROUS** | No medical device awareness |
| test8-cannabis-saas.md | Regulated SaaS | PASS (B/10) | 18 usability pain points |
| test9-sneaker-auth.md | Three-sided marketplace | PASS (7.2/10) | Multi-sided complexity ignored |

---

## Recommended Skill Fixes

### Immediate (Critical Safety)

1. **Add Industry Detection Header**
   - Health/medical → Warning + special requirements
   - Hardware/physical → Different MVP path
   - Regulated (cannabis, finance, etc.) → Compliance checklist
   - Marketplace → Multi-sided framework

2. **Remove Dangerous Defaults**
   - Don't suggest "build landing page" for medical devices
   - Don't use retention benchmarks for recovery apps

### Short Term (High Impact)

3. **Add Time Guidance**
   - Phase 1: 2 days 
   - Phase 2: 2-3 weeks
   - Phase 3: 1-2 weeks
   - Phase 4: 2-4 weeks
   - Phase 5: Ongoing
   - Phase 6: After PMF

4. **Add Customer Sourcing Section**
   - Where to find people by industry
   - Outreach templates
   - Incentive structures

5. **Fix MVP Decision Tree**
   - Add physical product branch
   - Add regulated product branch  
   - Add service vs product distinction

### Medium Term (Quality of Life)

6. **Template Selector Flowchart**
   - "I have an idea" → Go here
   - "I built something" → Go there
   - "I'm scaling" → Use this

7. **Add Progress Tracking**
   - Store interview count
   - Track which milestones reached
   - Save validation state

---

## Files Generated

All test outputs saved to:
```
~/github-push/business-validation-phases/stress-tests/
├── batch1-test2-storygrandma.md (9,951 bytes)
├── batch1-test3-beverage-chiller.md (15,000+ words)
├── batch1-test4-carbon-consultants.md (20,000+ chars)
├── batch1-test5-receipt-recipes.md (15.9 KB)
├── batch1-test6-construction-safety.md (414 lines)
├── batch1-test7-anxiety-predictor.md (689 lines)
├── batch1-test8-cannabis-saas.md (15KB)
└── batch1-test9-sneaker-auth.md (14,182 bytes)
```

---

## Overall Assessment

**Skill Rating: 7.5/10**

**Strengths:**
- Comprehensive framework coverage
- Professional template quality  
- Clear Go/No-Go criteria
- Good integration with entrepreneurship research

**Critical Weaknesses:**
- DANGEROUS for regulated industries (health, finance)
- Missing domain-specific adaptations
- Requires founder context (can't validate pre-founder)
- No automated execution

**Recommendation:** 
APPROVED with critical warning labels added. Do not use for medical/health ideas without additional clinical validation.

---

*Generated from 8 parallel stress tests run on Tuesday, May 12, 2026*
