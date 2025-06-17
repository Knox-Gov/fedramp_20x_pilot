# Knox FedRAMP 20x Pilot Submission
<div align="center">
  <img src="visualizations/image8.png" alt="Knox Systems Logo" title="Knox Systems, Inc." />
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
</div>

## Overview

This repository contains Knox's submission for the FedRAMP 20x pilot program, demonstrating our innovative approach to continuous compliance through AI-driven automation. Knox AI represents a paradigm shift from traditional manual compliance processes to real-time, pull-based security validation.

**Knox Trust Center**: For live compliance data, 3PAO attestation, and additional documentation, visit https://trustcenter.knoxsystems.com/

## Table of Contents

- [Cloud Service Provider Summary](#cloud-service-provider-summary)
- [Our Approach](#our-approach)
- [Machine-Readable Assessment](#machine-readable-assessment)
- [Continuous Reporting](#continuous-reporting)
- [3PAO Assessment](#3pao-assessment)
- [Repository Structure](#repository-structure)

## Cloud Service Provider Summary

Knox provides a comprehensive FedRAMP Authorized cloud platform that offers a distinguished record of secure and compliant operational performance. This robust and mature environment is specifically engineered to streamline the FedRAMP authorization journey for SaaS providers, enabling them to achieve their compliance objectives with efficiency and confidence. Our unwavering commitment is to deliver a highly secure and exceptionally reliable foundation for government agencies and their partners to host mission-critical applications and execute high-consequence operations, leveraging the infrastructure of leading hyperscalers such as Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform (GCP). On this platform, we host a variety of services designed to meet diverse federal agency needs:

Adobe Learning Manager (ALM) is an asynchronous Learning Management System that enables Learning and Development teams to drive personalized learning experiences across multiple devices.

## Our Approach

Knox AI fundamentally reimagines FedRAMP compliance through:

- **Pull-Based Architecture**: Unlike traditional push-based evidence collection, Knox AI continuously queries live data from cloud environments
- **100% Resource Coverage**: Evaluates ALL resources across multiple AWS accounts and regions, eliminating sampling bias
- **AI-Powered Analysis**: Leverages Google Gemini 2.5 Flash Preview for intelligent compliance evaluation
- **Automated Scheduling**: Compliance evaluations run automatically every 6 hours
- **Three-Pillar Integration**: Seamlessly integrates infrastructure (AWS APIs), security posture (Wiz CNAPP), and governance (Drata GRC)

[Read our detailed approach rationale →](documentation/approach-rationale.md)

## Machine-Readable Assessment

Our machine-readable assessment package provides:

- **FedRAMP-compliant JSON format** with complete KSI validation status
- **RESTful API endpoints** for real-time compliance data access
- **Comprehensive schema definition** for automated validation
- **Supporting evidence** integrated from multiple authoritative sources

This repository includes sample data and schemas. For live, real-time assessment data, visit the Knox Trust Center at https://trustcenter.knoxsystems.com/

Key endpoints:
- `/api/compliance/fedramp-output` - Complete FedRAMP-formatted results
- `/api/compliance/fedramp-output/detailed` - Includes additional metadata
- `/api/compliance/fedramp-output/schema-detailed` - Full schema definition

[View schema documentation →](schemas/fedramp-output-schema.json)

## Continuous Reporting

Knox AI enables true continuous compliance through:

- **6-hour automated evaluation cycles** with on-demand options
- **Historical tracking** with complete audit trails
- **Trend analysis** of compliance posture over time
- **Real-time drift detection** and automated remediation guidance
- **API-driven integration** with existing GRC platforms

[Read our continuous reporting proposal →](documentation/continuous-reporting-proposal.md)

## 3PAO Assessment

Our third-party assessment is conducted by Coalfire, a FedRAMP-recognized 3PAO with extensive experience in cloud security assessments. Their assessment validates Knox AI's innovative approach to continuous compliance.

The complete 3PAO attestation letter and detailed findings are available at the Knox Trust Center: https://trustcenter.knoxsystems.com/

[View 3PAO assessment overview →](3pao-assessment/README.md)

## Repository Structure

```
fedramp_20x_pilot/
├── README.md                          # This file
├── documentation/                     # Detailed documentation
│   ├── approach-rationale.md         # Our innovative approach explained
│   ├── continuous-reporting-proposal.md  # Continuous KSI validation
│   └── cloud-service-summary.md      # CSP and CSO details
├── machine-readable-assessment/       # Machine-readable compliance data
│   ├── ksi-validation-results.json   # Current KSI validation status
│   └── evidence-mappings.json        # Evidence source mappings
├── schemas/                          # Data schemas and definitions
│   └── fedramp-output-schema.json    # Complete schema definition
├── 3pao-assessment/                  # Third-party assessment
│   └── README.md                     # 3PAO overview and trust center reference
└── visualizations/                   # Screenshots and diagrams
    └── README.md                     # Platform walkthrough with screenshots
```

## Key Differentiators

1. **Scale**: Evaluates thousands of resources across multiple accounts in minutes
2. **Speed**: Reduces authorization time from weeks to hours
3. **Consistency**: AI-driven evaluation removes human variance
4. **Flexibility**: Easily adaptable to new KSIs or requirements
5. **Cost-Effective**: Reduces manual effort by 90%+
6. **Trustworthy**: Pull-based model with verifiable audit trails

## Contact Information

For questions about this submission:
- Email: fedramp20x@knoxsystems.com
- Website: [www.knoxsystems.com](https://www.knoxsystems.com)
- 3PAO Contact: Coalfire Systems, Inc.

---

*This submission represents the future of FedRAMP—real-time, automated, and ready now.*