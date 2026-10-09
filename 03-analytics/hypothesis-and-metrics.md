# Hypothesis & Success Metrics

> **Strategic goal:** Improve frontline product trust in a way that supports retention of at-risk enterprise accounts.

---

## Product Hypothesis

> **Based on UXR evidence of workflow complexity, manual workarounds, and a 48% baseline completion rate past the compliance step, I believe that simplifying the compliance workflow for Fleet Coordinators will improve in-platform execution, as measured by increasing workflow completion past compliance from 48% to 63% (+15 percentage points). I will protect real-time operational accuracy—GPS accuracy ≥95% and driver-status sync errors ≤2%—and make a go/no-go decision after 4 weeks.**

---

## Metric Hierarchy

| Metric | Type | Target | Why It Matters |
|---|---|---:|---|
| **At-risk account retention** | North Star / lagging business outcome | Improve over time | Connects frontline product health to the enterprise renewal risk driving RouteLogic Velocity |
| **Workflow completion past compliance** | Primary success metric / leading indicator | **48% → 63%** | Measures whether coordinators can complete the critical workflow in-platform |
| **Compliance step time** | Diagnostic friction metric | **14.6 min → ≤10 min** | Shows whether the workflow is becoming materially faster |
| **GPS accuracy** | Guardrail | **≥95%** | Prevents speed improvements from reducing operational accuracy |
| **Driver-status sync errors** | Guardrail | **≤2%** | Protects trust in real-time dispatch information |
| **Experiment window** | Decision window | **4 weeks** | Provides a fixed period for a go / iterate / kill decision |

---

## Why This Metric Structure

The business outcome we ultimately care about is **retaining at-risk enterprise accounts**.

But retention is a lagging result and cannot be credibly attributed to one 4-week workflow experiment.

For this test, the product team should therefore focus on a metric it can directly influence:

> **Can more Fleet Coordinators complete the compliance workflow inside RouteLogic without relying on manual workarounds?**

This keeps the experiment connected to the North Star without using retention as a short-term success claim.

---

## How My PM Input Improved the Initial Metric View

The initial metric view risked focusing on feature usage—whether coordinators clicked or used the new checklist.

I reframed success around **user outcome and business relevance**:

| Initial View | PM Reframe |
|---|---|
| Checklist usage | **Workflow completion past compliance** |
| Faster interaction | **Reduced operational friction** |
| Feature adoption | **More work completed inside RouteLogic** |
| Product metric in isolation | **Leading signal connected to account retention** |

**What changed:** the metric moved from proving the feature was used to proving the user's workflow improved.

---

## Decision Rule

- **SHIP:** Completion improves by **≥15 percentage points** at `p < 0.05`, with both guardrails intact.
- **ITERATE:** Direction is positive, but the lift does not clear the +15pp threshold.
- **KILL:** No improvement, negative movement, or a meaningful guardrail failure.
- **READ DATE:** End of week 4; no early redefinition of success.

---

## Strategic Takeaway

> **The experiment does not need to prove retention in four weeks. It needs to prove that RouteLogic is removing a measurable source of friction that contributes to retention risk.**

The metric hierarchy keeps the team focused on a product signal it can control while maintaining a clear line of sight to the business outcome that matters most.
