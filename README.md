# Resilient Systems

*A practical handbook for system design, reliability engineering, and resilience in production.*

- **Resilience:** fault isolation, static stability, multi-AZ/region, recovery
- **System Design:** architecture patterns, tradeoffs, scaling, data flows
- **Reliability (SRE):** SLIs/SLOs, incident response, runbooks, chaos drills


# Resilient Systems

Action-oriented guidance for designing **reliable, resilient, and well-operated systems**.  
Patterns over products. Actions over theory.

🔗 **Live site:** https://ahmadalkhaldi2013-star.github.io/Resilient-Systems/

---

## Start here

- **Cloud Resilience** → Fault isolation, static stability, AZ independence, recovery actions.  
  https://ahmadalkhaldi2013-star.github.io/Resilient-Systems/Cloud-Resilience/

> Each guide ends with clear **Action:** lines you can paste into design reviews and runbooks.

---

## Why this exists

For 15+ years I saved hard-won notes to external drives and left them in desk drawers—rarely revisited, and no one else learned from them.  
**This repo is my public notebook** so others can use (and improve) the checklists, patterns, and diagrams I wish I’d had.

---

## What you’ll find (topics)

- **Cloud Resilience** — fault isolation, static stability, AZ independence, recovery patterns.
- **System Design** — scalability, consistency/state, backpressure, latency budgets. *(coming soon)*
- **Reliability Engineering (SRE)** — SLOs, error budgets, incident response, post-incident learning. *(coming soon)*
- **Architecture Patterns** — queues vs pub/sub, idempotency, circuit breakers, bulkheads, retries/backoff.
- **Testing & Chaos** — load tests, dependency failure drills, game days, DR runbooks.
- **Ops Playbooks** — rollout/rollback, safe deploys, on-call ready. *(coming soon)*

Everything is **cloud-agnostic**, often illustrated with **AWS terminology** (widely recognized).  
Diagrams are **Mermaid** (render on GitHub and on the site).

---

## Who this is for

- Cloud / Solution **Architects**
- **SREs** and Platform / DevOps Engineers
- Backend Engineers who own services in prod
- Tech Leads & Engineering Managers

---

## What this is / is not

**This is**
- Principles, patterns, diagrams, and **Action:** checklists.
- Cloud-agnostic content with AWS examples for familiarity.

**This is not**
- Vendor documentation or copy-paste Terraform/CloudFormation.
- Implementation code—use these patterns to guide **design** and **operations**.
