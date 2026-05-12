# Enhanced MVP Decision Matrix

Based on stress testing findings (May 2026) - adds missing branches for hardware, regulated, and multi-sided products.

---

## BEFORE: Original MVP Decision Tree (Software Only)

```
Decision Tree:
Is backend complex?
├── YES → Can humans do the work?
    ├── YES → Wizard of Oz MVP
    └── NO → Mechanical Turk MVP
```

**Problem:** This only covers software. BREAKS for hardware, health, marketplace.

---

## AFTER: Enhanced MVP Decision Matrix with All Branches

### STEP 1: Product Type Assessment

First, identify your product type:

| Type | Key Characteristics | Examples |
|------|----------------------|----------|
| **A. Digital/Software** | Can be built with code | SaaS, app, platform |
| **B. Physical/Hardware** | Requires manufacturing | Devices, sensors, tools |
| **C. Service** | Human-delivered | Consulting, agency |
| **D. Hybrid** | Software + Physical | IoT, connected devices |

### STEP 2: Risk Classification

| Risk Level | Description |
|------------|-------------|
| **LOW** | Consumer software, content, productivity |
| **MEDIUM** | B2B SaaS, marketplaces, fintech |
| **HIGH** | Health, safety-critical, regulated industries |

---

## Type A: Digital/Software (Enhanced)

### Decision Tree - Software

```
Is backend complex (ML, distributed systems)?
├── YES → Can humans plausibly simulate?
│   ├── YES → Wizard of Oz MVP
│   │   *Example: Zappos - humans photographed shoes*
│   │
│   └── NO → Mechanical Turk + Alpha
│       *Example: Cardmunch - humans transcribed cards*
│
└── NO → Is this infrastructure (payment, comms)?
    ├── YES → Use existing APIs
    │   *Stripe, Twilio, Sendgrid*
    │
    └── NO → Standard MVP
        ├── Landing page test
        ├── Waitlist validation
        └── Concierge MVP
```

### Software - Special Cases

#### Two-Sided Marketplace

```
Can match supply/demand manually first?
├── YES → Paper Marketplace
│   *Manually connect via email/Instagram/WhatsApp*
│   *Target: 10 manual transactions in 30 days*
│
└── NO → Geographic Constraint MVP
    *Start in one city, expand later*
    *Manually recruit both sides locally*
```

#### AI/ML Where Core Value Is Prediction

**WARNING:** Standard MVPs may not apply

| Can Simulate? | Approach |
|---------------|----------|
| YES (humans can approximate) | Wizard of Oz with performance disclosure |
| NO (prediction must be accurate) | Benchmark dataset → Limited pilot |

**Red flag:** Medical diagnosis, anomaly detection, safety-critical predictions

---

## Type B: Physical/Hardware (NEW BRANCH - Critical Fix)

### Decision Tree - Hardware

```
Can you fake the core experience?
├── YES → Pinocchio MVP
│   *Non-functional prototype for interest/gathering*
│   *3D renderings, mockups, vibe demonstrations*
│   *Target: Pre-orders > 100 units
│
├── PARTIAL (software simulates hardware)
│   ├── Virtual Reality MVP
│   │   *App simulates what hardware would do*
│   │   *Example: Hardware companion app only*
│   │
│   └── Smartphone-as-Proxy
│       *Use phone sensors instead of custom hardware*
│
└── NO →
    ├── Can you rent existing hardware?
    │   ├── YES → Integration MVP
    │   │   *Build software on existing hardware*
    │   │
    │   └── NO → Functional Prototype Required
    │       *See "Pre-Prototype Phase" below*
```

### Hardware - Pre-Prototype Phase

**Before building anything physical:**

1. market_validation:
   - [ ] Landing page with renders: >500 signups
   - [ ] Explainer video: >1min average watch time
   - [ ] Pre-order page: Target 100+ pre-orders

2. technical_validation:
   - [ ] Physics simulation (thermal, structural)
   - [ ] Component sourcing identified
   - [ ] Manufacturing partners contacted (3+ quotes)
   - [ ] Patent/IP search complete

3. unit_economics_prototype:
   - [ ] BOM cost estimate
   - [ ] Retail price validated (>2x BOM)
   - [ ] Shipping/storage cost model

### Hardware - Prototype Timeline

| Phase | Timeline | Validation |
|-------|----------|------------|
| Render MVP | 1 week | Interest gathering |
| Mockup/3D | 2 weeks | Pre-sales |
| Proof of Concept | 4-8 weeks | Core mechanism works |
| Functional Prototype | 8-16 weeks | Customer testing |
| Design for Manufacture | 4-8 weeks | Partner validation |

**Critical:** Hardware takes 10x longer than software. Plan capital accordingly.

---

## Type C: Service (Enhanced)

### Decision Tree - Services

```
Can service be standardized?
├── YES (repeatable processes)
│   ├── Productized Service MVP
│   │   *Fixed scope, fixed price*
│   │   *Example: "Website in 2 weeks for $3k"*
│   │
│   └── Automation Layer MVP
│       *Humans deliver, software coordinates*
│       *Target: 20+ customers before automation*
│
└── NO (custom/variable scope)
    └── Concierge/High-touch MVP
        *Serve customers manually*
        *Document patterns for later productization*
        *Target: 10+ customers, document workflows*
```

### Service - Validation Checklist

1. founder_capability:
   - [ ] Can deliver service myself for 10 customers
   - [ ] Clearly defined scope for MVP
   - [ ] Pricing validated with 3+ customers

2. playbook_creation:
   - [ ] Documented repeatable processes
   - [ ] Identified what can be automated
   - [ ] Staffing model for scaling

