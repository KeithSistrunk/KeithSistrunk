# Keith Sistrunk — AI Security & Vulnerability Management 🛡️


> Network Security Engineer | AI/RAG Security | OWASP LLM Top 10 | Vulnerability Management

I build security systems and the AI tools that help defend them. 10+ years across Cisco, Palo Alto, FortiGate, and Zscaler — now working at the intersection of AI and security operations.

---

## 🤖 AI Security Projects

### [AuditIQ — CMMC Level 1 RAG Evidence Assistant](https://github.com/KeithSistrunk/auditiq)
[![Live App](https://img.shields.io/badge/Live%20App-auditiq--cmmc.streamlit.app-1565c0?style=flat&logo=streamlit)](https://auditiq-cmmc.streamlit.app)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![OpenAI](https://img.shields.io/badge/OpenAI-GPT--4o-412991?style=flat&logo=openai)](https://openai.com)
[![OWASP LLM](https://img.shields.io/badge/OWASP%20LLM-10%2F10%20Mitigated-2e7d32?style=flat)](https://owasp.org)

AI-powered compliance evidence assistant for CMMC Level 1 self-assessment preparation. Uses RAG (LlamaIndex + OpenAI) to let teams query audit evidence in plain English, identify control gaps across all 17 practices, and generate audit-ready outputs for human review.

- ✅ Full OWASP LLM Top 10 coverage — all 10 risks mitigated
- ✅ Prompt injection detection — 22 known attack patterns blocked
- ✅ File integrity monitoring via SHA-256 hashing
- ✅ Persistent audit logging via Supabase
- ✅ CI/CD via GitHub → Streamlit Cloud

---

### 🎯 RedScope AI — OWASP Web Security Red Team Tool
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![OpenAI](https://img.shields.io/badge/LLM-OpenAI_API-412991?style=flat&logo=openai)](https://openai.com)
[![Streamlit](https://img.shields.io/badge/UI-Streamlit-FF4B4B?style=flat&logo=streamlit&logoColor=white)](https://streamlit.io)
[![OWASP](https://img.shields.io/badge/OWASP-Top%2010-2e7d32?style=flat&logo=owasp&logoColor=white)](https://owasp.org/www-project-top-ten/)
[![Authorized Only](https://img.shields.io/badge/Scope-Authorized%20Targets%20Only-c62828?style=flat&logo=shield&logoColor=white)](https://owasp.org)

AI-powered red team application built to audit web applications against the OWASP Top 10. Used to identify and confirm a live XSS vulnerability (OWASP A03:2021) in AuditIQ production — demonstrating a complete offensive/defensive AI security workflow. Built as a class project in an AI security engineering program.

- ✅ Found a live XSS in production — real finding against AuditIQ, not a lab target
- ✅ Agentic AI red-team scanner — LLM guides testing, explains findings, organizes results
- ✅ OWASP-focused coverage — XSS · SQLi · IDOR / access control · misconfig · exposed files · security headers
- ✅ Evidence-based reporting — Markdown / PDF / HTML output for manual validation
- ✅ Authorized-targets-only by design — scope-consent flow, non-destructive checks
- ✅ Python stack — security checks + HTTP libraries, Streamlit dashboard, LLM via API

---

## 🔍 Automated Vulnerability Management Pipeline

### [Vulnerability Management Program](https://github.com/KeithSistrunk/Vulnerability-Management-Program)
[![Live Demo](https://img.shields.io/badge/Live_Demo-Vulnerability_Dashboard-3FD0C9?style=flat-square)](https://keithsistrunk.github.io/Vulnerability-Management-Program/)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![Tenable](https://img.shields.io/badge/Tenable-API-00558C?style=flat-square)](https://www.tenable.com)
[![Enrichment](https://img.shields.io/badge/Enrichment-KEV_·_EPSS_·_NVD-5BBF8A?style=flat-square)](https://github.com/KeithSistrunk/Vulnerability-Management-Program#4-system-architecture)
[![Scoring](https://img.shields.io/badge/Risk_Scoring-Explainable-A982E8?style=flat-square)](https://github.com/KeithSistrunk/Vulnerability-Management-Program#5-the-risk-scoring-model)


End-to-end VM pipeline built against a live Tenable enterprise instance. CVE ingestion, CVSS/EPSS/KEV risk scoring, automated remediation package generation, Excel dashboard output.

- ✅ Live Tenable API ingestion — no manual CSV exports
- ✅ Threat-intel enrichment — CISA KEV · EPSS · NVD on every CVE
- ✅ Explainable weighted risk scoring — every point auditable
- ✅ Severity-based SLA assignment — Critical 15d · High 30d · Medium 60d · Low 90d
- ✅ Secrets in env vars — least-privilege, read-only Tenable key
- ✅ Real scan data gitignored — public demo runs on synthetic data only

---

## 🕵️ Threat Hunting & Security Operations

### [Threat Hunt: Unauthorized Tor Usage](https://github.com/KeithSistrunk/threat-hunting-scenario-tor)
[![EDR](https://img.shields.io/badge/EDR-Microsoft_Defender-0078D4?style=flat-square&logo=microsoft&logoColor=white)](https://www.microsoft.com/security)
[![KQL](https://img.shields.io/badge/Query-KQL-512BD4?style=flat-square)](https://learn.microsoft.com/azure/data-explorer/kusto/query/)
[![Azure Lab](https://img.shields.io/badge/Lab-Azure_Win10-0089D6?style=flat-square&logo=microsoftazure&logoColor=white)](https://azure.microsoft.com)

End-to-end threat hunt detecting unauthorized Tor Browser use on a corporate endpoint, built on a Microsoft Defender for Endpoint cyber range. Reconstructed the full activity chain — download, silent install, execution, and outbound connections to known Tor entry nodes — directly from raw EDR telemetry.

- ✅ Hunted across `DeviceFileEvents`, `DeviceProcessEvents`, and `DeviceNetworkEvents` with custom KQL
- ✅ Reconstructed the timeline — installer download → silent install → browser launch → Tor node connections
- ✅ Surfaced concrete IoCs — portable Tor installer, `tor.exe`, `tor-shopping-list.txt`, known Tor ports
- ✅ Delivered an audit-ready hunt report with evidence and a notify-management workflow

---

## 🛡️ Security Technical Implementation

### [STIG Remediation Automation](https://github.com/KeithSistrunk/Automation)
[![PowerShell](https://img.shields.io/badge/PowerShell-STIG_Remediation-5391FE?style=flat-square&logo=powershell&logoColor=white)](https://learn.microsoft.com/powershell/)
[![DISA STIG](https://img.shields.io/badge/Baseline-DISA_STIG-00558C?style=flat-square)](https://public.cyber.mil/stigs/)

PowerShell automation that hardens Windows endpoints against DISA STIG baselines — driving a single host from 205 open findings down to 23 in one pass.

- ✅ Automated STIG remediation — 205 → 23 findings (~89% reduction)
- ✅ PowerShell-based and repeatable across hosts
- ✅ Maps to RMF / continuous-monitoring workflows (hardening baselines, POA&M)

### 🔒 Cisco IOS Hardening Checker
[![Cisco](https://img.shields.io/badge/Cisco-IOS_·_IOS--XE-1BA0D7?style=flat-square&logo=cisco&logoColor=white)](https://www.cisco.com)
[![Python](https://img.shields.io/badge/Python-stdlib_only-3776AB?style=flat-square&logo=python&logoColor=white)](https://www.python.org)
[![CMMC / STIG](https://img.shields.io/badge/Baseline-CMMC_·_STIG-00558C?style=flat-square)](https://public.cyber.mil/stigs/)

Read-only Python auditor that flags CMMC / STIG-style misconfigurations in a Cisco IOS / IOS-XE config — weak password encryption, missing session timeouts, plaintext management (Telnet/HTTP), absent logging, and default SNMP communities — with line-referenced findings and remediation guidance.

- ✅ 12 hardening controls checked, each with PASS / WARN / FAIL and a fix
- ✅ Secrets auto-redacted in output; non-zero exit code for CI gating
- ✅ Stdlib only, no device connection — parses an offline config export

---

## 🔗 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-keith--sistrunk-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/keith-sistrunk)
[![AuditIQ Live](https://img.shields.io/badge/AuditIQ-Live%20Demo-1565c0?style=flat&logo=streamlit)](https://auditiq-cmmc.streamlit.app)
