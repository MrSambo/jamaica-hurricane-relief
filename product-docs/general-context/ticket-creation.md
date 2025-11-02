# 🧾 Technical Ticket Creation Guidelines

## 🎯 Purpose

This document defines the **standards and structure** for creating technical tickets. It ensures that every ticket generated — whether by an agent or AI — is **actionable**, **technically complete**, and **aligned with team processes**.

---

## 🧱 Ticket Structure

Each ticket must include the following sections in the **Description** field.

### 1. Title
- Must clearly summarize the task or issue.
- Use **imperative form** (e.g., “Implement”, “Refactor”, “Fix”, “Update”).
- Example:  
  - ✅ `Refactor user authentication middleware for JWT support`  
  - ❌ `Authentication issue`  

---

### 2. Context
Briefly describe **why** this ticket exists. Include relevant background, the system or component affected, and any known dependencies.

> Example:  
> The current authentication middleware only supports session tokens.  
> The API now requires JWT authentication for all user-facing endpoints.

---

### 3. Objective
Define **what needs to be achieved**. This should be a clear technical goal or outcome.

> Example:  
> Implement JWT-based authentication and ensure backward compatibility with session tokens.

---

### 4. Technical Requirements
List specific **implementation details or constraints**. Focus on what must be built, changed, or configured.

> Example:  
> - Introduce JWT signing and verification using the shared secret.  
> - Update `authService.ts` to issue JWT tokens on login.  
> - Modify API gateway to validate JWTs.  
> - Update Postman tests to reflect new headers.

---

### 5. Acceptance Criteria
These are **verifiable conditions** that must be met for the ticket to be accepted. They should describe **expected results** rather than steps.

> Example:  
> - [ ] API endpoints successfully authenticate using JWT.  
> - [ ] Legacy session tokens remain valid for existing clients.  
> - [ ] All automated tests pass.  
> - [ ] Peer review completed and approved.

---

### 6. Definition of Done (DoD)
The **Definition of Done** applies universally to all technical tickets, ensuring consistency and quality. Each ticket must satisfy these before it can be closed.

> Example:  
> - [ ] All Acceptance Criteria are met.  
> - [ ] Code reviewed and merged into the main branch.  
> - [ ] Unit/integration tests updated and passing.  
> - [ ] Relevant documentation updated (e.g., README, API specs, configs).  
> - [ ] Deployment verified in staging environment.  
> - [ ] Ticket status updated to “Done” with final notes.

---

### 7. References / Attachments
Include any relevant:
- Log files, screenshots, or error traces.
- Links to related tickets, pull requests, or documentation.
- API endpoints, environment names, or service identifiers.

> Example:  
> - Related PR: `#452 - JWT Middleware Implementation`  
> - API Spec: `/auth/v2/openapi.yaml`

---

## 🧩 Ticket Metadata

When creating tickets, include the following metadata:

| Field | Description | Example |
|-------|--------------|----------|
| **Type** | Bug / Feature / Improvement / Refactor | Feature |
| **Priority** | Low / Medium / High / Critical | High |
| **Component / Module** | System or service affected | `Auth Service` |
| **Tags** | Tech or project keywords | `backend`, `auth`, `security` |
| **Assignee** | Leave blank — assigned by PMO or Tech Lead | — |
| **Due Date** | Optional unless specified | 2025-11-10 |

---

## ⚙️ Workflow for Automated / Agent Ticket Creation

1. **Gather Input:**  
   - Review request context or change description.  
   - Extract technical details (systems, dependencies, requirements).

2. **Generate Ticket:**  
   - Create using the above structure.  
   - Ensure Acceptance Criteria and DoD are clearly written.

3. **Validate Completeness:**  
   - Check that each section (Context → DoD) is filled.  
   - Confirm ticket is unambiguous and technically actionable.

4. **Submit to Review:**  
   - Reviewed by the Tech Lead before being assigned.

---

## 🧠 Quality Standards for AI / Agents

When creating tickets automatically:

- Maintain **technical precision** — use domain terms accurately.  
- Avoid vague language like “fix issue” or “make it better.”  
- Always include **verifiable Acceptance Criteria** and **Definition of Done**.  
- Use Markdown checkboxes (`- [ ]`) for checklist items.  
- Reference impacted services, repos, or files when known.

---

## ✅ Example Ticket

**Title:**  
Implement JWT-based authentication in API Gateway

**Description:**
```
### Context
Current API Gateway authenticates users via legacy session tokens.
We need to migrate to JWT authentication for consistency across services.

### Objective
Enable JWT-based authentication and maintain backward compatibility.

### Technical Requirements
- Introduce JWT verification middleware.
- Update auth service to issue JWT tokens on login.
- Update configuration to use shared secret from Vault.
- Modify Postman test collection to include JWT header.

### Acceptance Criteria
- [ ] All API endpoints accept valid JWTs.
- [ ] Session tokens continue working for existing users.
- [ ] All tests pass in CI pipeline.
- [ ] Peer review completed.

### Definition of Done
- [ ] Code merged to `main`.
- [ ] Tests updated and passing.
- [ ] Documentation updated.
- [ ] Verified in staging.
- [ ] Ticket marked “Done” with final notes.

### References / Attachments
- Related PR: #452
- API Spec: /auth/v2/openapi.yaml
```

---

**End of Document**