3. business_model_tests:
   - [ ] Hourly vs project vs retainer pricing test
   - [ ] Upsell path identified
   - [ ] LTV/CAC calculation

---

## Type D: Hybrid (Software + Hardware)

### Decision Tree - Hybrid

```
Which part delivers core value?
├── HARDWARE is core
│   └── Follow Hardware path
│       *Use smartphone as proxy where possible*
│
├── SOFTWARE is core
│   └── Follow Software path
│       *Use existing hardware APIs*
│
└── BOTH equally important
    └── Sequential MVP
        ├── Phase 1: Software MVP with simulated hardware
        ├── Phase 2: Hardware alpha (limited devices)
        └── Phase 3: Integrated beta
```

### Hybrid - Example: Smart Home Device

```
Week 1-2: App MVP
- Build control app
- Use smartphone sensors as proxy
- Validate user wants remote control

Week 3-6: Hardware Renderings
- Create product renders
- Landing page + pre-orders
- Target: 200+ pre-orders

Week 7-14: Proof of Concept
- Build 5 functional prototypes
- Test with 10 beta users
- Iterate on physical design

Week 15+: Hardware + Software Together
- Manufacture 50 units
- Pair with mobile app
- Beta launch
```

---

## REGULATED INDUSTRIES - Special Handling

### WARNING FRAMEWORK

**These industries need MORE than standard validation:**

- Health/Medical
- Financial Services  
- Transportation (drones, autonomous vehicles)
- Food/Drug
- Children's products
- Weapons/accessories

### Additional Validation Layers

| Requirement | Standard | Regulated Industry |
|-------------|----------|-------------------|
| Problem validation | 40 interviews | 60+ interviews |
| Legal review | Optional | Required before MVP |
| Compliance | Self-attestation | Third-party audit |
| Evidence type | Interest/behavior | Clinical/safety data |
| Timeline multiplier | 1x | 3-5x |

### Specific Industry Adaptations

#### Health Tech / Medical Devices

**STOP. Read this.**

The standard framework measures interest. Health requires evidence.

```
Where does this fall?
├── Wellness/Lifestyle (fitness, meditation)
│   └── Standard validation OK
│       *Warn: Cannot make medical claims*
│
├── Health Monitoring (sleep, activity)
│   └── Enhanced validation
│       *FDA/CDRH classification required*
│       *Clinical accuracy testing*
│
├── Diagnosis/Treatment
│   └── **STOP - Clinical Validation Required**
│       *Cannot use pretotyping*
│       *Requires IRB approval*
│       *FDA clearance pathway*
│       *See warnings section in SKILL.md*
│
└── FDA Regulated (Class I/II/III)
    └── **STOP - See Medical Device Framework**
        *510(k), De Novo, or PMA required*
        *Clinical trials*
        *Medical advisor required*
```

**Additional Requirements:**
- Clinical advisor (MD, PhD)
- Regulatory consultant
- IRB-approved study design
- Adverse event monitoring plan

#### FinTech

```
What are you handling?
├── Payments only (no lending)
│   └── Standard validation + compliance review
│       *PCI DSS requirements*
│       *Money transmitter licenses*
│
├── Lending/Credit
│   └── Enhanced requirements
│       *State lending licenses*
│       *Credit reporting compliance*
│       *Fair lending practices review*
│
├── Securities/Investments
│   └── **STOP - Financial Advisor Required**
│       *SEC registration considerations*
│       *Broker-dealer vs RIA status*
│
└── Crypto/DeFi
    └── **STOP - Regulatory Uncertainty**
        *Howey test application*
        *Money transmitter (+ state licenses)*
        *Consumer protection compliance*
```

#### Cannabis

```
State-by-State Complexity:
- Different regulations per state
- Cannot cross state lines
- Banking restrictions
- Advertising restrictions
- Age verification requirements

Additional Validation:
- [ ] Legal review for each target state
- [ ] Compliance software identified
- [ ] Banking relationship established
- [ ] Insurance (crop, liability)
```

---

## GO/NO-GO Gates by MVP Type

| MVP Type | Go Signal | No-Go Signal |
|----------|-----------|--------------|
| **Fake Door** | >10% signup rate | <5% or no qualified traffic |
| **Wizard of Oz** | >40% willingness to pay | Manual delivery unsustainable |
| **Functional Prototype** | >5 satisfied customers | Core mechanism doesn't work |
| **Pre-order** | >100 pre-orders | <50 signups |
| **Paper Marketplace** | 10 manual transactions | Can't match supply/demand |
| **Clinical Pilot** | Efficacy demonstrated | Adverse events or no effect |

---

## UPDATED TEMPLATES NEEDED

Test findings show these templates need updates:

- [X] `mvp-decision-matrix.md` - **This file** - Hardware/Regulated branches added
- [ ] `customer-discovery-guide.md` - Add customer sourcing by industry
- [ ] `pretotyping-checklist.md` - Add hardware pre-prototype phase
- [ ] `expansion-network-effects.md` - Add marketplace liquidity templates
- [ ] NEW: `clinical-validation-checklist.md` - For health tech
- [ ] NEW: `marketplace-validation-guide.md` - Multi-sided framework

---

## STRESS TEST CITATIONS

| Finding | Source Test | Severity |
|---------|-------------|----------|
| Hardware not covered | test3-beverage-chiller | HIGH |
| Medical device danger | test7-anxiety-predictor | CRITICAL |
| Marketplace gaps | test9-sneaker-auth | HIGH |
| Need customer sourcing | test8-cannabis-saas | MEDIUM |

---

*Enhanced MVP Decision Matrix v1.1*  
*Incorporates 8 stress test findings*  
*Created: May 2026*