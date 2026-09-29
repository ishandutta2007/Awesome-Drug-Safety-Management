# Awesome-Drug-Safety-Management

# Top Drug Safety Management Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Pharmacovigilance, Adverse Event Reporting & Signal Detection*  
**Last updated: September 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Drug Safety Management** (Pharmacovigilance). These tools manage adverse event intake, case processing, regulatory reporting, and safety signal detection for pharmaceutical companies, CROs, and regulatory affairs teams.

**Examples** include Oracle Argus, ArisGlobal, Veeva Vault Safety, Ennov, SARUS, AB Cube, Celegence, IQVIA Vigilance, EXTEDO, and Pharmapod (the category leaders).

**Open-source emphasis**: This section is expanded with active projects for self-hosting, custom signal detection, and transparent adverse event workflows — ideal for researchers, academic pharmacovigilance groups, and developers building vendor-independent drug safety solutions. The open-source ecosystem offers statistical signal detection packages, adverse event reporting systems, and RAG-based safety intelligence tools, though full enterprise case management platforms remain largely commercial.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Oracle Argus](https://www.oracle.com/life-sciences/safety-solutions/argus-safety-case-management/)**  
  Industry-leading pharmacovigilance platform for processing, analyzing, and reporting adverse event cases across pre-market and post-market drugs, biologics, vaccines, and devices. Modules include Argus Safety (case intake, triage, duplicate checking, medical review, E2B messaging), Argus Affiliate (global regulatory compliance for affiliates and partners), Argus Interchange (electronic exchange with regulators), Argus Dossier (periodic safety report lifecycle), and Argus Insight (multidimensional safety data analysis) . QPS Holdings deployed Oracle Argus in January 2026 for clinical trial safety case management .

- **[ArisGlobal LifeSphere](https://www.arisglobal.com/)**  
  AI-first pharmacovigilance platform with LifeSphere Safety, MultiVigilance (end-to-end case processing), Reporter (multilingual field reporting), and Advanced Signals powered by NavaX. Advanced Signals delivers 80% faster signal assessment and 40-50% reduced false positives . A leading Japanese pharmaceutical organization processing ~20,000 safety cases annually adopted LifeSphere Safety across Japan, US, and Europe in August 2025 . A global biopharmaceutical company deployed LifeSphere Intake & Triage, Literature Intelligence, and Reporter in Japan in June 2026, supporting ~10,000 annual PV and literature management activities .

- **[Veeva Vault Safety](https://www.veeva.com/)**  
  Modern ICSR management system on the Veeva Vault platform, announced 2019 and now Mature with 51-100 enterprise pharma, biotech, and CRO customers. Manages intake, processing, and submission of adverse events for clinical and post-marketed products across drug, biologic, vaccine, device, and combination products. Built-in gateway connections and reporting rules streamline submissions to health authorities. Central coding dictionary management automates semi-annual MedDRA, WHODrug, and EDQM updates .

- **[Ennov](https://www.ennov.com/)**  
  Life sciences regulatory and safety software covering pharmacovigilance, regulatory submissions, and quality management.

- **[SARUS](https://www.sarus.com/)**  
  Pharmacovigilance and drug safety platform for adverse event management and regulatory compliance.

- **[AB Cube](https://www.abcube.com/)**  
  Pharmacovigilance and safety database solutions for case management and regulatory reporting.

- **[Celegence](https://www.celegence.com/)**  
  Regulatory and pharmacovigilance services with technology solutions for safety case management.

- **[IQVIA Vigilance](https://www.iqvia.com/)**  
  Pharmacovigilance platform and services for adverse event management, signal detection, and regulatory reporting.

- **[EXTEDO](https://www.extedo.com/)**  
  Regulatory information management with pharmacovigilance capabilities for safety reporting.

- **[Pharmapod](https://www.pharmapod.com/)**  
  Pharmacy safety and adverse event reporting platform for community pharmacy and healthcare settings.

## Open-Source GitHub Projects

- **[pvEBayes](https://github.com/YihaoTancn/pvEBayes)**  
  The most comprehensive open-source R package for empirical Bayes methods in pharmacovigilance, published on CRAN (v0.2.1, January 2026, GPL-3). Implements Gamma-Poisson Shrinker (GPS), Koenker-Mizera (KM), Efron's nonparametric empirical Bayes, K-gamma model, and general-gamma model. First implementation of the bi-level Expectation Conditional Maximization (ECM) algorithm for efficient parameter estimation in gamma mixture prior models. Provides a fully open-source alternative to KM method using CVXR (avoiding commercial Mosek solver dependency) and modified Efron method supporting exposure/offset parameters . Published in Statistics in Medicine (2025) and arXiv .

- **[caAERS](https://github.com/CBIIT/caaers)**  
  Cancer Adverse Event Reporting System from NCI-CBIIT, a JSP-based Java web application using Hibernate and Spring technologies. Supports regulatory and protocol compliance for adverse event reporting, local collection, management, and querying of AE data, and service-based integration with other clinical trials management systems. BSD 3-Clause licensed. **Note**: Master codebase undergoing active development and may not be cleared for production usage by NCI-CBIIT .

- **[simaerep](https://github.com/openpharma/simaerep)**  
  Open-source R package from the IMPALA Consortium for rapid, comprehensive, and near-real-time detection of adverse event under-reporting and over-reporting at clinical trial sites. Uses patient-level AE and visit data with statistical probability scoring to manage and target quality assurance activities. v0.6.0 (late 2024) supports in-database processing for enterprise IT scaling. High unit test coverage with automated validation report pipeline. Ready for industry use .

- **[MakerChecker PV ICSR Processing](https://github.com/makerchecker/MakerChecker)**  
  Open-source agentic AI workflow for pharmacovigilance ICSR processing that enforces separation of duties with human-in-the-loop gates. The case-processor agent ingests adverse-event cases and proposes which look serious and unexpected (case-triage, low risk, ungated). Two high-risk acts are gated: seriousness-assess (the binding serious-and-unexpected determination that starts the 15-day expedited clock under 21 CFR 314.80) and e2b-submit (transmission of ICSR to regulatory gateway in E2B(R3) format). The engine's flow grammar will not publish a high-risk skill unless an approval gate precedes the step (high_risk_requires_gate rule). Separation of duties enforced at runtime with identity-mode gate (forbid_requester). Demonstrates a production-ready architecture for AI-assisted pharmacovigilance with regulatory compliance .

- **[OpenVigil](https://openvigil.sourceforge.net/)**  
  Open-access web resource that mines FDA Adverse Event Reporting System (FAERS) data for basic drug-ADR risk detection using RR, PRR, or ROR metrics. Free for academic use. One of several open-access tools for FAERS data mining .

- **[AERS Spider](https://github.com/)**  
  Open-access web resource for mining FAERS data with basic drug-ADR risk detection using RR, PRR, or ROR metrics. Free for academic use .

- **[openFDA Pharmacovigilance Tools](https://github.com/topics/openfda)**  
  Collection of open-source tools leveraging the openFDA API for adverse event analysis. Includes real-time drug safety intelligence APIs with hybrid RAG combining live openFDA adverse events, PubMed literature, and FAISS biomedical knowledge base synthesized by Llama 3.3-70B. Also includes audit-logged RAG over OpenFDA drug labels with citation grounding, PII detection, and adversarial safety (100% refusal on unanswerable/PII/adversarial queries, 90% citation rate on grounded queries) .

- **[OpenMed reporting-adverse-events Skill](https://tool.lu/es_ES/skill/s/bMP)**  
  Open-source agent skill (Apache-2.0) that structures adverse-event mentions into FAERS/ICH E2B(R3) reportable fields including suspect drug, reaction (MedDRA PT), seriousness criteria (death, life-threatening, hospitalization, disability, congenital anomaly), and reaction outcomes. Pairs with OpenMed NER to consume Pharmaceutical/Chemical and Disease entities. Produces structured drafts for human safety review — does not file reports or perform causality assessment autonomously. MedDRA is licensed and user-supplied, never bundled .

- **[REDCap Adverse Event Reporting](https://github.com/PHSERIS/ae_reporting)**  
  REDCap External Module facilitating creation of Adverse Event reports for ClinicalTrials.gov, IRB, and FDA templates. Connects to existing REDCap projects or acts as standalone AE data collection. Eliminates aggregation steps, minimizes redundancy. Requires REDCap v8.5+, HTTPS, API enabled, PHP 8.1 .

- **[MDDC (Multiple Drug-Drug Comparison)](https://cran.ma.ic.ac.uk/web/packages/MDDC/refman/MDDC.html)**  
  Open-source R package for statistical analysis of adverse event contingency tables with adaptive boxplot coefficient grid search for FDR control, and simulation of contingency tables with clustered AE correlation. Includes betablocker500 dataset for pharmacovigilance research .

### Additional Strong Open-Source Options

- **FAERS Analysis Repositories** — Numerous Jupyter Notebook projects performing disproportionality analysis (ROR/PRR/EBGM) on FDA FAERS data to surface drug safety signals .
- **Pharmacovigilance GraphRAG Assistant** — Cited, grounded Q&A over FDA drug labels using Neo4j + FAERS adverse-event data. Free-tier stack with risk-based OQ/PQ validation .
- **Adverse Event Queue Operator Surface** — Browser-only operator surface for adverse-event queue, signal-detection clusters, regulator-reporting deadlines (FDA MedWatch 15-day / EU MDR vigilance / PMDA), and causality-assessment workflow. AGPL-3.0. No telemetry .
- **OpenFDA Drug Recall Scraper** — OpenFDA drug/device/food recalls, adverse events & 510(k) clearances as JSON/CSV. No API key, no login .

**Frameworks for building custom drug safety solutions**: Combine **pvEBayes** for statistical signal detection with empirical Bayes methods validated in peer-reviewed publications . Use **simaerep** for clinical trial site-level AE under-reporting and over-reporting detection . Deploy **caAERS** for cancer clinical trial adverse event reporting with regulatory compliance . Leverage **MakerChecker** for AI-assisted ICSR processing with human-in-the-loop approval gates and separation of duties enforcement . Integrate **OpenMed reporting-adverse-events** for structuring narratives into E2B(R3) reportable fields . Note that true enterprise pharmacovigilance platforms with global regulatory gateway connectivity (FDA FAERS, EMA EudraVigilance), MedDRA/WHODrug licensing, and validated audit trails remain primarily commercial territory; open-source stacks provide strong statistical foundations, reporting frameworks, and AI-assisted case processing that require integration for complete safety operations.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Drug safety tools must comply with regulatory requirements (21 CFR 314.80, EU GVP, ICH E2B(R3)) and validated system requirements for GxP compliance. MedDRA and WHODrug dictionaries are licensed and user-supplied.
- Self-hosted open-source solutions require proper infrastructure, validation protocols, and ongoing maintenance. Statistical signal detection requires domain expertise and should complement, not replace, human safety review.
- The open-source ecosystem provides strong statistical foundations, clinical trial reporting, and AI-assisted case processing, but full enterprise pharmacovigilance platforms with global regulatory gateway connectivity and validated audit trails remain primarily a commercial offering.

---

**Made for pharmacovigilance professionals, drug safety officers, clinical researchers, and regulatory affairs teams.**  
Let's make drug safety management more open, transparent, and statistically rigorous.
