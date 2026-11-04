# Control Mapping: Risks and Policies to HIPAA and NIST CSF 2.0

This maps each risk in [02-risk-assessment/risk-register.md](../02-risk-assessment/risk-register.md) to the HIPAA Security Rule, to NIST CSF 2.0, and to the policy statements in [03-policies](../03-policies/) that address it. It is a portfolio exercise for a hypothetical hospital, not an audit and not legal advice.

## How to read this

- **Covered:** a policy statement directly addresses the risk.
- **Partial:** a policy addresses part of the risk, and something is still missing.
- **Gap:** no policy addresses the risk yet.
- Policy references use the policy name and statement number. For example, "Physical 7" means statement 7 of the Physical Access Control Policy.

## Mapping

| Risk | Risk summary | HIPAA Security Rule | NIST CSF 2.0 | Addressed by | Coverage |
|------|--------------|---------------------|--------------|--------------|----------|
| R01 | Tailgating or propped doors | 164.310(a)(1) facility access controls; 164.310(a)(2)(iii) access control and validation | PR.AA-06 physical access managed | Physical 6, 7; Visitor 6, 9 | Covered |
| R02 | Lost, unreturned, or duplicated keys and badges | 164.310(a)(1) facility access controls; 164.310(a)(2)(iv) maintenance records | PR.AA-06 physical access managed | Physical 2, 3, 4, 5 | Covered |
| R03 | Prohibited items brought in by visitors or deliveries | 164.310(a)(1) facility access controls (safety control, not a direct HIPAA requirement) | PR.AA-06 physical access managed | Visitor 3, 4, 7, 8 | Covered |
| R04 | Staff view patient records without a work reason | 164.308(a)(4) information access management; 164.312(a)(1) access control; 164.312(b) audit controls | PR.AA-05 access permissions; DE.CM-03 personnel activity monitored | Physical 11 covers badge logs only, not record access | Gap |
| R05 | Phishing of staff leads to stolen credentials | 164.308(a)(5) security awareness and training; 164.312(d) person or entity authentication | PR.AT-01 awareness and training; PR.AA-03 authentication | None | Gap |
| R06 | Ransomware takes the health record system offline | 164.308(a)(7) contingency plan | PR.DS-11 backups; RC.RP-01 recovery plan executed | None | Gap |
| R07 | Vendor remote access misused or unmonitored | 164.308(b)(1) business associate contracts; 164.312(a)(1) access control | GV.SC-05 supply chain requirements; GV.SC-07 supplier risk monitored | Physical 9 covers contractor badges and escorts, not remote access | Partial |
| R08 | Unpatched systems and devices exploited | 164.308(a)(1)(ii)(A) risk analysis; 164.308(a)(1)(ii)(B) risk management | ID.AM-01 hardware inventory; PR.PS-02 software maintained | None | Gap |
| R09 | Accounts and badges stay active after people leave | 164.308(a)(3)(ii)(C) termination procedures | PR.AA-01 identities and credentials managed; PR.AA-05 access reviewed | Physical 8, 10 cover badges, not system accounts | Partial |
| R10 | Paper records or printouts left unsecured | Privacy Rule 164.530(c) safeguards; 164.310(d)(1) device and media controls | PR.DS-01 data at rest protected | None | Gap |
| R11 | Incident not reported or escalated | 164.308(a)(6) security incident procedures | RS.MA-01 incident response plan executed; RS.CO-02 stakeholders notified | Physical 11, 12 and Visitor 10 touch on it, but no reporting procedure exists | Partial |
| R12 | Staff not trained on security and privacy duties | 164.308(a)(5) security awareness and training | PR.AT-01 awareness and training | None | Gap |

## Coverage summary

- Covered: 3 risks (R01, R02, R03), all physical security
- Partial: 3 risks (R07, R09, R11)
- Gap: 6 risks (R04, R05, R06, R08, R10, R12)

The two policies cover physical and visitor access well. Most of the technical and administrative risks still need policies.

## Gaps and next steps

1. **Information access and audit policy** (R04, and the accounts side of R09): role-based record access, regular review of who opened which records, and removal of system accounts when people leave.
2. **Security awareness and training policy** (R05, R12): training at hire and every year, phishing reminders, and completion tracking.
3. **Incident response policy** (R11): how to report, escalate, and review an incident.
4. **Contingency and backup plan** (R06): tested backups and downtime procedures.
5. **Patch and asset management policy** (R08): device inventory and a patch schedule.
6. **Vendor remote access procedure** (R07): approval, time limits, and logging for each session.
7. **Paper records handling** (R10): locked storage, a clean-desk rule, and secure shredding.

## References

- HHS, HIPAA Security Rule summary: https://www.hhs.gov/hipaa/for-professionals/security/index.html
- NIST Cybersecurity Framework 2.0: https://www.nist.gov/cyberframework
