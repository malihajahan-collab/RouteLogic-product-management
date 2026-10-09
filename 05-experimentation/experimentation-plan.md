# RouteLogic Velocity — Experimentation Plan

> **Decision question:** Does simplifying the compliance workflow keep more Fleet Coordinators in RouteLogic without weakening operational accuracy?

---

## Hypothesis Under Test

> **Based on UXR evidence of workflow complexity, manual workarounds, and a 48% baseline completion rate past the compliance step, I believe that introducing the One-Click Compliance Checklist for Fleet Coordinators will improve in-platform execution, as measured by increasing workflow completion past compliance from 48% to 63% (+15 percentage points) within 4 weeks. I will protect GPS accuracy ≥95% and driver-status sync errors ≤2%.**

---

## Experiment Design

| Element | Decision |
|---|---|
| **Method** | 50/50 A/B test |
| **Control** | Current multi-step compliance workflow |
| **Variant** | One-Click Compliance Checklist |
| **Primary metric** | Workflow completion past compliance |
| **Baseline** | 48% |
| **Minimum Detectable Effect** | +15 percentage points |
| **Success threshold** | ≥63% |
| **Diagnostic metric** | Compliance step time: 14.6 min → ≤10 min |
| **Guardrails** | GPS accuracy ≥95% · driver-status sync errors ≤2% |
| **Sample target** | ~175 qualifying workflow observations per arm |
| **Decision window** | 4 weeks minimum |

---

## What Changes — and What Does Not

### Control
Fleet Coordinators use the current compliance flow with multiple steps and navigation.

### Variant
The same workflow is simplified into one in-flow checklist that:
- pre-populates known route, driver, and vehicle data
- surfaces missing or invalid items
- enables approval only when required checks pass
- records the approval without leaving dispatch

### Held Constant
- Compliance rules
- Underlying GPS and status systems
- Core dispatch workflow
- Data sources and backend integrations
- Manager reporting

> **Experiment discipline:** Change the compliance interaction, not the surrounding system, so any lift can be attributed to the workflow simplification.

---

## Pre-Launch Decision Criteria

| Outcome | Decision |
|---|---|
| Primary metric reaches **≥63%**, `p < 0.05`, guardrails intact | 🚢 **SHIP** |
| Positive direction, but lift stays below +15pp | 🔁 **ITERATE** |
| Primary improves, but a guardrail breaks or key segments are harmed | 🔍 **INVESTIGATE** |
| No improvement or negative movement | ☠️ **KILL** |

**Read date:** End of week 4.  
**No early success redefinition or mid-test metric changes.**

---

## Result Quality Checks

Before making the decision, I would ask:

1. **Significance:** Is the result unlikely to be random (`p < 0.05`)?
2. **Magnitude:** Did the lift clear the +15pp threshold?
3. **Confidence:** Is the confidence interval narrow enough to support action?
4. **Guardrails:** Did speed improve without weakening data accuracy?
5. **Segments:** Did the average hide harm across account, device, or user-tenure groups?

---

## How My PM Input Improved the Experiment

The first-pass experiment could have optimized for whether users clicked or adopted the new checklist.

I reframed the test around the **user outcome** and locked the decision rules before seeing results.

| Initial Risk | PM Decision |
|---|---|
| Measure feature usage | Measure **workflow completion** |
| Treat any lift as success | Set a **+15pp MDE** before launch |
| Focus only on speed | Protect **GPS and sync accuracy** |
| Change several experience elements | Isolate **one workflow change** |
| Decide after seeing results | Pre-commit **Ship / Iterate / Investigate / Kill** criteria |

> **The goal is not to prove the feature works. It is to create evidence strong enough to make a product decision.**

---

## Business Link

**At-risk account retention** remains the North Star, but a 4-week workflow test cannot credibly prove retention impact.

This experiment tests the controllable leading signal:

**higher in-platform completion → fewer workarounds → stronger operational trust → lower retention risk**

---

## Findings & Decision

**Status: Not yet run.**

No result is claimed in this portfolio. The experiment brief documents the hypothesis, thresholds, guardrails, and decision criteria that would be used before exposing the feature to real users.

---

## Experimentation Takeaway

> **Experimentation is a decision system, not a feature-validation exercise.**

A successful test must show a meaningful user outcome, clear the pre-defined decision threshold, and avoid creating hidden damage elsewhere in the product.
