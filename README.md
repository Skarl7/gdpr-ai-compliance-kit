# GDPR & EU AI Act Compliance Kit

> Open-source compliance toolkit for GDPR and EU AI Act risk classification

[![GDPR](https://img.shields.io/badge/GDPR-Compliant-003087?logo=europeanunion&logoColor=white)](https://gdpr.eu)
[![EU AI Act](https://img.shields.io/badge/EU%20AI%20Act-2024-0052CC?logo=europeanunion&logoColor=white)](https://artificialintelligenceact.eu)
[![Open Source](https://img.shields.io/badge/Open%20Source-Apache%202.0-4A90D9)](./LICENSE)

**Built by** [Skarl7](https://github.com/Skarl7) | [AdnexAI](https://www.adnexai.co.uk)

---

## Overview

GDPR & EU AI Act Compliance Kit helps businesses and developers understand and implement their obligations under the General Data Protection Regulation and the EU AI Act. It provides risk classification tools, data mapping templates, and Article 30 Record of Processing Activities generators.

## Components

| Component | Description | Regulation |
|-----------|-------------|------------|
| AI Risk Classifier | Classifies AI systems by risk level | EU AI Act Arts. 5-8 |
| Article 30 Generator | Automated Records of Processing Activities | GDPR Art. 30 |
| DPIA Assistant | Data Protection Impact Assessment templates | GDPR Art. 35 |
| Data Mapping Tool | Visualise data flows and processing activities | GDPR Art. 5 |
| Consent Manager | Track and manage user consent records | GDPR Art. 7 |
| Breach Notification | Automated incident response checklists | GDPR Art. 33-34 |

## AI Risk Classification

The EU AI Act categorises AI systems into four risk levels:

```
Minimal Risk      →  No obligations (e.g. spam filters)
Limited Risk      →  Transparency duties (e.g. chatbots)
High Risk         →  Conformity assessment, documentation
Unacceptable Risk →  Prohibited (e.g. social scoring)
```

### Risk Assessment Matrix

| Factor | Low Score (1) | Medium Score (2) | High Score (3) |
|--------|--------------|------------------|----------------|
| Data Sensitivity | Public data | Personal data | Special category data |
| Decision Impact | Informational | Operational | Health/Legal/Finance |
| Automation Level | Human in loop | Partial automation | Fully autonomous |
| Scale | Individual use | SME use | Mass deployment |
| Duration | One-off | Periodic | Continuous |

**Total Score < 6**: Low risk — minimal obligations
**Total Score 6-10**: Medium risk — transparency + documentation
**Total Score > 10**: High risk — conformity assessment required

## Getting Started

### Prerequisites

- Node.js 18+
- OpenAI API key (for AI-powered assessments)
- Basic understanding of GDPR/EU AI Act principles

### Installation

```bash
git clone https://github.com/Skarl7/gdpr-ai-compliance-kit
cd gdpr-ai-compliance-kit
npm install
```

### Usage

#### Run AI Risk Classification

```bash
node scripts/classify-risk.js --system "AI-powered legal research tool" --data "client confidential" --automation "partial"
```

#### Generate Article 30 Records

```bash
node scripts/article30.js --category "legal services" --output ./records/
```

#### Start DPIA

```bash
node scripts/dpia.js --processing "client data intake" --controller "Lexsk Legal Ltd"
```

## File Structure

```
gdpr-ai-compliance-kit/
├── scripts/
│   ├── classify-risk.js
│   ├── article30.js
│   ├── dpia.js
│   └── consent-tracker.js
├── templates/
│   ├── article30-template.json
│   ├── dpia-template.md
│   ├── privacy-notice-template.md
│   └── breach-notification-template.md
├── docs/
│   ├── eu-ai-act-summary.md
│   ├── gdpr-principles.md
│   └── high-risk-use-cases.md
├── workflows/
│   └── compliance-pipeline.json
└── LICENSE
```

## EU AI Act Summary

### Prohibited Practices (Art. 5)
- Social scoring by governments
- Real-time biometric identification in public
- Manipulative AI (dark patterns)

### High-Risk AI Systems (Art. 6)
- Biometric identification and categorisation
- Critical infrastructure management
- Law enforcement
- Employment and recruitment
- Essential public services
- Credit scoring and insurance

### Obligations for High-Risk Systems
- Risk management system
- Technical documentation
- Concise public information
- Record-keeping
- Human oversight
- Accuracy, robustness, cybersecurity

## GDPR Principles (Art. 5)

1. **Lawfulness, Fairness, Transparency** — Clear legal basis for all processing
2. **Purpose Limitation** — Process data only for stated purposes
3. **Data Minimisation** — Collect only what is necessary
4. **Accuracy** — Keep data accurate and up to date
5. **Storage Limitation** — Delete when no longer needed
6. **Integrity & Confidentiality** — Secure and protect data
7. **Accountability** — Demonstrate compliance

## Disclaimer

This toolkit provides general guidance only and does not constitute legal advice. Always consult a qualified data protection officer or legal professional for specific compliance matters.

## Contributing

Contributions from compliance professionals, lawyers, and developers are welcome.

## License

Apache 2.0

---
*Lexsk Legal Limited — GDPR & Compliance | gdpr-ai-compliance-kit | www.lexsk.co.uk*
