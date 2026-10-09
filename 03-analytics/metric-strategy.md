# RouteLogic Velocity — Metric Strategy & Business Linkage

> **Measurement principle:** Track whether frontline execution improves, while maintaining a clear line of sight to enterprise retention.

---

## Business Outcome

The strategic outcome is:

**At-risk enterprise account retention**

Retention is the business result RouteLogic ultimately needs to protect, but it is a lagging metric influenced by many factors outside a single workflow change.

For near-term product decisions, I therefore use controllable leading indicators rather than claiming short-term retention impact.

---

## Metric Hierarchy

| Metric | Role | Baseline / Target | Why It Matters |
|---|---|---:|---|
| **At-risk account retention** | Business North Star | Improve over renewal cycle | Tests whether stronger frontline value contributes to account retention |
| **Workflow completion past compliance** | Primary leading indicator | **48% → 63%** | Measures whether more work stays inside RouteLogic |
| **Compliance step time** | Diagnostic metric | **14.6 min → ≤10 min** | Indicates whether the workflow is materially easier to complete |
| **GPS accuracy** | Guardrail | **≥95%** | Prevents speed improvements from weakening operational accuracy |
| **Driver-status sync errors** | Guardrail | **≤2%** | Protects trust in live operational data |

---

## Why Workflow Completion Is the Primary Signal

Feature clicks or checklist usage would show activity, but not whether the user's job improved.

The stronger signal is:

> **Can more Fleet Coordinators complete the critical workflow inside RouteLogic without falling back to manual workarounds?**

That connects product behavior to the underlying problem identified in discovery.

---

## Metric Logic

**Less workflow friction**  
↓  
**Higher in-platform completion**  
↓  
**Fewer external workarounds**  
↓  
**Stronger operational trust**  
↓  
**Stronger adoption and renewal case**

This is a **causal hypothesis**, not a claim that one workflow change directly causes retention.

---

## What I Would Not Use as the Primary KPI

### Checklist clicks
Measures interaction, not user success.

### Feature adoption alone
A feature can be adopted without improving the end-to-end workflow.

### Compliance step time alone
Speed matters, but a faster workflow that reduces accuracy would be a poor product outcome.

### Four-week retention movement
Retention is too lagging and too confounded to use as the primary decision metric for a short pilot.

---

## PM Judgment

The initial metric view could have optimized for usage of the new feature.

I reframed the measurement model around three levels:

| Level | Question |
|---|---|
| **Business** | Are at-risk accounts more likely to remain with RouteLogic? |
| **Product** | Are more critical workflows completed inside RouteLogic? |
| **Operational** | Are we improving speed without weakening accuracy or trust? |

This keeps the team from confusing **feature activity** with **customer or business value**.

---

## Measurement Boundary

The 4-week pilot can provide evidence about workflow behavior and operational quality.

It cannot credibly prove:

- long-term retention impact
- population-wide causal impact
- sustained behavior change beyond the pilot period

Those require broader rollout and longer observation.

---

## Strategic Takeaway

> **A useful product metric should sit close enough to the user behavior the team can change, while still maintaining a defensible connection to the business outcome that matters.**

For RouteLogic Velocity, that means measuring **in-platform workflow completion** as the leading signal, while treating retention as the longer-term business outcome.
