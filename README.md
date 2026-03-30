<img src="https://www.ideagen.com/media/11748/grc-circle.png" width="300" class="center">

# awesome-security-GRC

> A curated knowledge base for security GRC practitioners — built by someone who studied it, enforced it at enterprise scale, and runs it in a homelab.

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](CONTRIBUTING.md)

---

## Why This Exists

Most GRC resources are written from one of two angles: the compliance auditor or the framework theorist. This repo is different.

I came to GRC through the enforcement side — 6+ years building and shipping endpoint security products at Tanium, managing MDM policy across enterprise-scale Windows, macOS, and Linux fleets. I studied the academic foundations at Georgia Tech. I apply it daily in a 50+ endpoint homelab running pfSense, VLANs, Intune CSPs, and CIS-hardened systems.

GRC isn't a checkbox exercise. It's the connective tissue between policy and reality. This repo is the knowledge base I wish I had when I started — combining frameworks, tooling, practitioner patterns, and real-world enforcement resources.

Pull requests are welcome. Definitions are debated. The only consensus is that compliance is hard and everyone's doing their best.

---

## :notebook_with_decorative_cover: Contents

- [What is Security GRC?](#mortar_board-what-is-security-grc)
  - [Governance](#guardsman-governance)
  - [Risk Management](#chart_with_upwards_trend-risk-management)
  - [Audit & Compliance](#gun-audit--compliance)
- [Endpoint Security & GRC — The Practitioner's Angle](#computer-endpoint-security--grc--the-practitioners-angle)
- [Books](#books-books)
- [Talks & Videos](#tv-talksvideos)
- [People You Should Know](#telephone_receiver-people-you-should-know)
- [Repositories](#octocat-repositories)
- [Podcasts](#microphone-podcasts)
- [Certifications](#scroll-certifications)
- [The Knowledge Trifecta](#triangular_ruler-the-knowledge-trifecta)

---

# :mortar_board: What is Security GRC?

Security GRC (Governance, Risk, and Compliance) is the operational layer that connects a security program to business objectives. It answers three questions:

- **Governance**: Are we doing security the right way? Who's responsible?
- **Risk**: What could go wrong, how bad, and how likely?
- **Compliance**: Are we meeting the standards we committed to?

Every title in this field is different — Cyber Risk Manager, Security Compliance Program Manager, BISO, Head of the Department of No. The variety makes it harder to organize knowledge than in software engineering. This repo tries to bridge that gap.

## :guardsman: Governance

Governance focuses on how security is managed and its oversight. This includes:

- Building and maintaining the security strategy
- Managing the security programme with continuous monitoring
- Policy and procedure ownership
- Metrics, dashboards, and executive reporting
- Stakeholder management and upward communication

## :chart_with_upwards_trend: Risk Management

Risk is traditionally: **Risk = Threat × Vulnerability**

A robust program adds quantitative analysis — translating risk into financial impact so executives understand *cost*, not just severity.

### Risk Management Frameworks

#### COSO Enterprise Risk Management
The [COSO ERM Framework (2020)](https://www.coso.org/Documents/Compliance-Risk-Management-Applying-the-COSO-ERM-Framework.pdf) addresses *any type of risk* that could prevent achieving business objectives.

#### Factor Analysis of Information Risk (FAIR)
[FAIR](https://www.fairinstitute.org/) is the standard for quantitative cyber risk. If you want to put a dollar figure on risk, start here.

#### ISO 27005 / ISO 31000
- [ISO 27005:2022](https://www.iso.org/standard/80585.html) — information security risk management guidance
- [ISO 31000](https://www.iso.org/iso-31000-risk-management.html) — enterprise risk management guidelines

#### NIST RMF
The [NIST Risk Management Framework](https://csrc.nist.gov/Projects/risk-management) integrates security, privacy, and risk into the system development lifecycle. Key publications:
- [NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final) — RMF for Information Systems
- [NIST SP 800-39](https://csrc.nist.gov/publications/detail/sp/800-39/final) — Managing Information Security Risk
- [NIST SP 800-30](https://csrc.nist.gov/publications/detail/sp/800-30/rev-1/final) — Guide for Conducting Risk Assessments

#### Other Notable Frameworks
- **OCTAVE** — Carnegie Mellon SEI methodology
- **TARA (MITRE)** — [Threat Assessment and Remediation Analysis](https://www.mitre.org/publications/technical-papers/threat-assessment-and-remediation-analysis-tara)
- **Mozilla RRA** — [Rapid Risk Assessment](https://infosec.mozilla.org/guidelines/risk/rapid_risk_assessment.html) in 60 minutes

### Risk Management Tools

- **[Comply](https://github.com/strongdm/comply)** — SOC2-focused compliance automation
- **[CISO Assistant](https://github.com/intuitem/ciso-assistant-community)** — Open-source GRC platform supporting 46+ frameworks
- **[riskquant (Netflix)](https://github.com/Netflix-Skunkworks/riskquant)** — Python library for quantitative risk analysis

## :gun: Audit & Compliance

Compliance is evidence that controls work as designed. Audit is the verification mechanism.

### Frameworks and Regulations

| Framework | Scope |
|-----------|-------|
| [SOX](https://www.congress.gov/bill/107th-congress/house-bill/3763) | US publicly traded companies |
| [GDPR](https://gdpr-info.eu/) | Any org handling EU citizen data |
| [PCI-DSS](https://www.pcisecuritystandards.org/) | Payment card processing |
| [HIPAA](https://www.hhs.gov/hipaa/index.html) | US healthcare data |
| [ISO 27001](https://www.iso.org/isoiec-27001-information-security.html) | ISMS certification standard |
| [SOC 2](https://www.aicpa.org/interestareas/frc/assuranceadvisoryservices/aicpasoc2report.html) | SaaS/service org trust criteria |
| [FedRAMP](https://www.fedramp.gov/) | US federal cloud services |
| [FISMA](https://www.cisa.gov/federal-information-security-modernization-act) | US federal information security |
| [NIST SP 800-53](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final) | Security & privacy controls |
| [NIST CSF](https://www.nist.gov/cyberframework) | Cybersecurity framework |
| [NIS2](https://digital-strategy.ec.europa.eu/en/policies/nis2-directive) | EU critical infrastructure |

---

# :computer: Endpoint Security & GRC — The Practitioner's Angle

> *Most GRC resources are written from the compliance side. This section is written from the enforcement side — by someone who built the tools GRC teams depend on.*

Endpoint security is where GRC policy meets reality. A control is only as good as its enforcement. This section bridges device-level enforcement with compliance reporting.

## Policy Enforcement Tooling

- **[Tanium Enforce](https://www.tanium.com/products/tanium-enforce/)** — Policy enforcement at enterprise scale across Windows, macOS, Linux. Supports BitLocker, Defender, AppLocker, firewall rules, and CSP/LGPO. Built for 100K+ endpoint environments.
- **[Microsoft Intune](https://learn.microsoft.com/en-us/mem/intune/)** — Cloud-native MDM/MAM. Deep integration with Azure AD, Conditional Access, and Defender for Endpoint.
- **[Jamf Pro](https://www.jamf.com/products/jamf-pro/)** — Gold standard for Apple MDM. Supports configuration profiles, compliance checks, and macOS security baselines.
- **[Windows CSP](https://learn.microsoft.com/en-us/windows/client-management/mdm/configuration-service-provider-overview)** — Native Windows policy mechanism via MDM. Takes priority over Group Policy on modern Windows.

## Hardening Baselines & Benchmarks

- **[CIS Benchmarks](https://www.cisecurity.org/cis-benchmarks)** — Industry standard OS and application hardening. Start with Windows 10/11 and macOS.
- **[Microsoft Security Baselines](https://learn.microsoft.com/en-us/windows/security/threat-protection/windows-security-configuration-framework/windows-security-baselines)** — Microsoft's recommended configs. Importable into Group Policy or Intune.
- **[DISA STIGs](https://public.cyber.mil/stigs/)** — DoD hardening guides. Federal compliance gold standard.
- **[NIST SP 800-70](https://csrc.nist.gov/publications/detail/sp/800-70/rev-4/final)** — National Checklist Program tying benchmarks to NIST controls.

## Device Compliance as a Risk Signal

Endpoint telemetry is continuous, real-time evidence of control effectiveness — if you know how to read it:

| Signal | GRC Mapping |
|--------|-------------|
| Patch compliance % by BU | Vulnerability risk scoring |
| Encryption coverage (BitLocker/FileVault) | SOC2, ISO 27001, HIPAA data protection |
| AV/EDR health (Defender, CrowdStrike) | Threat detection capability metrics |
| Configuration drift from hardening baseline | Early warning of control failures |

Most GRC tools treat endpoints as checkboxes. The practitioner reality: this is your richest source of continuous compliance evidence.

## Real-World Resources

- **[Attack Surface Reduction Rules Reference](https://learn.microsoft.com/en-us/defender-endpoint/attack-surface-reduction-rules-reference)** — Full ASR rules catalog for hardening Windows beyond baseline Defender.
- **[Homelab Infrastructure Reference](https://github.com/mansudo/homelab-infrastructure)** — Real-world VLAN layout, Intune CSP policies, and UniFi topology from a 50+ endpoint homelab.
- **[Defender Hardening Playbook](https://github.com/mansudo/defender-hardening-playbook)** — CIS benchmark implementation, PowerShell audit scripts, ASR rule configurations.

---

# :books: Books

- **[Security Risk Management](https://learning.oreilly.com/library/view/security-risk-management/9781597496155/)** — Evan Wheeler, 2011. First stop in security risk management. Comprehensive and accessible.
- **[Measuring and Managing Information Risk](https://learning.oreilly.com/library/view/measuring-and-managing/9780124202313/)** — Freund & Jones, 2014. The FAIR book.
- **[How to Measure Anything in Cybersecurity Risk](https://learning.oreilly.com/library/view/how-to-measure/9781119085294/)** — Hubbard & Seiersen, 2016. Your problem isn't as unique as you think.
- **[Transformational Security Awareness](https://learning.oreilly.com/library/view/transformational-security-awareness/9781119566342/)** — Perry Carpenter, 2019. Best security awareness book written.
- **[Foundations of Information Security](https://learning.oreilly.com/library/view/foundations-of-information/9781098122546/)** — Jason Andress, 2019. High-level practitioner overview.
- **[ISO 27001 Controls](https://learning.oreilly.com/library/view/iso-27001-controls/9781787781467/)** — Bridget Kenyon, 2019. Every Annex A control with implementation guidance.
- **[IT Auditing Using Controls to Protect Information Assets](https://learning.oreilly.com/library/view/it-auditing-using/9781260453232/)** — Kegerreis, Schiller & Davis, 2019. Encyclopedia-level audit reference.
- **[A Leader's Guide to Cybersecurity](https://learning.oreilly.com/library/view/a-leaders-guide/9781633698000/)** — Parenty & Domet, 2019. Security written for the business.
- **[The Cybersecurity Manager's Guide](https://learning.oreilly.com/library/view/the-cybersecurity-managers/9781492076209/)** — Todd Barnum, 2021. Probably the best security leadership book written.

---

# :tv: Talks/Videos

- [Framework overview](https://www.youtube.com/watch?v=dt2IqidgpS4) — how control, program, and risk frameworks work together
- [Quantitative Cyber Risk Analysis](https://www.youtube.com/watch?v=fHUv8TJC6kM) — Evan Wheeler, practical FAIR walkthrough
- [DevOps vs. Compliance: Having It All](https://www.youtube.com/watch?v=r4vznrYn2Qk) — Atlassian GRC team

---

# :telephone_receiver: People You Should Know

- **[Ryan McGeehan](https://scrty.io/)** — Risk management thought leader, former Coinbase/Facebook security
- **[Phil Venables](https://www.philvenables.com/)** — CISO Google Cloud, 20+ years Goldman Sachs
- **[Adobe Tech GRC Team](https://medium.com/adobetech)** — Common Controls Framework, multi-cloud compliance automation
- **[Atlassian Risk & Compliance Team](https://community.atlassian.com)** — DevOps-native compliance patterns

### Follow on LinkedIn
- [Troy Fine](https://www.linkedin.com/in/troyjfine/) — GRC & SOC focus
- [Ayoub Fandi](https://www.linkedin.com/in/ayoubfandi/) — Cloud-native GRC
- [Jacob Horne](https://www.linkedin.com/in/jacob-evan-horne/) — NIST & CMMC

---

# :octocat: Repositories

- **[minimalist-risk-management](https://github.com/magoo/minimalist-risk-management)** — Ryan McGeehan's simple risk program documentation
- **[homelab-infrastructure](https://github.com/mansudo/homelab-infrastructure)** — Real-world endpoint compliance reference architecture
- **[defender-hardening-playbook](https://github.com/mansudo/defender-hardening-playbook)** — CIS benchmarks + PowerShell audit scripts

---

# :microphone: Podcasts

- **[The SecureWorld Sessions](https://podcasts.apple.com/us/podcast/the-secureworld-sessions/id1478674556)** — Weekly security thought leadership
- **[Cloud Security Podcast](https://cloudsecuritypodcast.tv/)** — Cloud-native security from Netflix, LinkedIn, Twilio
- **[Security & Compliance Weekly](https://podcasts.google.com/feed/aHR0cHM6Ly9zY3dhdWRpby5saWJzeW4uY29tL3Jzcw)** — PCI-DSS focus
- **[The GRC Podcast](https://www.thegrcpodcast.com/)** — GRC practitioners and champions

### Notable Episodes
- [Getting Over Our "Security ≠ Compliance" Obsession](https://podcasts.google.com/feed/aHR0cHM6Ly9kYXZpZHNwYXJrLmxpYnN5bi5jb20vY2lzb3ZlbmRvcg/episode/ZThiNjFmNGU0ZTVhNDAzM2E4YTQxZDkzYjE0M2E3NjA) — CISO/Vendor Relationship Podcast
- [Is Governance the Most Important Part of GRC?](https://podcasts.google.com/feed/aHR0cHM6Ly9kZWZlbnNlaW5kZXB0aC5saWJzeW4uY29tL3Jzcw/episode/NTI2MTAwM2MtZWIyZS00ZmIyLWJjY2UtNzk3MWVmNzhjOTE5) — Defense in Depth

---

# :scroll: Certifications

[Paul Jerimy's Security Certification Roadmap](https://pauljerimy.com/security-certification-roadmap/) is the definitive guide. For GRC specifically:

| Cert | Body | Focus |
|------|------|-------|
| CISSP | ISC² | Broad security leadership |
| CISM | ISACA | Security management |
| CRISC | ISACA | Risk and control |
| CISA | ISACA | Audit and assurance |
| Security+ | CompTIA | Foundational practitioner |


---

# :triangular_ruler: The Knowledge Trifecta

GRC requires fluency in three domains simultaneously:

## :floppy_disk: The Technical
Understanding how controls are implemented and measured. Endpoint telemetry, hardening benchmarks, configuration management, log analysis — the evidence layer.

## :lock_with_ink_pen: The Security
Understanding threat models, attack surfaces, and what "risk" actually means at the infrastructure layer. The difference between a checkbox and a control that works.

## :briefcase: The Business
Translating security risk into business language. Every framework exists to support business objectives and legal requirements. A GRC program that can't explain itself to the CFO isn't working.

---

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). PRs welcome — definitions debated, emojis appreciated.
