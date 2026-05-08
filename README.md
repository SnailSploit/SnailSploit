<p align="center">
  <a href="https://snailsploit.com">
    <img src="https://github.com/SnailSploit/SnailSploit/raw/main/banner.png" alt="SnailSploit — Same Attack. Different Substrate." width="100%">
  </a>
</p>

<p align="center">
  <strong>GenAI Security Researcher · AI Red Teamer · Offensive Security Writer</strong>
</p>

<p align="center">
  <a href="https://snailsploit.com"><img src="https://img.shields.io/badge/snailsploit.com-000?style=for-the-badge&logo=astro&logoColor=white" alt="Website"></a>
  <a href="https://thejailbreakchef.com"><img src="https://img.shields.io/badge/The_Jailbreak_Chef-FF6B35?style=for-the-badge&logo=fireship&logoColor=white" alt="The Jailbreak Chef"></a>
  <a href="https://linkedin.com/in/kaiaizen"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"></a>
  <a href="https://medium.com/@snailsploit"><img src="https://img.shields.io/badge/Medium-000?style=for-the-badge&logo=medium&logoColor=white" alt="Medium"></a>
</p>

---

I'm Kai Aizen — independent offensive security researcher. I break production systems — Linux kernel, Kubernetes, container runtimes, OSS libraries, and the LLMs increasingly woven through them — then publish the methodology.

Social engineering and prompt injection are the same attack class, executed against different substrates. The frameworks, tooling, and research below all trace back to that thesis.

```
Creator of AATMF / P.R.O.M.P.T / SEF · Author of Adversarial Minds
20+ CVEs · Linux kernel contributor · Hakin9 contributing author
OWASP GenAI Security Project 2026 roadmap · NVD contributor
```

---

## 🔴 Frameworks & Tooling

