# Hi, I'm Ojas Pandey 👋

### Senior Detection Engineer · SIEM & Threat Hunting · Applied AI/ML & GenAI for the SOC

I've spent the last decade in security operations - building detection content, hunting threats, and helping enterprises mature their SOCs at [Securonix](https://www.securonix.com/). I now work at the intersection of **detection engineering and applied AI**: writing ATT&CK-mapped detections, verifying them against simulated attacks, and building guardrailed LLM pipelines - then measuring honestly whether they actually help.

If you're working on detection engineering, AI for security operations, or SOC automation - I'd love to talk.

---

## 🔭 What I'm working on

- **LLM security & governance** - PII-masking gateway design (regex → NER → local LLM), and evaluating LLM outputs against ground truth: grounding, unsupported statements, IOC completeness, ATT&CK accuracy, query validity and confidence calibration - informed by ISO/IEC 42001
- **Applied ML for SOC operations** - explainable models for threat triage and agentic pipelines for ticket generation

## 🚀 Featured Projects

**[AlertMind - AI-Assisted Mini SOC](https://github.com/opandey1/alertmind)** 🛡️ *(capstone - complete)*

   - **End-to-end SOC architecture:** Built an isolated Wazuh 4.14.5 lab ingesting Windows/Sysmon and Linux/auditd telemetry, with two operational dashboards, three incident-response playbooks, and verified 90-day retention across 21 managed alert indices.
   - **Detection engineering:** Authored 25 Sigma detections and implemented 24 as custom Wazuh rules, with Windows service creation mapped to built-in rule 61138; documented ATT&CK-mapping caveats and verified all custom rules through controlled simulations, including Atomic Red Team.
   - **Detection performance:** Measured a **2.32-second median attack-to-alert latency** and retained command output, screenshots, rule sources, and tuning notes-including false-positive exclusions and known indicator-versus-behavioural coverage gaps.
   - **Guardrailed AI triage:** Engineered a Python/Streamlit Tier-1 assistant supporting local, hosted, and deterministic mock providers, with tested credential redaction, strict JSON validation, prompt-injection visibility, an independent boundary gate, and auditable runs.
   - **Constrained by design:** Assistant outputs are draft-only under mandatory analyst review, with **no Wazuh write/action path, no response tools, and no enforcement integration**.
   - **Measured human impact:** On a frozen 20-alert corpus, all 14 correctly dispositioned alerts were triaged faster, while all six incorrect dispositions were slower (**+1.68 min paired median**); analyst review preserved **20/20 accuracy** while exposing its measurable time cost.
   - **Evaluation integrity:** A strict label-reduced view collapsed llama3.1:8b's exact ATT&CK score from **14/14 to 1/14**, revealing label copying rather than independent classification; the model also identified **0/6 benign false positives**, supporting a documented no-deploy decision for that use case.
   - **Reproducible and honestly scoped:** Backed by **67 automated tests**, a hashed corpus, retained audit logs, timing data, manual grounding worksheets, and a re-runnable analysis notebook; live Wazuh-to-assistant integration remains an explicitly documented target state, not a shipped feature.

**[Project KAVACH](https://github.com/opandey1/project-kavach)** 🔍

A solo four-week security engagement for a fictional Indian NBFC, fusing **network forensics** (PCAP triage, hypothesis-driven analysis with confirm/refute verdicts, IOC extraction with confidence ratings) with **web application security assessment** (OWASP Top 10 exploitation, code-level remediation, before/after Semgrep SAST baselines) — synthesized into a joint **STRIDE threat model** and a seven-layer **defence-in-depth proposal** with a board-ready executive readout.

**[AI-SOC-Assistant](https://github.com/opandey1/AI-SOC-Assistant)** - Explainable, local-first SOC triage platform.

Classifies network connections into five classes - **Normal, DoS, Probe, R2L, and U2R** - instead of returning only a binary anomaly flag.

   - **Detection and evidence:** Fuses a Random Forest family classifier with a training-calibrated Isolation Forest signal. Per-connection SHAP evidence shows which observed features support or oppose the verdict.
   - **Live workflow:** Delayed replay and Kafka-compatible events feed a shared inference runtime and a dark Streamlit console for triage, SHAP analysis, incident tickets, and analyst review.
   - **Governed GenAI:** Generates evidence-bound tickets through deterministic templates or a guardrailed LangGraph workflow. Supports offline deterministic operation and local Ollama; cloud providers and threat-intelligence lookups are explicit opt-ins.
   - **Feedback loop:** Stores tickets and append-only analyst reviews in SQLite. Reviewed false positives become weighted retraining examples saved as atomic, versioned model artifacts.
   - **Honest evaluation:** Achieved 99.88% NSL-KDD holdout accuracy and 74.40% KDDTest+ accuracy; zero-tuning transfer to UNSW-NB15 reached 58.89% accuracy and 16.02% macro F1, quantifying the cross-dataset generalization gap.
   - **Engineering quality:** Backed by 118 automated tests, Python 3.10-3.12 CI, reproducible evaluation artifacts, and non-root Docker checks.

**[SentinelScribe](https://github.com/opandey1/SentinelScribe)** - A three-pass GenAI pipeline that transforms raw cybersecurity course audio transcripts into structured, forensically-accurate Markdown study guides.

**[Deep-Learning-Projects](https://github.com/opandey1/Deep-Learning-Projects)** - Iterative CNN optimization achieving >90% on CIFAR-10 and ~73% on CIFAR-100 in PyTorch, using SGD with Nesterov Momentum and Cosine Annealing.

## 🛠️ Tech Stack

**Detection & SIEM**
![Wazuh](https://img.shields.io/badge/-Wazuh-3585C6?style=flat&logo=wazuh&logoColor=white)
![Sigma](https://img.shields.io/badge/-Sigma_Rules-1a1a1a?style=flat)
![Sysmon](https://img.shields.io/badge/-Sysmon-0078D4?style=flat)
![auditd](https://img.shields.io/badge/-auditd-333?style=flat&logo=linux&logoColor=white)
![MITRE ATT%26CK](https://img.shields.io/badge/-MITRE_ATT%26CK-005FAD?style=flat)
![Atomic Red Team](https://img.shields.io/badge/-Atomic_Red_Team-D32F2F?style=flat)
![SIEM](https://img.shields.io/badge/-SIEM-B22222?style=flat)
![UEBA](https://img.shields.io/badge/-UEBA-8B0000?style=flat)
![Threat Hunting](https://img.shields.io/badge/-Threat_Hunting-1a1a1a?style=flat)
![Incident Response](https://img.shields.io/badge/-Incident_Response-555?style=flat)

**AI / ML / GenAI**
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat&logo=python&logoColor=white)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?style=flat&logo=pytorch&logoColor=white)
![scikit-learn](https://img.shields.io/badge/-scikit--learn-F7931E?style=flat&logo=scikit-learn&logoColor=white)
![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?style=flat&logo=langchain&logoColor=white)
![LangGraph](https://img.shields.io/badge/-LangGraph-1C3C3C?style=flat)
![Ollama](https://img.shields.io/badge/-Ollama-000000?style=flat&logo=ollama&logoColor=white)
![SHAP](https://img.shields.io/badge/-SHAP-9146FF?style=flat)
![Streamlit](https://img.shields.io/badge/-Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)
![Jupyter](https://img.shields.io/badge/-Jupyter-F37626?style=flat&logo=jupyter&logoColor=white)

**Forensics & AppSec**
![Wireshark](https://img.shields.io/badge/-Wireshark-1679A7?style=flat&logo=wireshark&logoColor=white)
![Zeek](https://img.shields.io/badge/-Zeek-777BB4?style=flat)
![OWASP ZAP](https://img.shields.io/badge/-OWASP_ZAP-00549E?style=flat)
![Semgrep](https://img.shields.io/badge/-Semgrep-2ACFA6?style=flat&logo=semgrep&logoColor=white)

**Data / Platforms**
![Spark](https://img.shields.io/badge/-Spark-E25A1C?style=flat&logo=apache-spark&logoColor=white)
![Solr](https://img.shields.io/badge/-Solr-D9411E?style=flat&logo=apache-solr&logoColor=white)
![HBase](https://img.shields.io/badge/-HBase-CC0000?style=flat&logo=apache&logoColor=white)
![MySQL](https://img.shields.io/badge/-MySQL-4479A1?style=flat&logo=mysql&logoColor=white)
![Linux](https://img.shields.io/badge/-Linux-FCC624?style=flat&logo=linux&logoColor=black)

## 💼 Experience snapshot

**Securonix** (2015 – 2025) — progressed from Information Security Analyst to Senior Technical Account Manager, leading threat hunting, SIEM/UEBA content development, and customer success across enterprise SOC programs. Highlights:

- Drove a **25% reduction in alert fatigue** for an enterprise client by re-engineering Insider Threat policies and threat models.
- Led end-to-end development of advanced detection content mapped to **MITRE ATT&CK**, lowering false positives and accelerating investigations.
- Contributed to **Securonix Threat Labs** threat intelligence publications (APT activity, ransomware, vulnerability exploitation, IOC/TTP analysis).
- Built and mentored an offshore team standardizing SIEM parsers and out-of-the-box content.

## 📜 Selected Certifications

- **GIAC** — AWS Secure Builder
- **MITRE ATT&CK** — Fundamentals · Cyber Threat Intelligence · Threat Hunting & Detection Engineering
- **SANS SEC401** — Security Essentials Bootcamp

## 🎓 Education

- **PG Certificate, AI/GenAI Powered Cybersecurity**, IIT Roorkee × Futurense — *Cohort 1*
- **M.S. Cyber Security Engineering**, University of Southern California — GPA 3.70
- **B.Tech Information Technology** (Honors), The NorthCap University

## 📫 Get in touch

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ojaspandey/)

---

<sub>Open to Senior SOC Engineer, Senior Detection Engineer, and AI Security Engineer roles — and collaborations in AI for security operations, detection engineering, and SOC automation.</sub>
