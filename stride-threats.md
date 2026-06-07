# STRIDE Threat Register - Solaris Care Connect 360

## Spoofing Threats

| ID | Threat | Component | Description | Severity |
|----|--------|-----------|-------------|----------|
| S1 | Credential Theft | Auth Service | Attacker obtains patient credentials via phishing | High |
| S2 | Fake Doctor Accounts | Admin Portal | Attacker creates unauthorized doctor accounts | Critical |
| S3 | Token Forgery | API Gateway | API requests made with stolen/forged JWT tokens | High |
| S4 | MITM on Insurance | External API | Man-in-the-middle attack on insurance provider API | Medium |
| S5 | Lab Result Spoofing | Lab Integration | Fake lab results injected into system | Critical |

## Tampering Threats

| ID | Threat | Component | Description | Severity |
|----|--------|-----------|-------------|----------|
| T1 | Record Modification | Patient Records | Unauthorized changes to patient medical records | Critical |
| T2 | Prescription Alteration | Rx Service | Changing drug dosages or medications | Critical |
| T3 | Audit Log Tampering | Audit Service | Deleting or modifying audit trails | High |
| T4 | Claims Manipulation | Insurance API | Modifying insurance claim amounts | High |
| T5 | Vitals Data Tampering | Monitoring | Altering real-time vital signs data | Critical |


## Repudiation Threats
| ID | Threat | Component | Description | Severity |
|----|--------|-----------|-------------|----------|
| R1 | Prescription Denial | Rx Service | Doctor denies approving a prescription | High |
| R2 | Record Access Denial | Patient Records | Patient denies accessing their records | Medium |
| R3 | Permission Change Denial | Admin Dashboard | Admin denies changing user permissions | High |
| R4 | Claims Denial | Insurance API | Insurance denies receiving a claim | Medium |
| R5 | Data Export No Audit | Patient Records | Lack of audit trail for data exports | High |

## Information Disclosure Threats
| ID | Threat | Component | Description | Severity |
|----|--------|-----------|-------------|----------|
| I1 | SQL Injection | Patient Records | Patient records exposed via SQL injection | Critical |
| I2 | API Over-exposure | API Gateway | API returns excessive data in responses | High |
| I3 | Error Message Leakage | All Services | Error messages reveal system internals | Medium |
| I4 | Unencrypted Transit | All Services | Unencrypted data in transit | Critical |
| I5 | Backup Exposure | Document Storage | Backup files accessible without authentication | Critical |
| I6 | PHI in Logs | All Services | PHI leaked in application logs | High |

## Denial of Service Threats
| ID | Threat | Component | Description | Severity |
|----|--------|-----------|-------------|----------|
| D1 | DDoS | API Gateway | DDoS attack on API Gateway | Critical |
| D2 | DB Exhaustion | Patient Database | Database exhaustion via expensive queries | High |
| D3 | Storage Exhaustion | Document Storage | Storage exhaustion via file uploads | Medium |
| D4 | Account Lockout | Auth Service | Account lockout attack on patient accounts | High |
| D5 | Resource Exhaustion | Rx Service | Resource exhaustion via prescription processing | Medium |

## Elevation of Privilege Threats
| ID | Threat | Component | Description | Severity |
|----|--------|-----------|-------------|----------|
| E1 | Patient Escalation | Auth Service | Patient escalates to doctor privileges | Critical |
| E2 | Doctor Escalation | Admin Dashboard | Doctor gains admin access | Critical |
| E3 | SQL Injection EoP | Patient Database | SQL injection leads to database admin | Critical |
| E4 | Container Escape | Infrastructure | Container escape to host system | Critical |
| E5 | IDOR | Patient Records | IDOR allows access to other patients records | High |