| Project | Description |
|---|---|
| [**AATMF v3.1**](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) | Adversarial AI Threat Modeling Framework — 20 tactics, 240+ techniques, 2,152+ procedures, 4,980+ prompts. Crosswalks to OWASP LLM Top-10, NIST AI RMF, MITRE ATLAS, EU AI Act. On OWASP GenAI Security 2026 roadmap. YARA + Sigma detection signatures included. |
| [**AATMF Toolkit**](https://github.com/SnailSploit/aatmf-toolkit) | Python CLI for systematic LLM safety testing — three-layer evaluation pipeline, defense fingerprinting, regression tracking, attack chain planning. Mapped to the full AATMF taxonomy. |
| [**Claude-Red**](https://github.com/SnailSploit/Claude-Red) | Curated library of 38+ offensive security skills for the Claude skills system. Drop a `SKILL.md` into your environment and Claude operates as a specialist — SQLi to shellcode, EDR evasion to ADCS abuse. Trigger-loaded on demand; zero context cost for unused skills. |
| [**LLM Red Teamer's Playbook**](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) | Diagnostic methodology for bypassing LLM defense layers — input filters → alignment → identity → output → agentic trust. Mapped to AATMF taxonomy. |
| [**Burp MCP Toolkit**](https://github.com/SnailSploit/Burp-MCP-Security-Analysis-Toolkit) | Skills-based security analysis framework combining Burp Suite traffic capture with Claude Code reasoning via MCP. Expert pentest methodology encoded into reusable skill files. |
| [**JystDastIt**](https://github.com/SnailSploit/JystDastIt) | The Burp You Can Afford — open-source CLI DAST toolkit for web application vulnerability scanning and XSS detection. |
| [**SnailObfuscator**](https://github.com/SnailSploit/SnailObfuscator) | Structurally-aware code obfuscation engine — polymorphic payload generation that bypasses static and behavioral detection. |
| [**P.R.O.M.P.T**](https://snailsploit.com/frameworks/prompt/) | Adversarial prompt engineering methodology — structured attack phases with Cialdini influence principles and PHLRA context injection. |
| [**SEF**](https://snailsploit.com/frameworks/sef/) | Social Engineering Framework — organizational gap analysis (Authority / Process / Trust / Pressure / Knowledge), pretext selection, MITRE ATT&CK mapping. |

---

## 🧪 Research

Published at [snailsploit.com](https://snailsploit.com), Hakin9 Magazine, and Medium.

| Paper | Summary |
|---|---|
| [Self-Replicating Memory Worm](https://snailsploit.com/ai-security/self-replicating-memory-worm/) | Autonomous persistence chain — skill injection + memory poisoning = self-healing implant. Four-stage kill chain from a single memory slot to autonomous propagation. No jailbreak required. |
| [Memory Injection Through Nested Skills](https://snailsploit.com/ai-security/nested-skill-injection/) | Novel persistence via skill files that regenerate poisoned memory slots on boot. Dual-persistence architecture: memory slots and skill files, each restoring the other. |
| [Weaponized AI Supply Chain](https://snailsploit.com/ai-security/weaponized-ai-supply-chain/) | End-to-end supply chain attack through AI agent skill injection, validated against DVWA and Juice Shop in agent harness. |
| [AI Gateway Threat Model (TC-21)](https://snailsploit.com/ai-security/ai-gateway-threat-model/) | First generalized threat model for AI gateways — 8 attack vectors, proposed as AATMF v3 TC-21. No prior academic or framework coverage existed. |
| [MCP vs A2A Attack Surface](https://snailsploit.com/ai-security/mcp-vs-a2a/) | Comparative threat model — where Model Context Protocol and Agent-to-Agent diverge in trust boundaries. |
| [The 30% Blind Spot](https://snailsploit.com/ai-security/llm-safety-judges/) | Empirical study showing LLM-as-judge safety classifiers miss ~30% of adversarial output classes. |
| [AI Breach Detection Gap](https://snailsploit.com/ai-security/ai-breach-detection-gap/) | Analysis of detection blind spots in AI-integrated production systems. |
| [AI Coding Agent Attack Surface](https://snailsploit.com/ai-security/ai-coding-agent-attack-surface/) | Attack surface analysis of AI-powered coding assistants and their tool-use capabilities. |
| [Agentic AI Threat Landscape](https://snailsploit.com/ai-security/agentic-ai-threat-landscape/) | Threat landscape survey of autonomous AI agent architectures. |
| [Adversarial Prompting: Complete Guide](https://snailsploit.com/ai-security/adversarial-prompting/) | End-to-end methodology covering direct, indirect, multi-turn, and agentic prompt injection. |
| [Computational Countertransference](https://snailsploit.com/ai-security/computational-countertransference/) | The psychology of human–AI manipulation dynamics. |
| [AATMF v3.1 vs MITRE ATLAS](https://snailsploit.com/ai-security/aatmf-vs-mitre-atlas/) | Framework comparison showing coverage gaps in existing AI threat taxonomies. |
| [The Memory Manipulation Problem](https://snailsploit.com/ai-security/jailbreaking/memory-manipulation-attacks/) | How attackers exploit persistent context to compromise future interactions and undermine AI system integrity. |
| [ChatGPT Canvas DNS Exfiltration](https://github.com/SnailSploit/ChatGPT-DNS-Exfill) | DNS exfiltration via ChatGPT Canvas — rendered content triggers DNS lookups without outbound HTTP. |
| [ChatGPT Sandbox RCE + DNS Exfil](https://github.com/SnailSploit/chatgpt-rce-dns) | Pickle deserialization RCE chained with DNS exfiltration to escape the Code Interpreter sandbox. |
| [Double AI, Triple Mechanism](https://snailsploit.com/ai-security/cloud-obfuscator/) | Cloud-based obfuscator attack research. |
| [Linux Kernel io_uring/zcrx Race Condition](https://snailsploit.com/security-research/general/io-uring-zcrx-race-condition/) | Race condition → double-free → OOB write in io_uring zero-copy receive. Mainline-merged. |

---

## 🐧 Linux Kernel

Five mainline-merged patches across networking, IPC, Bluetooth, RDMA, and io_uring — reviewed and accepted through the standard kernel maintainer process into Linus's tree.

| Subsystem | Vulnerability | Status |
|---|---|---|
| `io_uring/zcrx` | `user_ref` race → double-free → OOB write | ✅ Mainline 7.0-rc1 · stable backports [6.18.16](https://cdn.kernel.org/pub/linux/kernel/v6.x/ChangeLog-6.18.16) + [6.19.6](https://cdn.kernel.org/pub/linux/kernel/v6.x/ChangeLog-6.19.6) |
| `net/tipc` | `tipc_mon_peer_up` UAF vs bearer teardown | ✅ Mainline |
| `Bluetooth` | `hci_conn` UAF in `create_big_sync` / `create_big_complete` | ✅ Mainline |
| `RDMA/ionic` | Unbounded `node_desc` sysfs read via `%.64s` | ✅ Mainline |
| `net/rtnetlink` | `ifla_vf_broadcast` stack infoleak (zero init missing) | ✅ Mainline |

All patches on [lore.kernel.org →](https://lore.kernel.org/all/?q=Kai+Aizen)

---

## 🛡️ CVEs

Sorted by blast radius — shared infrastructure first, single-vendor plugins last.

| CVE | Target | Type | Severity |
|---|---|---|---|
| [CVE-2026-3288](https://github.com/SnailSploit/CVE-2026-3288) | Kubernetes ingress-nginx | Config injection → RCE | **High (8.8)** |
| [CVE-2026-30911](https://github.com/SnailSploit/CVE-2026-30911) | Apache Airflow Core | Missing authentication | **High (8.1)** |
| [CVE-2026-32794](https://github.com/SnailSploit/CVE-2026-32794) | Apache Airflow (Databricks provider) | TLS verification bypass | **High (7.4)** |
| [CVE-2026-31899](https://github.com/SnailSploit/CVE-2026-31899) | [CairoSVG](https://github.com/Kozea/CairoSVG/security/advisories/GHSA-f38f-5xpm-9r7c) | Exponential DoS — recursive amplification | **High (7.5)** |
| [CVE-2026-32809](https://snailsploit.com/security-research/cves/cve-2026-32809/) | ouch (Rust) | Symlink bypass | — |
| [CVE-2025-9776](https://github.com/SnailSploit/CVE-2025-9776) | CatFolders (WordPress) | SQL Injection via CSV Import | Medium (6.5) |
| [CVE-2025-12163](https://github.com/SnailSploit/CVE-2025-12163) | OmniPress (WordPress) | Stored XSS | Medium (6.4) |
| [CVE-2025-11171](https://github.com/SnailSploit/CVE-2025-11171) | Chartify (WordPress) | Missing Authentication | Medium (5.3) |
| [CVE-2025-11174](https://github.com/SnailSploit/CVE-2025-11174) | Document Library Lite (WordPress) | Unauth Info Disclosure | Medium (5.3) |
| [CVE-2025-12030](https://github.com/SnailSploit/CVE-2025-12030) | ACF to REST API (WordPress) | IDOR | Medium (4.3) |
| [CVE-2026-1208](https://github.com/SnailSploit/CVE-2026-1208) | Welcart (WordPress) | CSRF to Settings Update | Medium (4.3) |

Plus: **TelSender** — stored XSS that resulted in vendor-side plugin removal.

## 🔓 Security Advisories

| Advisory | Target | Type | Severity |
|---|---|---|---|
| [GHSA-j425-whc4-4jgc](https://github.com/SnailSploit/OpenClaw-Env-Injection) | [OpenClaw](https://github.com/openclaw/openclaw/security/advisories/GHSA-j425-whc4-4jgc) (309k⭐) | `system.run` env override RCE — allowlist bypass via `GIT_SSH_COMMAND`, editor hooks, `GIT_CONFIG_*` | Medium (6.3) |

---

## 🛠️ More Tools

| Tool | Description |
|---|---|
| [**SnailHunter**](https://github.com/SnailSploit/SnailHunter) | AI-powered bug bounty automation — LLM analysis combined with traditional security scanning. |
| [**KubeRoast**](https://github.com/SnailSploit/KubeRoast_v1) | Red-team Kubernetes misconfiguration & attack-path scanner. |
| [**Xposure**](https://github.com/SnailSploit/Xposure) | Autonomous credential intelligence platform for attack-surface recon. |
| [**SnailSploit Recon**](https://github.com/SnailSploit/SnailSploit_Recon_extension) | Chrome MV3 extension — passive recon, security headers, IP intel, CPE→CVE enrichment. |
| [**SnailPath**](https://github.com/SnailSploit/SnailPath) | Async directory & route discovery — HTTP/2, soft-404 suppression, JS/sourcemap mining. |
| [**ZenFlood**](https://github.com/SnailSploit/ZenFlood) | Low-bandwidth stress testing — modernized Slowloris. HTTP/1.1 + HTTP/2 with jittered, obfuscated payloads. |
| [**Awesome-Snail-OSINT**](https://github.com/SnailSploit/AwesomeSnailsOsint) | Curated OSINT resource collection for offensive recon. |

---

<p align="center">
  <a href="https://snailsploit.com"><img src="https://img.shields.io/badge/Read_the_research-snailsploit.com-black?style=for-the-badge" alt="SnailSploit"></a>
</p>

<p align="center">
  <code>same attack. different substrate.</code>
</p>
