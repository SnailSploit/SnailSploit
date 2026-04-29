<div align="center">

![SnailSploit Banner](https://github.com/SnailSploit/SnailSploit/raw/main/banner.png)

# SnailSploit · Kai Aizen

### *Same attack. Different substrate.*

[![Website](https://img.shields.io/badge/snailsploit.com-000?style=for-the-badge&logo=astro&logoColor=white)](https://snailsploit.com)
[![The Jailbreak Chef](https://img.shields.io/badge/The_Jailbreak_Chef-FF6B35?style=for-the-badge&logo=fireship&logoColor=white)](https://thejailbreakchef.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kaiaizen)
[![X](https://img.shields.io/badge/X-000?style=for-the-badge&logo=x&logoColor=white)](https://x.com/SnailSploit)

![Linux Kernel](https://img.shields.io/badge/Linux_Kernel-5_mainline_patches-A81D33?style=flat-square&logo=linux&logoColor=white)
![CVEs](https://img.shields.io/badge/CVEs-22_published-red?style=flat-square)
![GHSA](https://img.shields.io/badge/GHSA-1_advisory-orange?style=flat-square)
![Hakin9](https://img.shields.io/badge/Hakin9-Contributing_Author-blueviolet?style=flat-square)
![NVD](https://img.shields.io/badge/MITRE/NVD-Contributor-005DAA?style=flat-square)

</div>

---

Independent offensive security researcher. I break production systems — Linux kernel, Kubernetes, container runtimes, OSS libraries, and the LLMs increasingly woven through them — then publish the methodology. Frameworks for structured adversarial-AI red teaming. Tooling for systematic vulnerability discovery. Books and articles for the human layer.

`Creator of AATMF / P.R.O.M.P.T / SEF · Author of Adversarial Minds · Hakin9 contributing author · Linux kernel contributor`

---

## Linux Kernel Contributions

Five mainline-merged patches across networking, IPC, Bluetooth, RDMA, and `io_uring` — reviewed and accepted through the standard kernel maintainer process into Linus's tree.

| Subsystem | Vulnerability | Status |
| --- | --- | --- |
| `io_uring/zcrx` | `user_ref` race → double-free → OOB write | [Mainline 7.0-rc1](https://git.kernel.org/pub/scm/linux/kernel/git/stable/linux.git/commit/?id=003049b1c4fb8aabb93febb7d1e49004f6ad653b) · stable backports [6.18.16](https://cdn.kernel.org/pub/linux/kernel/v6.x/ChangeLog-6.18.16) + 6.19.6 |
| `net/tipc` | `tipc_mon_peer_up` UAF vs bearer teardown | [Mainline](https://lore.kernel.org/all/?q=tipc+tipc_mon_peer_up+bearer+teardown) |
| `Bluetooth` | `hci_conn` UAF in `create_big_sync` / `create_big_complete` | [Mainline](https://lore.kernel.org/all/?q=Bluetooth+hci_conn+create_big_sync) |
| `RDMA/ionic` | Unbounded `node_desc` sysfs read via `%.64s` | [Mainline](https://lore.kernel.org/all/?q=RDMA+ionic+node_desc+sysfs) |
| `net/rtnetlink` | `ifla_vf_broadcast` stack infoleak (zero init missing) | [Mainline](https://lore.kernel.org/all/?q=ifla_vf_broadcast+rtnl_fill_vfinfo) |

[All patches on lore.kernel.org →](https://lore.kernel.org/all/?q=Kai+Aizen)

---

## AI Security Research

Original research — published at [snailsploit.com](https://snailsploit.com), Hakin9 Magazine, and Medium.

| Research | Summary |
| --- | --- |
| [**Self-Replicating Memory Worm**](https://snailsploit.com/ai-security/self-replicating-memory-worm/) | Adversarial self-replicating prompt that survives across sessions and propagates via long-term memory writes — the AI-worm primitive applied to persistent agent state. |
| [**Memory Injection Through Nested Skills**](https://snailsploit.com/ai-security/prompt-injection/memory-injection-nested-skills/) | Novel persistence chain — skill injection + memory poisoning = self-healing autonomous implant. Validated against DVWA and Juice Shop in agent harness. |
| [**ChatGPT Canvas DNS Exfiltration**](https://github.com/SnailSploit/ChatGPT-DNS-Exfill) | DNS exfiltration via rendered Canvas content — triggers lookups without outbound HTTP. |
| [**ChatGPT Sandbox: Pickle RCE + DNS Chain**](https://github.com/SnailSploit/chatgpt-rce-dns) | Pickle deserialization RCE chained with DNS exfil to break out of the Code Interpreter sandbox. |
| [**MCP vs A2A Attack Surface**](https://snailsploit.com/ai-security/mcp-vs-a2a-attack-surface/) | Comparative threat model: where Model Context Protocol and Agent-to-Agent diverge in trust boundaries. |
| [**The 30% Blind Spot — LLM Safety Judges**](https://snailsploit.com/ai-security/rai-judge-blind-spots/) | Empirical study showing LLM-as-judge safety classifiers miss ~30% of adversarial output classes. |
| [**Adversarial Prompting: Complete Guide**](https://snailsploit.com/ai-security/adversarial-prompting/) | End-to-end methodology covering direct, indirect, multi-turn, and agentic prompt injection. |

---

## Frameworks & Tooling

| Project | Description | |
| --- | --- | --- |
| [**AATMF v3.1**](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) | Adversarial AI Threat Modeling Framework — 15 tactics, 240+ techniques, 2,150+ procedures. Mapped to NIST AI RMF and MITRE ATLAS. | [![Stars](https://img.shields.io/github/stars/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework?style=flat-square&logo=github&label=Stars)](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) |
| [**AATMF Red Teaming Toolkit**](https://github.com/SnailSploit/aatmf-toolkit) | Python CLI for systematic LLM safety testing — three-layer eval pipeline, defense fingerprinting, decay tracking, attack chain planning. | [![Stars](https://img.shields.io/github/stars/SnailSploit/aatmf-toolkit?style=flat-square&logo=github&label=Stars)](https://github.com/SnailSploit/aatmf-toolkit) |
| [**LLM Red Teamer's Playbook**](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) | Diagnostic methodology for bypassing LLM defense layers — input filters → alignment → identity → output → agentic trust. | [![Stars](https://img.shields.io/github/stars/SnailSploit/The-LLM-Red-Teamer-s-Playbook?style=flat-square&logo=github&label=Stars)](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) |
| [**Claude-Red**](https://github.com/SnailSploit/Claude-Red) | Curated offensive security skills library for the Claude skills system — 38 SKILL.md files spanning SQLi, shellcode, EDR evasion, exploit dev. | [![Stars](https://img.shields.io/github/stars/SnailSploit/Claude-Red?style=flat-square&logo=github&label=Stars)](https://github.com/SnailSploit/Claude-Red) |

---

## Offensive Tools

| Tool | Description |
| --- | --- |
| [**Burp MCP Toolkit**](https://github.com/SnailSploit/Burp-MCP-Security-Analysis-Toolkit) | MCP security analysis for Burp Suite — prompt injection and tool poisoning testing via Model Context Protocol. |
| [**SnailHunter**](https://github.com/SnailSploit/SnailHunter) | AI-powered bug bounty automation — LLM analysis combined with traditional security scanning. |
| [**KubeRoast**](https://github.com/SnailSploit/KubeRoast_v1) | Red-team Kubernetes misconfiguration & attack-path scanner. |
| [**Xposure**](https://github.com/SnailSploit/Xposure) | Autonomous credential intelligence platform for attack-surface recon. |
| [**SnailSploit Recon**](https://github.com/SnailSploit/SnailSploit_Recon_extension) | Chrome MV3 extension — passive recon, security headers, IP intel, CPE→CVE enrichment. |
| [**SnailPath**](https://github.com/SnailSploit/SnailPath) | Async directory & route discovery — HTTP/2, soft-404 suppression, JS/sourcemap mining. |
| [**ZenFlood**](https://github.com/SnailSploit/ZenFlood) | Low-bandwidth stress testing — modernized Slowloris. |
| [**SnailObfuscator**](https://github.com/SnailSploit/SnailObfuscator) | Structurally-aware code obfuscation engine. |
| [**Awesome-Snail-OSINT**](https://github.com/SnailSploit/Awesome-Snail-OSINT) | Curated OSINT resource collection for offensive recon. |

---

## CVEs

Sorted by blast radius — shared infrastructure first, single-vendor plugins last.

### Container & Cluster Infrastructure

| CVE | Target | Type | Severity |
| --- | --- | --- | --- |
| [CVE-2026-3288](https://github.com/SnailSploit/CVE-2026-3288) | Kubernetes ingress-nginx | Config injection → RCE | **High (8.8)** |

### Apache Foundation

| CVE | Target | Type | Severity |
| --- | --- | --- | --- |
| [CVE-2026-30911](https://nvd.nist.gov/vuln/detail/CVE-2026-30911) | Apache Airflow Core | Missing authentication | **High (8.1)** |
| [CVE-2026-32794](https://nvd.nist.gov/vuln/detail/CVE-2026-32794) | Apache Airflow (Databricks provider) | TLS verification bypass | Medium (4.8) |

### Cross-Language OSS

| CVE | Target | Lang | Type | Severity |
| --- | --- | --- | --- | --- |
| [CVE-2026-31899](https://nvd.nist.gov/vuln/detail/CVE-2026-31899) | CairoSVG | Python | Exponential DoS — recursive amplification | **High (7.5)** |
| [CVE-2026-32809](https://nvd.nist.gov/vuln/detail/CVE-2026-32809) | ouch-org/ouch | Rust | Symlink escape — arbitrary file overwrite | **High (7.4)** |
| [CVE-2026-33693](https://nvd.nist.gov/vuln/detail/CVE-2026-33693) | activitypub-federation-rust | Rust | SSRF — `0.0.0.0` bypass in fediverse federation | Medium (6.5) |
| [CVE-2026-32885](https://nvd.nist.gov/vuln/detail/CVE-2026-32885) | ddev/ddev | Go | ZipSlip — path traversal in archive extraction | Medium (6.5) |

### WordPress Plugin Ecosystem

| CVE | Target | Type | Severity |
| --- | --- | --- | --- |
| [CVE-2026-3596](https://nvd.nist.gov/vuln/detail/CVE-2026-3596) | Riaxe Product Customizer | Privilege escalation | **Critical (9.8)** |
| [CVE-2026-1313](https://nvd.nist.gov/vuln/detail/CVE-2026-1313) | MimeTypes Link Icons | SSRF | **High (8.3)** |
| [CVE-2026-3599](https://nvd.nist.gov/vuln/detail/CVE-2026-3599) | Riaxe Product Customizer | SQL injection | **High (7.5)** |
| [CVE-2025-9776](https://github.com/SnailSploit/CVE-2025-9776) | CatFolders | SQL injection via CSV import | Medium (6.5) |
| [CVE-2025-12163](https://github.com/SnailSploit/CVE-2025-12163) | OmniPress | Stored XSS | Medium (6.4) |
| [CVE-2026-2717](https://nvd.nist.gov/vuln/detail/CVE-2026-2717) | HTTP Headers | CRLF injection | Medium (5.5) |
| [CVE-2026-0811](https://nvd.nist.gov/vuln/detail/CVE-2026-0811) | Advanced CF7 DB | CSRF | Medium (5.4) |
| [CVE-2026-1314](https://nvd.nist.gov/vuln/detail/CVE-2026-1314) | 3D FlipBook | Missing authentication | Medium (5.3) |
| [CVE-2026-3594](https://nvd.nist.gov/vuln/detail/CVE-2026-3594) | Riaxe Product Customizer | Information disclosure | Medium (5.3) |
| [CVE-2026-3595](https://nvd.nist.gov/vuln/detail/CVE-2026-3595) | Riaxe Product Customizer | Unauthenticated user deletion | Medium (5.3) |
| [CVE-2025-11171](https://github.com/SnailSploit/CVE-2025-11171) | Chartify | Missing authentication | Medium (5.3) |
| [CVE-2025-11174](https://github.com/SnailSploit/CVE-2025-11174) | Document Library Lite | Unauth info disclosure | Medium (5.3) |
| [CVE-2026-0814](https://nvd.nist.gov/vuln/detail/CVE-2026-0814) | Advanced CF7 DB | Missing authentication | Medium (4.3) |
| [CVE-2025-12030](https://github.com/SnailSploit/CVE-2025-12030) | ACF to REST API | IDOR | Medium (4.3) |
| [CVE-2026-1208](https://github.com/SnailSploit/CVE-2026-1208) | Welcart Friendly Functions | CSRF → settings update | Medium (4.3) |

Plus: TelSender — stored XSS that resulted in [vendor-side plugin removal](https://www.wordfence.com/threat-intel/vulnerabilities/researchers/kai-aizen).

---

## Security Advisories

| Advisory | Target | Type | Severity |
| --- | --- | --- | --- |
| [GHSA-j425-whc4-4jgc](https://github.com/advisories/GHSA-j425-whc4-4jgc) | [OpenClaw](https://github.com/openclaw/openclaw/security/advisories/GHSA-j425-whc4-4jgc) | `system.run` env override RCE — allowlist bypass via `GIT_SSH_COMMAND`, editor hooks, `GIT_CONFIG_*` | Medium (6.3) |

---

## Source-Tree Contributions

| Project | Contribution | Status |
| --- | --- | --- |
| [concourse/concourse#9486](https://github.com/concourse/concourse/pull/9486) | Symlink breakout fix | Merged in v8.1.1 |

---

<div align="center">

[![Read the research](https://img.shields.io/badge/Read_the_research-snailsploit.com-000?style=for-the-badge&logo=astro&logoColor=white)](https://snailsploit.com)
[![Hire / Collaborate](https://img.shields.io/badge/Hire_/_Collaborate-Get_in_touch-FF6B35?style=for-the-badge)](mailto:kai@snailsploit.com)

</div>
