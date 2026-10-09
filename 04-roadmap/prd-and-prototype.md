# One-Click Compliance Checklist — Scoped PRD & Prototype

> **Scope principle:** Build the shortest viable path that removes the compliance bottleneck without weakening operational accuracy.

---

## The NOW Feature

### One-Click Compliance Checklist

A single in-flow compliance step that pre-populates required information, surfaces only exceptions, and allows approval without leaving dispatch.

**Primary user:** Fleet Coordinator  
**Core problem:** Compliance is slow and fragmented, contributing to manual workarounds and workflow abandonment.

---

## Why This Feature Earned NOW

The feature connects directly to a measurable product leak:

- Only **48%** of workflows complete past the compliance step
- Current compliance time is **14.6 minutes**
- Coordinators already use external workarounds when RouteLogic becomes slow or cumbersome
- At-risk account retention is the business-level outcome Velocity is designed to protect

> **Product bet:** Remove avoidable compliance friction first, then test whether more work stays inside RouteLogic.

---

## MVP Scope — MoSCoW

### Must-Have

| Requirement | Why It Is a Ship-Blocker |
|---|---|
| Auto-populate route, driver, and vehicle | Removes duplicate entry |
| Show required checks only | Protects focus and compliance completeness |
| Flag missing / invalid information | Prevents false approval |
| Block approval until required items pass | Protects operational and compliance integrity |
| One-click approval when valid | Delivers the core speed improvement |
| Log timestamp, coordinator, and status | Maintains traceability |
| Stay inside dispatch flow | Removes the navigation friction being tested |

### Should-Have

- Clear progress / completion state
- Inline correction of missing information
- Visible approval confirmation
- Retry state if an update fails

### Could-Have

- Additional visual polish
- Configurable checklist ordering
- Expanded contextual help

### Won't-Have — V1

- Contextual AI ETA
- Fleet analytics
- Automated daily reporting
- Training module
- New external data integrations
- Autonomous compliance decisions

---

## What I Demoted — and Why

The initial scope risked treating several useful enhancements as MVP requirements.

I applied the MoSCoW **kill test**:

> If we remove this, can the Fleet Coordinator still complete the core compliance outcome?

If yes, it did not belong in Must-Have.

This pushed analytics, AI recommendations, reporting, training, and broader dashboard changes out of V1.

**PM judgment:** protecting the learning objective matters more than demonstrating feature breadth.

---

## Core User Flow

1. Coordinator opens the route in dispatch
2. Checklist pre-populates known route, driver, and vehicle information
3. System highlights only missing or invalid required items
4. Coordinator resolves exceptions in-flow
5. **Approve Compliance** becomes available when requirements are satisfied
6. Approval is logged and the route can proceed

---

## Smart Behaviors

| Situation | Expected Behavior |
|---|---|
| All required checks pass | Enable **Approve Compliance** |
| Required data is missing or invalid | Highlight the issue and block approval |
| Coordinator edits an exception | Revalidate the checklist immediately |
| Approval succeeds | Show confirmation and record coordinator + timestamp |
| Update fails | Show an explicit failure / retry state; never silently confirm success |
| Data confidence is insufficient | Surface uncertainty rather than inventing or assuming a valid state |

---

## Edge Cases

- Missing driver or vehicle information
- Invalid compliance field
- Weak or unavailable location signal
- Sync failure during approval
- Duplicate approval attempt
- Route state changes while checklist is open

The system should fail visibly and safely. It should never imply compliance approval when required information is unresolved.

---

## What the PRD Makes Explicit

A vague brief could easily interpret “one-click compliance” as approving everything automatically.

The PRD makes the boundary clear:

> **One click reduces interaction cost; it does not remove validation.**

Automation prepares and verifies the workflow. The Fleet Coordinator remains the decision-maker.

---

## Prototype Learning

The prototype makes one product principle tangible:

**The happy path should surface exceptions, not make the coordinator re-confirm information RouteLogic already knows.**

This reinforced the need to:
- pre-populate known data
- keep validation visible
- block invalid approval
- give explicit success or failure feedback

These behaviors were made explicit in the PRD so a prototype—or engineering implementation—does not fill the gaps with assumptions.

---

## Success Criteria

| Metric | Target |
|---|---:|
| Workflow completion past compliance | **48% → 63%** |
| Compliance step time | **14.6 min → ≤10 min** |
| GPS accuracy guardrail | **≥95%** |
| Driver-status sync error guardrail | **≤2%** |
| Decision window | **4 weeks** |

The experiment measures **workflow improvement**, not checklist clicks.

---

## Clickable Prototype

https://preview--swift-check-approve.lovable.app/

<img width="1202" height="556" alt="image" src="https://github.com/user-attachments/assets/a8261e1e-9823-41ec-862e-5683c0f8a25f" />


---

## PM Takeaway

> **Scoping is not deciding what the product could do. It is deciding the minimum the product must do to test the strategic bet credibly.**

The final scope protects both the user outcome and the experiment: fewer steps, clear validation, no unnecessary capability, and no hidden compromise on operational accuracy.
