# FieldTrack — Technical One-Pager

**Purpose:**  
Rapid, field-ready system for emergency response headquarters to aggregate relief needs from affected areas and allocate available aid resources through streamlined workflows. MVP must ship in 1 week; strict focus on needs intake, status tracking, aid inventory management, and allocation workflows.

**What Is Tracked:**  
- Community needs from affected areas (location, type, quantity, urgency, demographics)
- Aid stock inventory (type, quantity, location, allocation status)
- Allocation assignments (matching needs to available aid resources)
- Not tracked: field distribution details, individual beneficiary data, equipment, tools (V2+ scope)

**Main Users & Roles:**  
- **Admin/HQ Coordinator:** Aggregates needs, manages aid inventory, creates allocation assignments, tracks fulfillment status.
- **Field Intake Specialist:** Submits needs assessments from affected communities, updates needs status and urgency levels.
- **Aid Logistics Manager (V1):** Views aggregated reports, optimizes routing, tracks fulfillment rates.
- **No extra roles, no analytics, no integration — just get needs data in, aid stock tracked, allocations made, data exported fast.**

**Core Features (MVP/V0):**  
- Needs registry: Create/edit/update needs records (location, type, quantity, urgency, demographics) with status tracking (Reported, Verified, Allocated, Fulfilled, Critical).
- Priority classification: Assign urgency levels (Critical/24hr, High/48hr, Medium/72hr, Low/Planning).
- Aid stock management: Track available relief supplies (type, quantity, location, allocation status).
- Allocation workflows: View needs alongside available aid, create allocation assignments, track allocation pipeline.
- Fully offline operation on low-end Android; all interactions saved locally, with manual sync when internet returns.
- HQ can see all needs, stock levels, assignments, and allocation status after sync.
- CSV export of all tracking data (needs, aid inventory, allocations, status updates).
- Minimal UI: mobile-first, big buttons, minimal text, frictionless flows for rapid coordination decisions.

**Out Of Scope (strictly):**  
- Field distribution tracking or individual team usage monitoring (V2+ future phases).
- Equipment tracking, vehicle management, or secondary logistics coordination.
- Advanced analytics, reporting dashboards beyond basic planning exports.
- Integration with existing disaster management systems or databases.
- Multi-organization or inter-agency coordination features.

**V1 Additions (Week 2):**  
- Needs aggregation & planning: Cross-area analysis, resource gap identification, routing optimization.
- Advanced allocation: Batch allocations, conditional assignments, priority escalation automation, allocation history audit trail.
- Fulfillment tracking: Monitor allocation completion rates, identify persistent unmet needs.

**Timeline:**  
- V0 live in 1 week. V1 (aggregation, optimization, advanced allocation) in week 2 max.

**Field Constraints:**  
- App works with no internet. Data sync is user-triggered and robust to network failures.
- Designed for team training time = zero. Single screen for almost all actions.
- Must not break with partial info or bad inputs — always save a needs record or allocation, even if optional fields are missing.

**Success =**  
Faster, more reliable relief coordination: complete visibility of community needs across all affected areas, accurate aid inventory tracking, efficient allocation matching, and clear allocation plans for field distribution teams.