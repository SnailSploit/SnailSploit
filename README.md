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
24 CVEs · 38 public findings · Linux kernel contributor · Hakin9 contributing author
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
| [Self-Replicating Memory Worm](https://snailsploit.com/ai-security/self-replicating-memory-worm/) | Autonomous persistence chain — skill injection + memory poisoning = self-healing implant. Four-stage kill chain, no jailbreak required. |
| [Memory Injection Through Nested Skills](https://snailsploit.com/ai-security/nested-skill-injection/) | Dual-persistence architecture: memory slots and skill files, each restoring the other on boot. |
| [Weaponized AI Supply Chain](https://snailsploit.com/ai-security/weaponized-ai-supply-chain/) | End-to-end supply chain attack through AI agent skill injection, validated against DVWA and Juice Shop. |
| [AI Gateway Threat Model (TC-21)](https://snailsploit.com/ai-security/ai-gateway-threat-model/) | First generalized threat model for AI gateways — 8 attack vectors, proposed as AATMF v3 TC-21. |
| [MCP vs A2A Attack Surface](https://snailsploit.com/ai-security/mcp-vs-a2a/) | Comparative threat model — where MCP and Agent-to-Agent diverge in trust boundaries. |
| [The 30% Blind Spot](https://snailsploit.com/ai-security/llm-safety-judges/) | Empirical study showing LLM-as-judge safety classifiers miss ~30% of adversarial output classes. |
| [AI Breach Detection Gap](https://snailsploit.com/ai-security/ai-breach-detection-gap/) | Detection blind spots in AI-integrated production systems. |
| [AI Coding Agent Attack Surface](https://snailsploit.com/ai-security/ai-coding-agent-attack-surface/) | Attack surface analysis of AI-powered coding assistants and their tool-use capabilities. |
| [Agentic AI Threat Landscape](https://snailsploit.com/ai-security/agentic-ai-threat-landscape/) | Threat landscape survey of autonomous AI agent architectures. |
| [Adversarial Prompting: Complete Guide](https://snailsploit.com/ai-security/adversarial-prompting/) | End-to-end methodology — direct, indirect, multi-turn, and agentic prompt injection. |
| [Computational Countertransference](https://snailsploit.com/ai-security/computational-countertransference/) | The psychology of human–AI manipulation dynamics. |
| [AATMF v3.1 vs MITRE ATLAS](https://snailsploit.com/ai-security/aatmf-vs-mitre-atlas/) | Framework comparison showing coverage gaps in existing AI threat taxonomies. |
| [The Memory Manipulation Problem](https://snailsploit.com/ai-security/jailbreaking/memory-manipulation-attacks/) | How attackers exploit persistent context to compromise future interactions. |
| [ChatGPT Canvas DNS Exfiltration](https://github.com/SnailSploit/ChatGPT-DNS-Exfill) | DNS exfil via ChatGPT Canvas — rendered content triggers DNS lookups without outbound HTTP. |
| [ChatGPT Sandbox RCE + DNS Exfil](https://github.com/SnailSploit/chatgpt-rce-dns) | Pickle deserialization RCE chained with DNS exfiltration to escape Code Interpreter sandbox. |
| [Double AI, Triple Mechanism](https://snailsploit.com/ai-security/cloud-obfuscator/) | Cloud-based obfuscator attack research. |
| [Linux Kernel io_uring/zcrx Race Condition](https://snailsploit.com/security-research/general/io-uring-zcrx-race-condition/) | Race condition → double-free → OOB write in io_uring zero-copy receive. Mainline-merged. |

---

## 🐧 Linux Kernel

Five patches across networking, IPC, Bluetooth, RDMA, and io_uring — accepted through the standard kernel maintainer process.

| # | Subsystem | Vulnerability | Status |
|---|---|---|---|
| 25 | `io_uring/zcrx` | `user_ref` race between scrub and refill → double-free → OOB write | ✅ Mainlined 7.0-rc1 · stable backports 6.18.16 + 6.19.6 |
| 26 | `net/tipc` | `tipc_mon_peer_up`/`down`/`remove_peer` UAF vs bearer teardown | 🔄 Under review |
| 27 | `Bluetooth/hci_conn` | UAF in `create_big_sync` / `create_big_complete` | ✅ Successor merged |
| 28 | `RDMA/ionic` | Unbounded `node_desc` sysfs read — bound with `%.64s` | ✅ Mainlined 2026-04-20 |
| 29 | `net/rtnetlink` | `ifla_vf_broadcast` stack infoleak — zero init missing | 🔄 Under review |

All patches on [lore.kernel.org →](https://lore.kernel.org/all/?q=Kai+Aizen)

---

## 🛡️ CVEs (24)

Sorted by severity — shared infrastructure first.

| # | CVE | Target | Type | Severity |
|---|---|---|---|---|
| 1 | [CVE-2026-3596](https://nvd.nist.gov/vuln/detail/CVE-2026-3596) | Riaxe Product Customizer (WP) | Missing Auth → Priv Esc | **Critical (9.8)** |
| 2 | [CVE-2026-3288](https://nvd.nist.gov/vuln/detail/CVE-2026-3288) | Kubernetes ingress-nginx | Config Injection → RCE | **High (8.8)** |
| 3 | [CVE-2026-1313](https://nvd.nist.gov/vuln/detail/CVE-2026-1313) | MimeTypes Link Icons (WP) | SSRF | **High (8.3)** |
| 4 | [CVE-2026-30911](https://nvd.nist.gov/vuln/detail/CVE-2026-30911) | Apache Airflow Core | Missing Auth (HITL) | **High (8.1)** |
| 5 | [CVE-2026-43884](https://nvd.nist.gov/vuln/detail/CVE-2026-43884) | AVideo | SSRF Protection Bypass via DNS Rebinding | **High** |
| 6 | [CVE-2026-31899](https://nvd.nist.gov/vuln/detail/CVE-2026-31899) | CairoSVG | Exponential DoS — Recursive Amplification | **High (7.5)** |
| 7 | [CVE-2026-3599](https://nvd.nist.gov/vuln/detail/CVE-2026-3599) | Riaxe Product Customizer (WP) | Unauthenticated SQLi | **High (7.5)** |
| 8 | [CVE-2026-32809](https://nvd.nist.gov/vuln/detail/CVE-2026-32809) | ouch (Rust) | Symlink Escape | **High (7.4)** |
| 9 | [CVE-2025-9776](https://nvd.nist.gov/vuln/detail/CVE-2025-9776) | CatFolders (WP) | SQLi via CSV Import | Medium (6.5) |
| 10 | [CVE-2026-33693](https://nvd.nist.gov/vuln/detail/CVE-2026-33693) | activitypub-federation-rust | SSRF — `0.0.0.0` Bypass | Medium (6.5) |
| 11 | [CVE-2026-32885](https://nvd.nist.gov/vuln/detail/CVE-2026-32885) | ddev/ddev | ZipSlip | Medium (6.5) |
| 12 | [CVE-2025-12163](https://nvd.nist.gov/vuln/detail/CVE-2025-12163) | OmniPress (WP) | Stored XSS | Medium (6.4) |
| 13 | [CVE-2026-44217](https://nvd.nist.gov/vuln/detail/CVE-2026-44217) | sse-channel (npm) | SSE Injection — Unsanitized Fields | Moderate |
| 14 | [CVE-2026-2717](https://nvd.nist.gov/vuln/detail/CVE-2026-2717) | HTTP Headers (WP) | CRLF Injection | Medium (5.5) |
| 15 | [CVE-2026-0811](https://nvd.nist.gov/vuln/detail/CVE-2026-0811) | Advanced CF7 DB (WP) | CSRF → Form Deletion | Medium (5.4) |
| 16 | [CVE-2026-1314](https://nvd.nist.gov/vuln/detail/CVE-2026-1314) | 3D FlipBook (WP) | Missing Auth | Medium (5.3) |
| 17 | [CVE-2026-3594](https://nvd.nist.gov/vuln/detail/CVE-2026-3594) | Riaxe Product Customizer (WP) | Info Disclosure — `/orders` | Medium (5.3) |
| 18 | [CVE-2026-3595](https://nvd.nist.gov/vuln/detail/CVE-2026-3595) | Riaxe Product Customizer (WP) | Unauthenticated User Deletion | Medium (5.3) |
| 19 | [CVE-2025-11171](https://nvd.nist.gov/vuln/detail/CVE-2025-11171) | Chartify (WP) | Missing Auth — Admin Function | Medium (5.3) |
| 20 | [CVE-2025-11174](https://nvd.nist.gov/vuln/detail/CVE-2025-11174) | Document Library Lite (WP) | Missing Auth → Info Disclosure | Medium (5.3) |
| 21 | [CVE-2026-32794](https://nvd.nist.gov/vuln/detail/CVE-2026-32794) | Apache Airflow (Databricks) | TLS Verification Bypass → MitM | Medium (4.8) |
| 22 | [CVE-2026-0814](https://nvd.nist.gov/vuln/detail/CVE-2026-0814) | Advanced CF7 DB (WP) | Missing Auth — Subscriber+ Export | Medium (4.3) |
| 23 | [CVE-2025-12030](https://nvd.nist.gov/vuln/detail/CVE-2025-12030) | ACF to REST API (WP) | IDOR | Medium (4.3) |
| 24 | [CVE-2026-1208](https://nvd.nist.gov/vuln/detail/CVE-2026-1208) | Welcart (WP) | CSRF → Settings Update | Medium (4.3) |

---

## 🔓 GHSAs & Vendor Findings

| # | ID | Target | Type | Status |
|---|---|---|---|---|
| 30 | — | TelSender (WP) | Unauthenticated Stored XSS (7.2) | Plugin shut down by vendor |
| 31 | [GHSA-j425-whc4-4jgc](https://github.com/advisories/GHSA-j425-whc4-4jgc) | OpenClaw (309k⭐) | `system.run` env override RCE — allowlist bypass (6.3) | Published |
| 32 | [PR #9486](https://github.com/concourse/concourse/pull/9486) | Concourse CI | Symlink breakout in tar extraction | Merged v8.1.1 |

---

## 🐛 Public Issues & Disclosures

| # | Target | Description | Link |
|---|---|---|---|
| 33 | Exiv2/exiv2 | OOB access in `SigmaMakerNote::printStripLabel` | [#3461](https://github.com/Exiv2/exiv2/issues/3461) |
| 34 | fastify-sse-v2 | SSE Event Injection (CWE-93) | [#110](https://github.com/mpetrunic/fastify-sse-v2/issues/110) |
| 35 | express-sse | SSE Event Injection (CWE-93) | [#60](https://github.com/dpskvn/express-sse/issues/60) |
| 36 | django-eventstream | SSE Event Injection (CWE-93) | [#185](https://github.com/fanout/django-eventstream/issues/185) |
| 37 | flask-sse | SSE Injection in `Message.str()` (CWE-93) | [#40](https://github.com/singingwolfboy/flask-sse/issues/40) |
| 38 | koa-sse | SSE Injection in `_transform` (CWE-93) | [#13](https://github.com/yklykl530/koa-sse/issues/13) |

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

## 📊 Summary

| Metric | Count |
|---|---|
| Published CVEs | 24 |
| Linux Kernel Patches | 5 |
| GHSAs / Vendor Disclosures | 2 |
| Merged Source-tree PRs | 1 |
| Public Issues Filed | 6 |
| **Total Distinct Public Findings** | **38** |

**Sources of record:** [Wordfence](https://www.wordfence.com/threat-intel/vulnerabilities/researchers/kai-aizen) · [GHSA Credit](https://github.com/advisories?query=credit%3ASnailSploit) · [GitHub](https://github.com/SnailSploit) · [lore.kernel.org](https://lore.kernel.org/all/?q=Kai+Aizen)

---

<p align="center">
  <a href="https://snailsploit.com"><img src="https://img.shields.io/badge/Read_the_research-snailsploit.com-black?style=for-the-badge" alt="SnailSploit"></a>
</p>

<p align="center">
  <code>same attack. different substrate.</code>
</p>
