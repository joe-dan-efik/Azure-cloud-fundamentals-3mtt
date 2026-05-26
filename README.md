# Azure Cloud Infrastructure Fundamentals
Mini project-1
##  Project Overview
This project provides a foundational practical introduction to cloud computing through the setup and configuration of a Microsoft Azure environment. It demonstrates transitioning from theoretical cloud concepts to hands-on application—establishing a functional cloud environment, exploring enterprise governance interfaces, and reviewing the operational frameworks utilized in standard cloud management setups.

---

##  Project Goals
* Establish a functional cloud footprint using the **Azure Free Tier**.
* Gain navigational proficiency within the Azure Portal and its management directories.
* Understand foundational cloud governance structures (Subscriptions & Resource Groups).
* Review cloud Identity & Access Management (IAM) and Role-Based Access Control (RBAC).
* Analyze cost management frameworks, regional latency, and the Shared Responsibility Model.

---

## 🛠️ Infrastructure Documentation & Verification

### 1. Active Subscription Verification
Demonstration of an active Azure platform identity with full administrative permissions and the core Free Tier credits applied.
* **Subscription Name:** `Azure subscription 1`
* **Role:** `Owner`
* **Status:** `Active`

![Active Subscription](./01_active_subscription.png)

---

### 2. Governance Layout (Resource Group)
Creation of a dedicated logical container to manage resource lifecycles and deployments safely.
* **Resource Group Name:** `azure-fundamentals-mini-project-1`

![Resource Group](./02_resource_group.png)

---

### 3. Cost Management Configuration
Verification of active access to the Cost Analysis and Budgets plane to ensure continuous tracking and proactive threshold alerts.

![Cost Management](./04_cost_management.png)

---

## 📄 Summary Report

### 🗺️ 1. Region Selection & Latency Optimization
* **Primary Regional Choice:** `East US`
* **Technical Rationale:** The **East US** region was selected as the deployment target for this project. As a major flagship hub for Microsoft Azure, East US provides comprehensive service availability, immediate access to foundational cloud offerings, and optimal pricing tiers for the Free Tier track. Additionally, it offers stable routing and competitive network latencies across global transit lines.
* **High Availability Architecture:** The East US region guarantees a minimum layout of **3 distinct Availability Zones (AZs)**. Each zone is comprised of one or more physical datacenters equipped with completely independent power, cooling, and network infrastructure. This ensures that infrastructure deployed across these zones remains resilient and fault-tolerant against localized datacenter failures.

### 🛡️ 2. Shared Responsibility Model Application
The Shared Responsibility Model outlines the explicit security boundaries between Microsoft Azure and the account user. 

For the resources explored during this environment setup:
* **Microsoft's Responsibility:** Microsoft maintains absolute control over the physical infrastructure layer. This includes the physical security of the datacenter facilities (guards, biometric access), server hardware lifecycle management, host hypervisor integrity, underlying network switch operations, and environmental infrastructure (cooling and power grid backup resilience).
* **My Responsibility:** I retain full ownership of the configuration and data deployed *within* the tenant. This includes managing subscription-level permissions, implementing Identity security through Microsoft Entra ID boundaries (RBAC assignments), enforcing proper naming conventions, setting up cost alert thresholds, and ensuring that any deployed resources are not left exposed to the public internet through misconfigured network security policies.
