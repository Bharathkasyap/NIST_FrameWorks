# 🛡️ NIST Frameworks for SOC Analysts – Complete Reference Guide

> **Purpose:** This Markdown file serves as a **one-stop GitHub page** to help SOC (Security Operations Center) analysts understand, reference, and apply the **most critical NIST (National Institute of Standards and Technology) frameworks and publications** used in cybersecurity monitoring, detection, response, and risk handling.

---

## 📚 Table of Contents

1. [What is NIST?](#what-is-nist)
2. [Why NIST is Important for SOC Analysts](#why-nist-is-important-for-soc-analysts)
3. [Top NIST Standards Every SOC Analyst Should Know](#top-nist-standards-every-soc-analyst-should-know)
4. [Detailed Breakdown of Each NIST Framework](#detailed-breakdown-of-each-nist-framework)
   - [NIST SP 800-61 (Computer Security Incident Handling Guide)](#1-nist-sp-800-61)
   - [NIST SP 800-53 (Security and Privacy Controls)](#2-nist-sp-800-53)
   - [NIST SP 800-171 (Protecting CUI)](#3-nist-sp-800-171)
   - [NIST CSF (Cybersecurity Framework)](#4-nist-cybersecurity-framework-csf)
   - [NIST SP 800-115 (Technical Guide to Security Testing)](#5-nist-sp-800-115)
   - [NIST SP 800-137 (Information Security Continuous Monitoring - ISCM)](#6-nist-sp-800-137)
   - [NIST SP 800-30 (Risk Assessments)](#7-nist-sp-800-30)
   - [NIST SP 800-92 (Log Management)](#8-nist-sp-800-92)
5. [NIST Controls Mapping for Daily SOC Tasks](#nist-controls-mapping-for-daily-soc-tasks)
6. [Tools, Policies, and Documents NIST Aligns With](#tools-policies-and-documents-nist-aligns-with)
7. [External References](#external-references)

---

## 🏛️ What is NIST?

**NIST (National Institute of Standards and Technology)** is a U.S. government agency that develops and publishes cybersecurity frameworks, guidelines, and standards to help organizations manage and reduce cybersecurity risks.

---

## 🔍 Why NIST is Important for SOC Analysts

| Benefit                         | Description                                                                 |
|--------------------------------|-----------------------------------------------------------------------------|
| **Compliance**                 | Helps meet legal and industry standards like FISMA, FedRAMP, DFARS         |
| **Consistency**                | Provides unified language and structure for cybersecurity                   |
| **Incident Response**          | Offers structured procedures to identify, detect, respond, and recover     |
| **Audit Readiness**            | Ensures proper documentation and log retention practices                    |
| **Continuous Improvement**     | Enables SOC teams to benchmark, tune, and mature their detection program   |

---

## 🔝 Top NIST Standards Every SOC Analyst Should Know

| NIST Publication     | Focus Area                                     | Why It Matters to SOC Analysts                                 |
|----------------------|------------------------------------------------|----------------------------------------------------------------|
| SP 800-61 Rev. 2     | Incident Response                              | IR lifecycle, detection, containment, eradication              |
| SP 800-53 Rev. 5     | Security & Privacy Controls                    | Full catalog of controls used in audits and defense programs   |
| SP 800-171 Rev. 2    | Protection of CUI in Non-Federal Systems       | Especially important for federal contractors                   |
| NIST CSF             | Cybersecurity Risk Management Framework        | Baseline model used by all industries                          |
| SP 800-115           | Penetration Testing & Technical Assessments    | Important for purple teams and attack simulation               |
| SP 800-137           | Continuous Monitoring                          | Aligns with SOC alert tuning and threat monitoring             |
| SP 800-30            | Risk Assessments                               | Used during threat modeling and risk scoring                   |
| SP 800-92            | Log Management                                | Establishes guidelines for logging and retention policies      |

---

## 🔬 Detailed Breakdown of Each NIST Framework

> 📎 **Click the titles below to open official NIST documentation for each framework.**

### 1. [NIST SP 800-61 – *Computer Security Incident Handling Guide*](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf) – *Computer Security Incident Handling Guide*

| Section            | Key Concepts                                                                 |
|--------------------|------------------------------------------------------------------------------|
| Preparation         | Roles, response policies, training, tools                                   |
| Detection & Analysis| Indicators of compromise (IoCs), classification, initial handling           |
| Containment         | Short-term (isolation), long-term (patch, update) strategies                |
| Eradication & Recovery | Malware removal, credential resets, backups                              |
| Post-Incident       | Lessons learned, root cause, documentation updates                          |

👉 This is the **most referenced guide** in IR workflows and SOC alert triage.

---

### 2. [NIST SP 800-53 – *Security and Privacy Controls*](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final) – *Security and Privacy Controls*

| Family         | Example Controls           | Purpose                                        |
|----------------|----------------------------|------------------------------------------------|
| AC (Access Control)       | AC-2, AC-6                     | Role-based access, least privilege             |
| AU (Audit & Accountability)| AU-2, AU-6                    | Logging and alert review practices             |
| IR (Incident Response)    | IR-4, IR-5                     | Incident handling, reporting, coordination     |
| SI (System Integrity)     | SI-4, SI-7                     | Malware defense, system monitoring             |

👉 Used in STIG checklists, SIEM alerts, and audit validations.

---

### 3. [NIST SP 800-171 – *Protecting Controlled Unclassified Information (CUI)*](https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final) – *Protecting Controlled Unclassified Information (CUI)*

| Control Family        | Use Case for SOC Analysts                                |
|-----------------------|----------------------------------------------------------|
| 3.3 Audit and Accountability | Log review, alert correlation, audit trails         |
| 3.14 System & Info Integrity | Malware detection, file integrity monitoring       |

👉 Common for contractors, DFARS/FedRAMP environments, and DoD work.

---

### 4. [NIST Cybersecurity Framework (CSF)](https://www.nist.gov/cyberframework)

| Function     | Description                                                   |
|--------------|---------------------------------------------------------------|
| Identify     | Asset management, risk assessments                            |
| Protect      | Access control, awareness training                            |
| Detect       | SIEM, endpoint detection, alerting                            |
| Respond      | Incident response planning, mitigation                        |
| Recover      | Backups, business continuity                                  |

👉 High-level framework aligned with business and board reporting.

---

### 5. [NIST SP 800-115 – *Technical Guide to Information Security Testing*](https://csrc.nist.gov/publications/detail/sp/800-115/final) – *Technical Guide to Information Security Testing*

- Covers **vulnerability scanning**, **red teaming**, **log review**, and **penetration testing**
- Helps define testing methodologies for internal audits
- SOCs use it to simulate and validate detection capabilities

---

### 6. [NIST SP 800-137 – *Information Security Continuous Monitoring (ISCM)*](https://csrc.nist.gov/publications/detail/sp/800-137/final) – *Information Security Continuous Monitoring (ISCM)*

- Explains how to **automate alerting, tuning SIEM**, and reduce false positives
- Used to build **dashboards and SOC metrics**
- Encourages integration with CDM (Continuous Diagnostics & Mitigation)

---

### 7. [NIST SP 800-30 – *Guide for Conducting Risk Assessments*](https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final) – *Guide for Conducting Risk Assessments*

| Phase         | SOC Application                                |
|---------------|-------------------------------------------------|
| Threat ID     | Create threat models for alert use cases       |
| Vulnerability Analysis | Align with CVE or scanner output         |
| Risk Likelihood & Impact | Used in prioritizing alert severity    |

---

### 8. [NIST SP 800-92 – *Guide to Computer Security Log Management*](https://csrc.nist.gov/publications/detail/sp/800-92/final) – *Guide to Computer Security Log Management*

| Focus Area        | Importance for SOC                                   |
|-------------------|-------------------------------------------------------|
| Log Generation     | Ensuring telemetry coverage across systems          |
| Log Normalization  | Making data usable for SIEM correlation             |
| Retention Policies | Enforcing compliance (HIPAA, PCI-DSS, etc.)         |
| Review Procedures  | Alerting on anomalies and suspicious sequences      |

---

## 🧩 NIST Controls Mapping for Daily SOC Tasks

| SOC Task                        | NIST Reference                     |
|---------------------------------|------------------------------------|
| Alert triage                    | SP 800-61 (Detection & Analysis)   |
| Patch verification              | SP 800-53 SI-2, SI-7               |
| Vulnerability scan handling     | SP 800-115                         |
| Log monitoring                  | SP 800-92                          |
| Risk scoring for alerts         | SP 800-30                          |
| Dashboarding/reporting          | SP 800-137                         |

---

## 🛠️ Tools, Policies, and Docs NIST Aligns With

- **SIEMs**: Microsoft Sentinel, Splunk, QRadar (used with SP 800-92 & SP 800-137)
- **EDR**: Defender for Endpoint, CrowdStrike, SentinelOne (SP 800-53 SI controls)
- **Incident Reports**: Written following SP 800-61
- **Vulnerability Reports**: Use SP 800-115 format
- **Compliance Programs**: HIPAA, FedRAMP, FISMA, NIST CSF, SP 800-53

---

## 🌐 External References

| Title                          | URL                                                                 |
|--------------------------------|----------------------------------------------------------------------|
| NIST Official Publications     | https://csrc.nist.gov/publications                                   |
| NIST SP 800-61 Guide           | https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf |
| NIST CSF Framework             | https://www.nist.gov/cyberframework                                  |
| NIST SP 800-53 Controls        | https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final       |
| NIST SP 800-171 (CUI)          | https://csrc.nist.gov/publications/detail/sp/800-171/rev-2/final      |
| NIST SP 800-137 ISCM           | https://csrc.nist.gov/publications/detail/sp/800-137/final            |
| NIST SP 800-30 Risk Guide      | https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final       |
| NIST SP 800-92 Logging Guide   | https://csrc.nist.gov/publications/detail/sp/800-92/final             |

---

> 🛠️ **Maintained by:** Bharath Kasyap | Cybersecurity Analyst  
> 🧠 **Contribution Welcome:** Pull requests to improve, add NIST references, or SOC tools mapping are encouraged.
