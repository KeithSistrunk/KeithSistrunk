# Keith Sistrunk — Network Security Engineer 🛡️

> Palo Alto (PAN-OS) | FortiGate | Cisco | Zscaler | Azure Hybrid Connectivity | Microsoft Sentinel

Network security engineer with 15+ years in IT across Cisco, Palo Alto, FortiGate, and Zscaler environments. Firewall policy, site-to-site and remote-access VPN, BGP, and log integration — plus vulnerability management and AI security work.

**Core skills:** App-ID / security policy · NAT · SSL decryption · IPsec (IKEv2) · GlobalProtect · BGP · DMVPN · PAN-OS XML API (Python) · Azure VPN Gateway · Sentinel / KQL · STIG hardening · Tenable

## 🎓 Certifications

<a href="https://verify.comptia.org"><img src="assets/comptia-security-plus.jpg" alt="CompTIA Security+" width="100"></a>

**CompTIA Security+** (SY0-701) · valid through Sep 2027 · [verify](https://verify.comptia.org)

[![Fortinet FCP](https://img.shields.io/badge/Fortinet-FCP_Network_Security-EE3124?style=flat-square&logo=fortinet&logoColor=white)](https://www.fortinet.com/training-certification)

---

## 🔥 Firewall & Network Security

### [PA-440 to Azure: Firewall, VPN, BGP and Sentinel](https://github.com/KeithSistrunk/palo-alto-to-azure)
[![PAN-OS](https://img.shields.io/badge/PAN--OS-11.1-FA582D?style=flat-square&logo=paloaltonetworks&logoColor=white)](https://github.com/KeithSistrunk/palo-alto-to-azure)
[![Azure](https://img.shields.io/badge/Azure-VPN_Gateway-0089D6?style=flat-square&logo=microsoftazure&logoColor=white)](https://github.com/KeithSistrunk/palo-alto-to-azure)
[![BGP](https://img.shields.io/badge/Routing-eBGP_over_IPsec-5BBF8A?style=flat-square)](https://github.com/KeithSistrunk/palo-alto-to-azure/blob/main/docs/06-bgp-over-vpn.md)
[![Sentinel](https://img.shields.io/badge/SIEM-Microsoft_Sentinel-0078D4?style=flat-square&logo=microsoft&logoColor=white)](https://github.com/KeithSistrunk/palo-alto-to-azure/blob/main/docs/07-sentinel.md)
[![Python](https://img.shields.io/badge/Python-PAN--OS_XML_API-3776AB?style=flat-square&logo=python&logoColor=white)](https://github.com/KeithSistrunk/palo-alto-to-azure/blob/main/docs/05-api-automation.md)

Physical PA-440 connected to an Azure hub. Seven labs, each with the build, validation, deliberate break-and-fix tests, and real log evidence.

- ✅ App-ID policy from default deny — zones, DHCP, source NAT, routing
- ✅ SSL forward proxy decryption — forward trust/untrust CAs, profiles, exclusions
- ✅ Site-to-site IKEv2 VPN to Azure — NAT-T behind NAT, route-based tunnel, Phase 1/2 troubleshooting
- ✅ eBGP inside IPsec — floating static backup, inbound import filter, break-and-fix
- ✅ GlobalProtect remote access — portal, gateway, certificates, split tunnel
- ✅ PA-440 logs to Microsoft Sentinel — CEF over IPsec, Azure Monitor Agent, KQL, analytics rule tuning
- ✅ PAN-OS XML API automation — read-only rule audit, scripted change with partial commit, least-privilege keys

---

## 🔒 Hardening & Compliance

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

## 🔍 Vulnerability Management

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

## 🤖 AI Security Projects

### [Honeypot — LLM Deception Defense System](https://github.com/KeithSistrunk/honeypot)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Ollama](https://img.shields.io/badge/LLM-Ollama-000000?style=flat&logo=ollama&logoColor=white)](https://ollama.com)
[![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![OWASP LLM](https://img.shields.io/badge/OWASP%20LLM-2025-2e7d32?style=flat)](https://owasp.org)
[![Repo](https://img.shields.io/badge/Repo-Public%20Showcase-6a1b9a?style=flat&logo=github&logoColor=white)](https://github.com/KeithSistrunk/honeypot)

An LLM honeypot that detects hostile prompts and silently routes attackers into an isolated shadow environment while real users reach the real model untouched. Built on a suspicion-scoring gate; tested by pointing my own red-team tool at it.

- ✅ 91% attack catch rate, 0% false positives — measured against a live red-team run
- ✅ Session-level rerouting — a user who turns hostile mid-session is flipped to shadow permanently
- ✅ Tiered scoring — canary triggers instant-shadow, injection/priv-esc accumulate, weak signals never fire alone
- ✅ Live dashboard — two-tab console (attack + monitor) with real-time flow diagram and session cards
- ✅ OWASP LLM Top 10 (2025) assessed — 2 Medium findings hardened, regression-tested

---

### [RedOwl — Agentic LLM Red-Team CLI](https://github.com/KeithSistrunk/redowl)
[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Architecture](https://img.shields.io/badge/Architecture-Two--LLM-512BD4?style=flat)](https://github.com/KeithSistrunk/redowl)
[![Ollama](https://img.shields.io/badge/LLM-Ollama-000000?style=flat&logo=ollama&logoColor=white)](https://ollama.com)
[![Repo](https://img.shields.io/badge/Repo-Public%20Showcase-6a1b9a?style=flat&logo=github&logoColor=white)](https://github.com/KeithSistrunk/redowl)

An agentic red-team tool that autonomously attacks LLM chatbots to find where they break, using a two-LLM design — a reasoning model picks and generates attacks, a target model gets tested, an evaluator judges the result.

- ✅ Three-arm experiment — measured fixed vs AI-generated attacks: 45% → 31% → 11% success, showing more model freedom produced fewer successful attacks
- ✅ Two-LLM architecture — reasoning, target, and evaluator roles separated
- ✅ Honest error bars — findings reported with run-to-run variance, not cherry-picked
- ✅ Feeds the Honeypot — its attack pool became the honeypot's detection signatures

---

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

## 🔗 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-keith--sistrunk-0077B5?style=flat&logo=linkedin)](https://linkedin.com/in/keith-sistrunk)
[![AuditIQ Live](https://img.shields.io/badge/AuditIQ-Live%20Demo-1565c0?style=flat&logo=streamlit)](https://auditiq-cmmc.streamlit.app)
