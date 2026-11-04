# Hospital GRC Portfolio

A governance, risk, and compliance (GRC) case study for a **hypothetical state psychiatric hospital**. It walks through the same steps a GRC analyst follows on a real engagement: define the scope, assess the risks, write policies, and map everything to HIPAA and NIST CSF 2.0 to see what is covered and what is missing.

The hospital in this project is a made-up composite. It is not based on any real facility, and nothing here describes a real organization's systems, staff, or incidents.

## What is in this repo

| Folder | What it contains |
|--------|------------------|
| [01-scope-and-assumptions](01-scope-and-assumptions/) | The hypothetical hospital, what is in and out of scope, and the assumptions behind the work |
| [02-risk-assessment](02-risk-assessment/) | A register of 12 risks, each scored on likelihood and impact |
| [03-policies](03-policies/) | Two policies: Visitor Access and Physical Access Control |
| [04-control-mapping](04-control-mapping/) | Each risk mapped to HIPAA, NIST CSF 2.0, and the policy that addresses it, with coverage gaps |

## Approach

1. **Scope.** Set the boundaries first: which systems, locations, and people are covered, and what is assumed.
2. **Assess risk.** Score each risk by likelihood and impact on a 1 to 5 scale, using the NIST SP 800-30 approach. Scores of 1 to 6 are Low, 7 to 12 are Medium, and 13 to 25 are High.
3. **Write policies.** Address the physical and visitor risks with clear, numbered statements that can be checked.
4. **Map controls.** Tie each risk to HIPAA Security Rule citations and NIST CSF 2.0 subcategories, then mark it Covered, Partial, or Gap.

## Key findings

- **12 risks were identified:** 7 High and 5 Medium. There are 4 physical, 4 technical, and 4 administrative risks.
- **The highest-rated risk is phishing (R05, score 20).** Stolen staff credentials could expose patient records.
- **Physical and visitor access are well covered.** The two policies fully address tailgating, lost keys and badges, and prohibited items.
- **Most technical and administrative risks still have no policy.** Of the 12 risks, 3 are Covered, 3 are Partial, and 6 are Gaps.
- **The control mapping ends with a prioritized list of seven policies to write next**, including information access and audit, security awareness training, and incident response.

## Frameworks used

- HIPAA Security Rule (45 CFR 164.308, 164.310, 164.312) and the Privacy Rule safeguards standard (164.530(c))
- NIST Cybersecurity Framework 2.0
- NIST SP 800-30 for risk rating

## Limitations

- This is a portfolio exercise for a hypothetical organization. It is not an audit, a compliance certification, or legal advice.
- Likelihood and impact scores are reasoned estimates. A real engagement would base them on interviews, incident history, and technical testing.
- Only the physical and visitor policies are written. The gaps listed in the control mapping are future work.

## About

Built by Luella Henderson as part of a transition into cybersecurity and GRC. More projects are on my [GitHub profile](https://github.com/Luella-Cyber).
