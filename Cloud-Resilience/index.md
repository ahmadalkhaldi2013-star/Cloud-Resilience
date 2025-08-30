---
layout: default
title: Welcome to Cloud Resilience
---

# Cloud Resilience

📂 **Topic area** in *Resilient Systems*.  
Action-oriented guidance to design workloads that **survive failures and recover fast**.

**What this is**
- Patterns, checklists, and diagrams with clear **Action** lines.
- Cloud-agnostic principles illustrated with **AWS terminology** (widely used).

**What this is not**
- Not vendor docs or step-by-step Terraform/CloudFormation.
- Not implementation code. Use these patterns to guide design and reviews.

---

## How to use this topic
- Skim each section, then copy the **Action** lines into runbooks / review checklists.
- Use the diagrams to explain fault boundaries to teammates.
- Map terms to your cloud (table below) and adjust examples accordingly.

---

## AWS terms → cross-cloud mapping

| Concept / Function        | AWS                         | Azure                               | GCP                          |
|---------------------------|-----------------------------|-------------------------------------|------------------------------|
| Failure domain            | **Availability Zone (AZ)**  | Availability Zone                    | Zone                         |
| Virtual machine           | **EC2**                     | Virtual Machines                     | Compute Engine VM            |
| Serverless function       | **Lambda**                  | Azure Functions                      | Cloud Functions              |
| Load balancer (L4/L7)     | **NLB / ALB**               | Load Balancer / Application Gateway  | Cloud Load Balancing         |
| Object storage            | **S3**                      | Blob Storage                         | Cloud Storage                |
| DNS                       | **Route 53**                | Azure DNS                            | Cloud DNS                    |
| Private network           | **VPC**                     | Virtual Network (VNet)               | VPC                          |
| **Queueing**              | **SQS**                     | Storage Queues / Service Bus **Queue** | Pub/Sub (pull subscribers) |
| **Pub/Sub events**        | **SNS** / EventBridge       | Service Bus **Topics** / Event Grid  | Pub/Sub (push & pull)        |

> Note: products don’t line up 1:1—choose the closest managed primitive to implement the **pattern**.

**Action:** If you’re not on AWS, replace labels in diagrams/checklists with your equivalents and keep the **principles**.

---

## 📖 Start Here
- [Resilience in the Cloud](resilience-in-the-cloud.md)
- [Resilience Analysis Framework](resilience-analysis-framework.md)
- [Fault Isolation & Static Stability](fault-isolation-core-concepts.md)

---

## Notes on diagrams
- Diagrams use **Mermaid**. They render on this site; in GitHub’s raw Markdown you may see the code fence—expected.
- Copy/paste and adapt diagrams in your design docs and reviews.

---

## Contribute
Real-world examples, corrections, or better diagrams are welcome.  
**Action:** Open an Issue/PR on GitHub with context and what changed.

---

## Audience

**Primary**
- Cloud / Solution Architects
- Site Reliability Engineers (SREs)
- Platform / DevOps Engineers

**Also useful for**
- Backend & Feature Engineers (owning services in prod)
- Tech Leads & Engineering Managers (reviewing designs/runbooks)
- Security/Compliance & Risk (failure modes, controls)
- Data/ML Platform Engineers (pipelines, state, recovery)
- Incident Commanders & On-call Responders
- QA / Performance Engineers (failure & load test planning)

**How to use by role**
- *Architects*: adopt patterns, fault boundaries, and **Action** checklists in design reviews.
- *SRE/Platform*: turn **Action** lines into runbooks, SLOs, chaos & DR tests.
- *Developers*: map diagrams to your service, swap AWS terms for your cloud, and add to service READMEs.
- *Leads/Managers*: use sections as acceptance criteria for design docs and launch reviews.

**Prereqs**
- Working knowledge of cloud primitives (compute, storage, networking) and basic IaC.
- AWS terms are used for examples; map to your cloud using the table above.

**Goal:** Provide a clear framework to **evaluate, design, and operate workloads** that can survive failure and recover fast.
