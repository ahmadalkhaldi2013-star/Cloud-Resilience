---
layout: default
title: Welcome to Cloud Resilience
---

# Cloud Resilience

📂 **Topic area** in *Resilient Systems*.  
Action-oriented guidance to design workloads that **survive failures and recover fast**.

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

**Goal:** Provide a clear framework to **evaluate, design, and operate workloads** that can survive failure and recover fast.
