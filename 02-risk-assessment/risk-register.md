# Risk Register: Hypothetical State Hospital

Scope and assumptions are in [01-scope-and-assumptions/scope-and-assumptions.md](../01-scope-and-assumptions/scope-and-assumptions.md). This is a portfolio exercise, and all ratings are illustrative.

## Rating method

- Likelihood: 1 (rare) to 5 (almost certain)
- Impact: 1 (minor) to 5 (severe)
- Score: likelihood x impact. 1-6 Low, 7-12 Medium, 13-25 High
- Safeguard type follows the HIPAA Security Rule: Administrative, Physical, or Technical
- Method follows the approach in NIST SP 800-30

## Register

| ID | Risk | Asset | Safeguard | L | I | Score | Rating | Treatment | Owner |
|----|------|-------|-----------|--:|--:|------:|--------|-----------|-------|
| R01 | Tailgating or propped doors let an unauthorized person into patient areas | Doors and patient areas | Physical | 4 | 4 | 16 | High | Door alarms for held-open doors, staff reminders, regular door audits | Security Director |
| R02 | Lost, unreturned, or duplicated keys and badges | Keys and badges | Physical | 4 | 3 | 12 | Medium | Key and badge inventory, immediate deactivation of lost badges, periodic re-keying | Facilities Manager |
| R03 | Prohibited items enter the facility through visitors or deliveries | Patients and staff | Physical | 3 | 5 | 15 | High | Visitor screening, clear rules posted at check-in, supervised special visits | Security Director |
| R04 | Staff look at patient records without a work reason | Electronic health record | Technical | 4 | 4 | 16 | High | Role-based access, access logging, regular audit of who opened which records | Privacy Officer |
| R05 | Phishing of staff leads to stolen credentials | Staff accounts | Technical | 4 | 5 | 20 | High | MFA, email filtering, phishing awareness training | IT Security |
| R06 | Ransomware takes the health record system offline | Electronic health record | Technical | 3 | 5 | 15 | High | Tested offline backups, network segmentation, downtime procedures | IT Security |
| R07 | Vendor remote access is misused or goes unmonitored | Vendor accounts | Administrative | 3 | 5 | 15 | High | Time-limited vendor accounts, approval before each session, session logging | IT Security |
| R08 | Unpatched systems and devices are exploited | Servers, workstations, devices | Technical | 4 | 4 | 16 | High | Asset inventory, patch schedule, vulnerability scanning | IT Operations |
| R09 | Accounts and badges stay active after staff or contractors leave | Staff accounts and badges | Administrative | 3 | 4 | 12 | Medium | Offboarding checklist, same-day removal, quarterly access review | HR and IT Security |
| R10 | Paper records or printouts are left unsecured | Paper records | Physical | 3 | 3 | 9 | Medium | Locked storage, clean-desk rule, secure shredding | Privacy Officer |
| R11 | An incident is not reported or escalated because of unclear steps or a missed handoff | Incident records | Administrative | 3 | 4 | 12 | Medium | Written incident procedure, standard shift handoff form, supervisor review | Security Director |
| R12 | Staff are not trained on security and privacy duties | Workforce | Administrative | 3 | 3 | 9 | Medium | Annual training, training at hire, completion tracking | Compliance Officer |

## Summary

- High: 7 risks (R01, R03, R04, R05, R06, R07, R08)
- Medium: 5 risks (R02, R09, R10, R11, R12)
- Low: none at this stage
- By safeguard type: 4 Physical, 4 Technical, 4 Administrative
