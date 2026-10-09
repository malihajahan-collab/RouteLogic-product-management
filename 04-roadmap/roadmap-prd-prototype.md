# RouteLogic Velocity — Roadmap, PRD & Prototype

> **Roadmap principle:** Prioritize the frontline execution problems most closely tied to trust, adoption, and at-risk account retention.

---
<img width="1881" height="885" alt="image" src="https://github.com/user-attachments/assets/e74538eb-f89a-482e-b0dc-5e66908c0c74" />

## 12-Week Product Roadmap

### NOW — Validate the Core Execution Layer  
**Weeks 1–4 · 3 pilot accounts**

| Initiative | Why Now |
|---|---|
| **One-Click Compliance Checklist** | Directly targets a measurable workflow leak: only 48% complete past compliance |
| **Driver Alert Notifications** | Reduces the need for calls and WhatsApp during urgent changes |
| **Step Progress Indicator** | Makes core workflow state visible without adding new complexity |
| **Shift Handoff Wizard** | Reduces manual notes and fragmented exception context |

**Pilot checkpoints**
- Week 2: CS training and midpoint review
- Week 4: Go / iterate / kill decision
- Team: 2 engineers · 1 designer · 1 CS lead

---

### NEXT — Simplify the Daily Operating Experience  
**Weeks 5–8**

| Initiative | Why Next |
|---|---|
| **High-Velocity Mode / UI Simplification** | Extends the pilot learning into a cleaner frontline experience |
| **Mobile-First Coordinator Dashboard** | Improves access to the operational information coordinators use most often |

These are higher-effort changes, so they follow validation of the core workflow rather than leading it.

---

### LATER — Extend Value Without Reintroducing Clutter  
**Weeks 9–12+**

- Smart Daily Report Auto-Fill
- Compliance Audit Trail Export
- In-App Coordinator Training

These may add value, but they are not required to prove the core Velocity bet.

---

## Cut / Defer List

| Initiative | Decision | PM Rationale |
|---|---|---|
| **Contextual AI ETA Display** | Defer | No strong evidence that ETA prediction is the primary user problem or retention lever |
| **Fleet Analytics Manager View** | Defer | Useful for managers, but does not address the frontline execution crisis driving the 12-week roadmap |

> **PM judgment:** A feature can be relevant to logistics and still have no strategic right to consume engineering capacity now.

---

## How My PM Input Changed the Roadmap

The first-pass feature set was capability-heavy. I reprioritized it using the evidence from discovery and analytics.

| Initial Bias | PM Override |
|---|---|
| Add useful logistics features | Prioritize the broken Fleet Coordinator job-to-be-done |
| Treat all high-value ideas similarly | Separate urgent execution fixes from adjacent capability |
| Optimize for feature breadth | Optimize for trust, speed, and in-platform completion |
| Keep attractive AI/analytics ideas | Defer ideas without evidence of user or retention impact |

**Result:** the roadmap moved from a feature list to a sequence of bets tied to measurable user and business outcomes.

---

## Top NOW Feature

### One-Click Compliance Checklist

**Core outcome:** Help Fleet Coordinators complete compliance inside the dispatch flow with fewer steps and fewer manual workarounds.

**Success signal:** workflow completion past compliance improves from **48% to 63%**.

**Diagnostic signal:** compliance step time improves from **14.6 minutes to ≤10 minutes**.

**Guardrails:** GPS accuracy ≥95% · driver-status sync errors ≤2%.

---

## Simplified PRD Snapshot

### Vision
Make compliance a fast, trustworthy step inside dispatch—not a separate workflow coordinators have to work around.

### Must-Haves
- Auto-populate route, driver, and vehicle information
- Show only required compliance items
- Highlight missing or invalid information
- Block approval when required information is invalid
- Allow one-click approval when all required checks pass
- Record timestamp, coordinator, and approval status
- Keep the user inside the dispatch workflow

### Explicitly Not in V1
- AI ETA recommendations
- Manager analytics
- Broad reporting automation
- Training modules
- New data sources or backend architecture changes

---

## Roadmap & Prototype

**Interactive roadmap:**  
https://bolt.new/~/sb1-pxzxtfvc

**Clickable prototype:**  
https://preview--swift-check-approve.lovable.app/

---

## Strategic Takeaway

> **The roadmap protects focus by sequencing the work around the product crisis, not around the size of the backlog.**

Velocity starts by proving that RouteLogic can restore frontline execution trust before investing in broader experience redesign or adjacent capability.
