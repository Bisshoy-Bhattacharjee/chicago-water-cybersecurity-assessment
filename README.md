# Chicago Department of Water Management: Cybersecurity Risk Assessment

An independent, public-information-based cybersecurity risk assessment examining ransomware, third-party risk, and IT/OT resilience within the City of Chicago Department of Water Management (DWM).

![Assessment Cover](diagrams/assessment-cover.png)

**Framework:** NIST Cybersecurity Framework (CSF) 2.0  
**Information cutoff:** November 2026  
**Version:** 2.1

---

## Project Overview

In August 2026, Chicago's Water Commissioner publicly disclosed that the Department of Water Management had experienced a ransomware incident approximately one year earlier. The incident affected vendor-supplied administrative and office computers, which remained locked for roughly two months. A small amount of work-related paperwork was taken, no ransom was paid, and the affected systems were rebuilt.

This project examines the publicly reported incident and evaluates potential cybersecurity risks to the department, with particular attention to third-party access, ransomware resilience, and the boundary between information technology (IT) and operational technology (OT).

Using publicly available reporting, City disclosures, and cybersecurity guidance, the assessment identifies potential risk scenarios, reviews publicly visible controls, and develops practical remediation recommendations.

## Assessment Scope

The assessment focuses on five areas:

- Third-party and vendor access management
- Ransomware prevention and administrative IT resilience
- Identity and privileged access management
- IT/OT network separation and OT remote access
- Incident response, backup, and operational recovery

The assessment uses NIST CSF 2.0 as its primary framework, supported by the following publications:

- NIST SP 800-30 Rev. 1: Guide for Conducting Risk Assessments
- NIST SP 800-82 Rev. 3: Guide to Operational Technology Security
- NIST SP 800-161 Rev. 1 Update 1: Cybersecurity Supply Chain Risk Management
- NIST SP 800-53 Rev. 5: Security and Privacy Controls

## Key Findings

The assessment identified six potential cybersecurity risk scenarios.

| Risk ID | Risk Scenario | Score | Rating |
|---|---|---:|---|
| RSK-001 | Third-Party and Vendor Access | 12 | High |
| RSK-002 | Ransomware and Administrative IT Disruption | 12 | High |
| RSK-003 | Unauthorized Access and Identity Compromise | 8 | Moderate |
| RSK-004 | Insufficient IT/OT Separation | 10 | High |
| RSK-005 | Unauthorized Remote Access to OT | 10 | High |
| RSK-006 | Backup, Recovery, and Operational Resilience | 12 | High |

Five scenarios received a High rating and one received a Moderate rating.

These are preliminary inherent risk estimates based on a project-defined likelihood and impact scale. They do not represent confirmed security weaknesses or verified operational risk.

The assessment also reviewed eight control areas and proposed eight remediation actions. The highest-priority recommendations include:

1. Reviewing vendor inventories, permissions, and remote access arrangements.
2. Validating endpoint protection, patching, and ransomware containment capabilities.
3. Testing backup isolation, integrity, and restoration procedures.
4. Verifying current IT/OT network separation and approved communication paths.
5. Reviewing OT remote access, security monitoring, and incident response procedures.

## Methodology

The assessment follows a structured risk assessment approach:

1. Collect and review public sources, including news reporting, City disclosures, and government cybersecurity publications.
2. Establish the organization's operational and technology context.
3. Document incident-related evidence and distinguish confirmed information from unknowns.
4. Identify cybersecurity risk scenarios based on available evidence.
5. Evaluate likelihood and impact using a 1–5 scoring scale.
6. Map eight control areas to NIST CSF 2.0 functions.
7. Develop prioritized remediation recommendations and a proposed implementation roadmap.

### Risk Scoring

Risk score = Likelihood × Impact

Both likelihood and impact are scored from 1 to 5. The resulting scoring bands are defined for this project and are not prescribed by NIST.

| Score | Rating |
|---|---|
| 1–4 | Low |
| 5–9 | Moderate |
| 10–16 | High |
| 17–25 | Critical |

Only inherent risk is scored. Residual risk is not calculated because current control implementation and effectiveness could not be validated using public information.

## Repository Contents

```text
chicago-water-cybersecurity-assessment/
│
├── README.md
│
├── report/
│   └── Chicago_Water_Cybersecurity_Assessment.pdf
│
├── workbook/
│   └── Chicago_Water_Cybersecurity_Assessment_Workbook.xlsx
│
├── diagrams/
│   └── assessment-cover.png
│
└── references/
    └── sources.md
```

### Assessment Report

The PDF report contains the full assessment, including:

- Scope, methodology, and evidence standards
- Organization and technology context
- Incident background and timeline
- Risk evaluation and prioritization
- NIST CSF 2.0 control assessment
- Recommendations and remediation roadmap
- Limitations and further research

### Supporting Excel Workbook

The workbook contains the supporting assessment registers and analysis:

- Source register
- Incident timeline
- Technology inventory
- Research gaps
- Evidence register
- Assessment methodology
- Risk register
- Control assessment
- Remediation plan

## Limitations

This assessment is based exclusively on publicly available information. No internal DWM documentation, network diagrams, system configurations, access records, or stakeholder interviews were available.

Consequently:

- Risk scores represent the author's preliminary estimates, not measured operational risk.
- Publicly undocumented controls are not assumed to be absent.
- Historical disclosures are not treated as proof of current security configurations.
- Public reporting does not establish that water treatment or OT systems were compromised.
- Residual risk is not scored because control effectiveness could not be independently validated.

The assessment is not an official audit, penetration test, compliance certification, or evaluation commissioned by the City of Chicago.

## References

The assessment draws on public reporting, City of Chicago disclosures, and NIST publications. The complete source list is included in the report.

Key references:

- [NIST Cybersecurity Framework 2.0](https://www.nist.gov/cyberframework)
- [NIST SP 800-30 Rev. 1](https://csrc.nist.gov/pubs/sp/800/30/r1/final)
- [NIST SP 800-82 Rev. 3](https://csrc.nist.gov/pubs/sp/800/82/r3/final)
- [NIST SP 800-161 Rev. 1 Update 1](https://csrc.nist.gov/pubs/sp/800/161/r1/upd1/final)
- [NIST SP 800-53 Rev. 5](https://csrc.nist.gov/pubs/sp/800/53/r5/upd1/final)

## Disclaimer

This is an independent academic and portfolio project prepared for educational and professional development purposes. It is based on publicly available information and is not affiliated with, commissioned by, or endorsed by the City of Chicago or its Department of Water Management.
