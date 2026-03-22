# Assignment No. 01 — RPA Use Case: Employee Onboarding Analysis

## Course
Robotic Process Automation (RPA)

## Assignment Overview
Design and document an RPA use case analysis for a real-world business process. This assignment covers business process description, automation type evaluation, implementation planning, and projected benefits quantification.

---

## Deliverable

| File | Description |
|------|-------------|
| `rpa-onboarding.html` | Single-page interactive website presenting the full use case analysis |

To view: open `rpa-onboarding.html` in any web browser (Chrome, Edge, Firefox, Safari).

---

## Topic
**Employee Onboarding Automation**

HR onboarding was selected as the use case due to its high transaction volume, rule-based workflow structure, multi-system data entry requirements, and clear pain points — all of which make it a strong candidate for RPA.

---

## Website Structure

### Section 1 — Introduction
Provides context on why HR onboarding is suitable for RPA automation. Covers the manual nature of existing processes, the cascade of activities triggered by each new hire, and the characteristics (structured data, predictable rules, high volume) that make it automation-ready.

### Section 2 — Business Process Description
Documents the end-to-end onboarding workflow across seven steps:
1. Job Offer & Acceptance
2. Pre-Onboarding Setup
3. Document Management
4. Payroll & Benefits Setup
5. IT & Equipment Provisioning
6. Orientation & Training Scheduling
7. First-Day Follow-Up

**Systems involved:**
- **JD Edwards** — HRIS / ERP
- **Paycon** — Payroll
- **Microsoft 365** — Email & IT provisioning
- **OneDrive / SharePoint** — Document storage

**Key pain points identified:**
- Manual re-entry of employee data across disconnected systems
- Duplicate effort and time-consuming setup
- Payroll entry errors (5–10% error rate)
- Manual document tracking via email
- Lack of native integration between JD Edwards, Paycon, and Microsoft 365

### Section 3 — Use Case Evaluation
**Recommended Automation Type: Hybrid RPA**

- **Unattended automation** handles standard, high-volume tasks: JD Edwards data entry, Microsoft 365 account creation, SharePoint document uploads, Paycon payroll setup.
- **Attended automation** supports HR in exception handling: visa cases, custom benefits, compliance sign-offs.

Justification: The majority of hires are standard and rule-based — ideal for unattended bots. Edge cases are preserved for human-in-the-loop review, balancing efficiency with oversight.

### Section 4 — Implementation Plan (High-Level)
**Priority automation targets:**
1. Employee data entry into JD Edwards
2. Microsoft 365 account creation
3. Document uploads to SharePoint
4. Payroll setup in Paycon

**Tools & platforms considered:**
- UiPath, Automation Anywhere, Blue Prism, Microsoft Power Automate
- JD Edwards REST API (preferred) / screen scraping (fallback)
- Microsoft Graph API for M365 provisioning
- SharePoint REST API / Power Automate connectors

**Implementation challenges noted:**
- Exception handling for non-standard hire types
- JD Edwards API limitations
- PII data security across automated workflows
- Inconsistent SharePoint permission structures
- HR change management and adoption

### Section 5 — Projected Benefits (Quantified)

| Metric | Before | After | Improvement |
|--------|--------|-------|-------------|
| Time per hire | 4–6 hours | 1–2 hours | ~65–75% reduction |
| Payroll/HRIS error rate | 5–10% | <1% | ~90% reduction |
| Weekly HR hours (50 hires/week) | 250–300 hrs | 50–75 hrs | ~75–80% savings |
| Document completeness | ~70–80% | >95% | Significant compliance gain |
| Time-to-productivity | 3–5 days | 1–2 days | Faster ramp-up |

**Visual charts included:**
- Bar chart comparing time per hire and weekly HR hours before/after automation
- Bar chart comparing payroll error rate and document completeness before/after automation

**Summary:** Hybrid RPA reduces manual effort by 70–80%, brings error rates below 1%, and accelerates new hire readiness — freeing HR to focus on strategic and relationship-driven work.

---

## Technical Notes

- Built as a single self-contained HTML file (no build tools or dependencies required)
- Charts rendered using **Chart.js** (loaded via CDN)
- Fully responsive layout using CSS Grid and Flexbox
- No frameworks — plain HTML, CSS, and vanilla JavaScript

---

## How to Open

```
Double-click rpa-onboarding.html
```
or drag and drop into any web browser window.
