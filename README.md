# Threat Model — Solaris Care Connect 360

A comprehensive security threat model for a healthcare platform managing 50,000 patient records, completed as part of the DevSecAI Threat Modelling Workshop.

## Overview

**Platform:** Solaris Care Connect 360 (Healthcare SaaS)
**Scope:** Patient mobile app, doctor portal, admin dashboard, backend APIs, database layer, external integrations
**Methodology:** STRIDE, MITRE ATT&CK, Cyber Kill Chain, NIST CSF

## Key Findings

| Severity | Count | Examples |
|----------|-------|---------|
| Critical | 2 | SQL Injection (I1), Credential Phishing (S1) |
| High | 4 | SQLi to DBA (E3), Privilege Escalation (E1) |
| Medium | 2 | DDoS (D1), Repudiation (R1) |

## Repository Structure

- diagrams/ — architecture.md, architecture2.md, dfd-level0.md, dfd-level1.md, attack-trees.md
- reports/ — threat-model-report.md
- templates/ — stride-threats.md, mitre-mapping.md, kill-chain-analysis.md, risk-register.md, control-mapping.md

## Top Risks

1. **SQL Injection (I1)** — Score 20/25 — Immediate WAF deployment required
2. **Credential Phishing (S1)** — Score 16/25 — MFA rollout urgently needed
3. **SQLi to DBA (E3)** — Score 15/25 — Database privilege review required

## Immediate Actions

- [ ] Deploy Web Application Firewall (WAF)
- [ ] Implement MFA for all user types
- [ ] Review and restrict database account privileges

## Skills Demonstrated

- STRIDE threat categorisation
- MITRE ATT&CK mapping
- Cyber Kill Chain analysis
- Risk scoring (Likelihood × Impact)
- NIST CSF control mapping
- Attack tree development
- Professional security documentation

---
*Part of the DevSecAI Bootcamp — Project 3: Threat Modelling Workshop*
