# Zero Trust Architecture & Microsegmentation Posture Reviewer

<p align="center">
  <img src="https://img.shields.io/badge/Security-Defensive_Auditor-blue?style=flat" alt="Type">
  <img src="https://img.shields.io/badge/Status-Architectural_Showcase-success?style=flat" alt="Status">
  <img src="https://img.shields.io/badge/Python-3.10+-3776AB?style=flat&logo=python&logoColor=white" alt="Python">
</p>

> 🔒 **Technical Showcase & Architecture Specification**  
> *This repository provides public architectural documentation, system specifications, and implementation summaries. Full production source code, internal test suites, and proprietary algorithms are maintained in a secure private repository.*

---

## 📌 Executive Summary

**Category**: Zero Trust Architecture  
**Tech Stack**: `Python 3.10+ · NIST SP 800-207 · Zero Trust Architecture · Microsegmentation`  

Deterministic audit engine evaluating enterprise network, identity, and workload controls against NIST SP 800-207 Zero Trust Architecture principles.

---

## 🎯 The Problem It Solves

Organizations frequently claim 'Zero Trust' without validating whether implicit network trust has actually been eliminated. Objective, deterministic evidence review is required.

---

## ⚙️ How the Engine Works

1. **Evidence Input Parsing**: Ingests structured posture evidence across the 7 NIST Zero Trust pillars (User, Device, Network, Workload, Data, Visibility, Automation).
2. **Implicit Trust Detection**: Scans network and application configs for implicit trust assumptions (e.g. allowing unauthenticated traffic simply because it originates from internal IP subnets).
3. **Continuous Verification Check**: Audits session token lifetimes, continuous posture evaluation hooks, and step-up authentication policies.
4. **Microsegmentation Analysis**: Validates whether workloads communicate through mutual TLS (mTLS) with strict service-to-service authorization or flat internal networks.
5. **Maturity Scoring**: Outputs a NIST 800-207 maturity score and prioritized gap remediation roadmap.

---

## 🚀 Key Capabilities

- Evaluates enterprise architectures against NIST SP 800-207 Zero Trust standards
- Identifies flat network designs and implicit internal IP trust vulnerabilities
- Audits mTLS service-to-service segmentation and device posture verification
- Generates comprehensive Zero Trust maturity reports for leadership

---

## 🏗️ System Data Flow & Architecture

```
+-----------------------------------+
|  Target Input / Configuration    |
|  (JSON Snapshots / Policies)      |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  1. Schema Normalization Engine   |
|  Validates types & formats        |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  2. Core Analytical Pipeline      |
|  Heuristic rule evaluation,       |
|  invariant checks & drift diffs   |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  3. Risk Classification           |
|  Assigns severity: INFO / HIGH    |
+-----------------+-----------------+
                  |
                  v
+-----------------------------------+
|  4. Structured Findings & Report  |
|  Root cause, evidence &           |
|  actionable remediation steps     |
+-----------------------------------+
```

---

## 📄 Findings Output Structure

The engine generates structured, machine-parsable JSON reports adhering to this standard audit schema:

```json
{
  "results": [
    {
      "resource": "resource-identifier",
      "severity": "HIGH",
      "check": "CHECK_IDENTIFIER",
      "detail": "Descriptive analysis of the identified security posture issue.",
      "remediation": "Actionable step-by-step guidance to restore compliant state.",
      "evidence": {
        "observed_field": "value",
        "required_policy": "enforced_policy"
      }
    }
  ],
  "count": 1,
  "scope": "Comprehensive defensive security audit"
}
```

---

## 🔒 Source Code & Enterprise Inquiries

To protect proprietary intellectual property and client operational security:
* **Public Repository**: Contains comprehensive architecture specifications, schemas, and design overviews.
* **Private Repository**: Contains the complete production implementation, continuous integration pipelines, and full regression test suites.

For architectural questions or enterprise inquiries, connect via [LinkedIn](https://www.linkedin.com/in/karthikeyansubramaniam04/) or visit the [Portfolio Site](https://karthikeyansubramaniyam.github.io).
