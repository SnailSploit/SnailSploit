<img src="banner.png" alt="SnailSploit Banner" width="100%"/>

<div align="center">

# SnailSploit

**GenAI Security Researcher · AI Red Teamer · Offensive Security Writer**

[![Website](https://img.shields.io/badge/snailsploit.com-000?style=for-the-badge&logo=astro&logoColor=white)](https://snailsploit.com)
[![The Jailbreak Chef](https://img.shields.io/badge/The_Jailbreak_Chef-FF6B35?style=for-the-badge&logo=fireship&logoColor=white)](https://thejailbreakchef.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kaiaizen)

</div>

---

I'm Kai Aizen — independent security researcher focused on adversarial AI, LLM red teaming, and the intersection of social engineering and prompt injection. I build frameworks and tooling for structured AI safety testing.

`Creator of AATMF · Author of Adversarial Minds · 19 CVEs · Linux kernel contributor · Hakin9 Contributing Author`

---

## 🔴 Frameworks & Tooling

| Project | Description | |
|---------|-------------|:-:|
| [**AATMF v3.1**](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) | Adversarial AI Threat Modeling Framework — 20 tactics, ~240 techniques. Maps to OWASP LLM Top-10, NIST AI RMF, MITRE ATLAS. | [![AATMF](https://img.shields.io/badge/AATMF-v3.1-red?style=flat-square)](https://snailsploit.com/frameworks/aatmf/core-tactics/) |
| [**AATMF Red Teaming Toolkit**](https://github.com/SnailSploit/aatmf-toolkit) | Python CLI for systematic LLM safety testing — three-layer eval pipeline, defense fingerprinting, decay tracking, attack chain planning. | [![NEW](https://img.shields.io/badge/NEW-2026-brightgreen?style=flat-square)]() |
| [**LLM Red Teamer's Playbook**](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) | Diagnostic methodology for bypassing LLM defense layers — input filters → alignment → identity → output → agentic trust. | |

## 🧪 Experiments & PoCs

| Project | Description |
|---------|-------------|
| [**ChatGPT-DNS-Exfill**](https://github.com/SnailSploit/ChatGPT-DNS-Exfill) | DNS exfiltration via ChatGPT Canvas — rendered content triggers DNS lookups without HTTP requests. |
| [**chatgpt-rce-dns**](https://github.com/SnailSploit/chatgpt-rce-dns) | DNS exfiltration and Python Pickle RCE attack chains in AI code execution sandboxes. |

## 🛠️ Offensive Tools

| Tool | Description |
|------|-------------|
| [**Burp MCP Toolkit**](https://github.com/SnailSploit/Burp-MCP-Security-Analysis-Toolkit) | MCP security analysis for Burp Suite — prompt injection and tool poisoning testing via Model Context Protocol. |
| [**SnailHunter**](https://github.com/SnailSploit/SnailHunter) | AI-powered bug bounty automation — LLM analysis combined with traditional security scanning. |
| [**KubeRoast**](https://github.com/SnailSploit/KubeRoast_v1) | Red-team Kubernetes misconfiguration and attack-path scanner. |
| [**Xposure**](https://github.com/SnailSploit/Xposure) | Autonomous credential intelligence platform for attack surface recon. |
| [**SnailSploit Recon**](https://github.com/SnailSploit/SnailSploit_Recon_extension) | Chrome MV3 extension for passive recon and bug bounty automation. |
| [**ZenFlood**](https://github.com/SnailSploit/ZenFlood) | Low-bandwidth stress testing — modernized Slowloris. |
| [**Claude-Red**](https://github.com/SnailSploit/Claude-Red) | Curated offensive security skills library for the Claude skills system. |
| [**SnailObfuscator**](https://github.com/SnailSploit/SnailObfuscator) | Structurally-aware code obfuscation engine. |

## 🛡️ CVEs

| CVE | Target | Type | Severity |
|-----|--------|------|:--------:|
| [CVE-2026-3288](https://github.com/SnailSploit/CVE-2026-3288) | [Kubernetes](https://github.com/advisories/GHSA-c56h-j8gw-3v54) | Config Injection → RCE | **High (8.8)** |
| [CVE-2026-1313](https://github.com/SnailSploit/CVE-2026-1313) | MimeTypes Link Icons (WP) | SSRF via crafted post content | **High (8.3)** |
| [CVE-2026-30911](https://github.com/SnailSploit/CVE-2026-30911) | [Apache Airflow Core](https://github.com/apache/airflow) | Missing Authorization — HITL Endpoints (v3.1.0–3.1.7) | **High (8.1)** |
| [CVE-2026-31899](https://github.com/SnailSploit/CVE-2026-31899) | [CairoSVG](https://github.com/Kozea/CairoSVG/security/advisories/GHSA-f38f-5xpm-9r7c) | Exponential DoS — recursive `<use>` amplification | **High (7.5)** |
| [CVE-2026-32809](https://github.com/SnailSploit/CVE-2026-32809) | [ouch](https://github.com/ouch-org/ouch/security/advisories/GHSA-pcw6-cg54-qvm8) | Symlink escape → arbitrary file overwrite | **High (7.4)** |
| (pending) | TelSender (WP) | Unauthenticated Stored XSS via Telegram Chat Title | **High (7.2)** |
| [CVE-2025-9776](https://github.com/SnailSploit/CVE-2025-9776) | CatFolders (WP) | SQL Injection via CSV Import | Medium (6.5) |
| [CVE-2026-33693](https://github.com/SnailSploit/CVE-2026-33693) | [Lemmy](https://github.com/LemmyNet/activitypub-federation-rust/security/advisories/GHSA-q537-8fr5-cw35) | SSRF — 0.0.0.0 bypass | Medium (6.5) |
| [CVE-2026-32885](https://github.com/SnailSploit/CVE-2026-32885) | [ddev](https://github.com/ddev/ddev/security/advisories/GHSA-x2xq-qhjf-5mvg) | ZipSlip path traversal in archive extraction | Medium (6.5) |
| [CVE-2025-12163](https://github.com/SnailSploit/CVE-2025-12163) | Omnipress (WP) | Stored XSS | Medium (6.4) |
| [CVE-2026-0811](https://github.com/SnailSploit/CVE-2026-0811) | Advanced CF7 DB (WP) | CSRF → Form Entry Deletion | Medium (5.4) |
| [CVE-2026-1314](https://github.com/SnailSploit/CVE-2026-1314) | 3D FlipBook (WP) | Missing Auth → Data Exposure | Medium (5.3) |
| [CVE-2026-3594](https://github.com/SnailSploit/CVE-2026-3594) | Riaxe Product Customizer (WP) | Unauthenticated Info Disclosure via /orders | Medium (5.3) |
| [CVE-2025-11171](https://github.com/SnailSploit/CVE-2025-11171) | Chartify (WP) | Missing Authentication for Admin Function | Medium (5.3) |
| [CVE-2025-11174](https://github.com/SnailSploit/CVE-2025-11174) | Document Library Lite (WP) | Missing Auth → Info Disclosure | Medium (5.3) |
| [CVE-2026-32794](https://github.com/SnailSploit/CVE-2026-32794) | [Apache Airflow Databricks Provider](https://github.com/apache/airflow/security/advisories) | TLS Certificate Verification Bypass → MitM | Medium (4.8) |
| [CVE-2026-0814](https://github.com/SnailSploit/CVE-2026-0814) | Advanced CF7 DB (WP) | Missing Auth → Subscriber+ Export | Medium (4.3) |
| [CVE-2025-12030](https://github.com/SnailSploit/CVE-2025-12030) | ACF to REST API (WP) | IDOR → Contributor+ Field Modification | Medium (4.3) |
| [CVE-2026-1208](https://github.com/SnailSploit/CVE-2026-1208) | Welcart (WP) | CSRF → Settings Update | Medium (4.3) |

## 🔓 Security Advisories (GHSAs)

| Advisory | Target | Type | Severity |
|----------|--------|------|:--------:|
| [GHSA-f38f-5xpm-9r7c](https://github.com/advisories/GHSA-f38f-5xpm-9r7c) | [CairoSVG](https://github.com/Kozea/CairoSVG/security/advisories/GHSA-f38f-5xpm-9r7c) | Exponential DoS — recursive `<use>` element amplification | **High (7.5)** |
| [GHSA-j425-whc4-4jgc](https://github.com/SnailSploit/OpenClaw-Env-Injection) | [OpenClaw](https://github.com/openclaw/openclaw/security/advisories/GHSA-j425-whc4-4jgc) (309k⭐) | system.run env override RCE — allowlist bypass via GIT_SSH_COMMAND, editor hooks, GIT_CONFIG_* | Medium (6.3) |
| [GHSA-9jmq-9m65-3fhx](https://github.com/advisories/GHSA-9jmq-9m65-3fhx) | [dagster-io/dagster](https://github.com/dagster-io/dagster) | Arbitrary code exec via pickle deserialization in IO managers + Databricks | — |
| [GHSA-pph4-qh43-9qm6](https://github.com/advisories/GHSA-pph4-qh43-9qm6) | [vllm-project/vllm](https://github.com/vllm-project/vllm) | RCE via unauthenticated TCPStore Pickle deserialization (V1 Engine) | — |
| [GHSA-gwmc-ch8w-qhx5](https://github.com/advisories/GHSA-gwmc-ch8w-qhx5) | [vllm-project/vllm](https://github.com/vllm-project/vllm) | RCE via TCPStore Pickle deserialization (StatelessProcessGroup) | — |
| [GHSA-c64x-w74w-4h53](https://github.com/advisories/GHSA-c64x-w74w-4h53) | [FlowiseAI/Flowise](https://github.com/FlowiseAI/Flowise) | Unauthenticated code exec via prediction API auth whitelist bypass | — |
| [GHSA-9vqm-j6v3-2xr4](https://github.com/advisories/GHSA-9vqm-j6v3-2xr4) | [juspay/hyperswitch](https://github.com/juspay/hyperswitch) | SSRF via merchant webhook URL | — |

## 🐧 Kernel Research

| Finding | Component | Type | Status |
|---------|-----------|------|:------:|
| [io_uring/zcrx Race Condition](https://snailsploit.com/security-research/general/io-uring-zcrx-race-condition/) | Linux kernel io_uring/zcrx | Race Condition → Double-Free → OOB Write | ✅ [Upstream](https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/commit/?id=003049b1c4fb8aabb93febb7d1e49004f6ad653b), backported to [v6.18.16](https://cdn.kernel.org/pub/linux/kernel/v6.x/ChangeLog-6.18.16) + v6.19 |

## 🔧 Additional Merged Security Fixes

| PR | Target | Type | Status |
|----|--------|------|:------:|
| [concourse/concourse#9486](https://github.com/concourse/concourse/pull/9486) | Concourse CI | Symlink breakout — unvalidated symlink targets in tar extraction | ✅ Merged, shipped in v8.1.1 |

---

<div align="center">

[![SnailSploit](https://img.shields.io/badge/Read_the_research-snailsploit.com-black?style=for-the-badge)](https://snailsploit.com)

</div>
