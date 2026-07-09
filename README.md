# Hi, I'm Ojas Pandey 👋

### Senior Detection Engineer · SIEM & Threat Hunting · Applied AI/ML & GenAI for the SOC

I've spent the last decade in security operations — building detection content, hunting threats, and helping enterprises mature their SOCs at [Securonix](https://www.securonix.com/). I now work at the intersection of **detection engineering and applied AI**: writing ATT&CK-mapped detections, validating them against real adversary tooling, and building guardrailed LLM pipelines that cut triage time without cutting corners.

If you're working on detection engineering, AI for security operations, or SOC automation — I'd love to talk.

---

## 🔭 What I'm working on

- **[AlertMind](https://github.com/opandey1/alertmind)** — my capstone: a working mini-SOC with an LLM tier-1 triage assistant, measured for real impact (details below)
- **LLM security & governance** — PII-masking LLM gateway design (regex → NER → local LLM) and evaluating LLM outputs against ground truth: IOC completeness, ATT&CK mapping accuracy, hallucination rate (ISO/IEC 42001-aligned)
- **Applied ML for SOC operations** — explainable models for threat triage and agentic pipelines for ticket generation

## 🚀 Featured Projects

**[AlertMind — AI-Assisted Mini SOC](https://github.com/opandey1/alertmind)** 🛡️ *(active capstone)*
A working Security Operations Centre built end-to-end in a virtual lab: **Wazuh SIEM** ingesting Windows (**Sysmon**) and Linux (**auditd**) telemetry, with a **25-rule detection pack authored in Sigma and shipped as Wazuh-native rules — every rule mapped to MITRE ATT&CK** and validated through adversary emulation (Atomic Red Team, Impacket) with screenshot-level evidence for each verified detection. On top of it: an **LLM tier-1 triage assistant behind strict guardrails** — PII redaction before any prompt leaves the runner, no autonomous actions, human review on every output, full prompt/response logging — with impact measured honestly: time-to-triage and hallucination rate against ground truth, not vibes.

**[Project KAVACH](https://github.com/opandey1/project-kavach)** 🔍
A solo four-week security engagement for a fictional Indian NBFC, fusing **network forensics** (PCAP triage, hypothesis-driven analysis with confirm/refute verdicts, IOC extraction with confidence ratings) with **web application security assessment** (OWASP Top 10 exploitation, code-level remediation, before/after Semgrep SAST baselines) — synthesized into a joint **STRIDE threat model** and a seven-layer **defence-in-depth proposal** with a board-ready executive readout.

**[AI-SOC-Assistant](https://github.com/opandey1/AI-SOC-Assistant)** — An AI-driven threat hunting pipeline using Random Forest, SHAP, and LangGraph to automate SOC ticket generation with explainable outputs. The alert-summarization core now powers AlertMind's assistant.

**[SentinelScribe](https://github.com/opandey1/SentinelScribe)** — A three-pass GenAI pipeline that transforms raw cybersecurity course audio transcripts into structured, forensically-accurate Markdown study guides.

**[Deep-Learning-Projects](https://github.com/opandey1/Deep-Learning-Projects)** — Iterative CNN optimization achieving >90% on CIFAR-10 and ~73% on CIFAR-100 in PyTorch, using SGD with Nesterov Momentum and Cosine Annealing.

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
![SHAP](https://img.shields.io/badge/-SHAP-9146FF?style=flat)
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

- **PG Certificate, AI/GenAI Powered Cybersecurity**, IIT Roorkee × Futurense — *in progress (Cohort 1)*
- **M.S. Cyber Security Engineering**, University of Southern California — GPA 3.70
- **B.Tech Information Technology** (Honors), The NorthCap University

## 📫 Get in touch

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ojaspandey/)

---

<sub>Open to Senior SOC Engineer, Senior Detection Engineer, and AI Security Engineer roles — and collaborations in AI for security operations, detection engineering, and SOC automation.</sub>
