# FieldTrack — Technical One-Pager

**Purpose:**  
Rapid, field-ready system to track relief item distribution to affected communities during hurricane response. MVP must ship in 1 week; strict focus on supplies setup, assignment, field logging, sync, and CSV export.

**What Is Tracked:**  
Only relief items (food, water, hygiene, medical) — not tools, radios, or general equipment. Each “item” is always a supply unit intended for distribution to beneficiaries.

**Main Users & Roles:**  
- **HQ/Admin:** Enters and assigns stock (by item, quantity, batch/lot if needed).
- **Field Team Lead:** Updates status, logs distributions in real time; operates offline when needed.
- **No extra roles, no analytics, no integration — just get relief item data in/out, fast.**

**Core Features (MVP/V0):**  
- Relief item registry: Add/view/edit item details (name, type, quantity, optionally batch).
- Assign stock to a field team or distribution event.
- Simple field interface for updating how much of each item was actually distributed (count), with timestamp and team.
- Fully offline operation on low-end Android; all interactions saved locally, with manual sync when internet returns.
- HQ can see current stock, team assignments, and logs after sync.
- CSV export of all tracking data (items, assignments, distributions, logs).
- Minimal UI: mobile-first, big buttons, minimal text, frictionless flows.

**Out Of Scope (strictly):**  
- Anything related to equipment, complex reporting, advanced permissions, analytics, integrations, or “nice to have” features.
- No maps, no beneficiary-level tracking (just team/event-level for speed).

**Timeline:**  
- V0 live in 1 week. V1 (field-driven improvements, with partial use logging and admin override) in week 2 max.

**Field Constraints:**  
- App works with no internet. Data sync is user-triggered and robust to network failures.
- Designed for team training time = zero. Single screen for almost all actions.
- Must not break with partial info or bad inputs — always log a distribution, even if “batch” or “category” is missing.

**Success =**  
Faster, more reliable relief supply accountability for each team/event (what was sent, where it went, what was distributed, and when).