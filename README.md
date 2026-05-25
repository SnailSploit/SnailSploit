<p align="center">
  <a href="https://snailsploit.com">
    <img src="https://github.com/SnailSploit/SnailSploit/raw/main/banner.png" alt="snailsploit — same attack. different substrate." width="100%">
  </a>
</p>

<p align="center">
  <strong>adversarial ai research · llm red teaming · kernel</strong>
</p>

<p align="center">
  <a href="https://snailsploit.com"><img src="https://img.shields.io/badge/snailsploit.com-0E0E0F?style=flat-square&logo=astro&logoColor=E9E7E1&labelColor=0E0E0F" alt="Website"></a>
  <a href="https://thejailbreakchef.com"><img src="https://img.shields.io/badge/the_jailbreak_chef-0E0E0F?style=flat-square&logo=fireship&logoColor=E9E7E1&labelColor=0E0E0F" alt="The Jailbreak Chef"></a>
  <a href="https://linkedin.com/in/kaiaizen"><img src="https://img.shields.io/badge/linkedin-0E0E0F?style=flat-square&logo=linkedin&logoColor=E9E7E1&labelColor=0E0E0F" alt="LinkedIn"></a>
  <a href="https://medium.com/@snailsploit"><img src="https://img.shields.io/badge/medium-0E0E0F?style=flat-square&logo=medium&logoColor=E9E7E1&labelColor=0E0E0F" alt="Medium"></a>
</p>

---

same attack. different substrate.

snailsploit is an independent adversarial research group.

**frameworks.** AATMF, SEF, P.R.O.M.P.T — adversarial ai threat modeling and social engineering taxonomies.
**CVEs.** 60+ published across linux kernel, kubernetes, oss libraries, and wordpress plugins.
**tools.** open-source offensive tooling — recon, scanning, exploitation, obfuscation.

[snailsploit.com →](https://snailsploit.com)

---

## frameworks & tooling

| Project | Description |
|---|---|
| [**AATMF v3.1**](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) | Adversarial AI Threat Modeling Framework — 20 tactics, 240+ techniques, 2,152+ procedures, 4,980+ prompts. Crosswalks to OWASP LLM Top-10, NIST AI RMF, MITRE ATLAS, EU AI Act. On OWASP GenAI Security 2026 roadmap. YARA + Sigma detection signatures included. |
| [**AATMF Toolkit**](https://github.com/SnailSploit/aatmf-toolkit) | Python CLI for systematic LLM safety testing — three-layer evaluation pipeline, defense fingerprinting, regression tracking, attack chain planning. Mapped to the full AATMF taxonomy. |
| [**Claude-Red**](https://github.com/SnailSploit/Claude-Red) | Curated library of 58 offensive security skills across 13 categories (web, wireless, exploit-dev, infrastructure, cloud, AD, auth, fuzzing, recon, AI, IoT, mobile, utility) for the Claude skills system. Drop a `SKILL.md` into your environment and Claude operates as a specialist — SQLi to shellcode, EDR evasion to ADCS abuse. Trigger-loaded on demand; zero context cost for unused skills. |
| [**LLM Red Teamer's Playbook**](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) | Diagnostic methodology for bypassing LLM defense layers — input filters → alignment → identity → output → agentic trust. Mapped to AATMF taxonomy. |
| [**Burp MCP Toolkit**](https://github.com/SnailSploit/Burp-MCP-Security-Analysis-Toolkit) | Skills-based security analysis framework combining Burp Suite traffic capture with Claude Code reasoning via MCP. Expert pentest methodology encoded into reusable skill files. |
| [**JystDastIt**](https://github.com/SnailSploit/JystDastIt) | The Burp You Can Afford — open-source CLI DAST toolkit for web application vulnerability scanning and XSS detection. |
| [**SnailObfuscator**](https://github.com/SnailSploit/SnailObfuscator) | Structurally-aware code obfuscation engine — polymorphic payload generation that bypasses static and behavioral detection. |
| [**P.R.O.M.P.T**](https://snailsploit.com/frameworks/prompt/) | Adversarial prompt engineering methodology — structured attack phases with Cialdini influence principles and PHLRA context injection. |
| [**SEF**](https://snailsploit.com/frameworks/sef/) | Social Engineering Framework — organizational gap analysis (Authority / Process / Trust / Pressure / Knowledge), pretext selection, MITRE ATT&CK mapping. |

---

## research

published at [snailsploit.com](https://snailsploit.com), Hakin9 Magazine, and Medium.

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
| [Linux Kernel io_uring/zcrx Race Condition](https://snailsploit.com/security-research/general/io-uring-zcrx-race-condition/) | Race condition → double-free → OOB write in io_uring zero-copy receive. Mainlined; assigned CVE-2026-43121. |

---

## CVEs (34)

sorted by target reach — core infrastructure first, WordPress plugins last. severity is the secondary sort within each tier.

| # | CVE | Target | Type | Severity | Status |
|---|---|---|---|---|---|
| 1 | [CVE-2026-47393](https://snailsploit.com/security-research/cves/cve-2026-47393/) | PraisonAI | Authentication Disabled by Default | **Critical (9.8)** | Published |
| 2 | [CVE-2026-47398](https://snailsploit.com/security-research/cves/cve-2026-47398/) | PraisonAI | Code Injection via `exec_module` (YAML-controlled module paths) | **High (8.1)** | Published |
| 3 | [CVE-2026-43121](https://nvd.nist.gov/vuln/detail/CVE-2026-43121) | Linux Kernel io_uring | `user_ref` race → double-free → OOB write | Medium (4.7) | Published |
| 4 | [CVE-2026-3288](https://nvd.nist.gov/vuln/detail/CVE-2026-3288) | Kubernetes ingress-nginx | Config Injection → RCE | **High (8.8)** | Published |
| 5 | [CVE-2026-30911](https://nvd.nist.gov/vuln/detail/CVE-2026-30911) | Apache Airflow Core | Missing Auth (HITL) | **High (8.1)** | Published |
| 6 | [CVE-2026-32794](https://nvd.nist.gov/vuln/detail/CVE-2026-32794) | Apache Airflow (Databricks Provider) | TLS Verification Bypass → MitM | Medium (4.8) | Published |
| 7 | [CVE-2026-8368](https://github.com/libwww-perl/libwww-perl/pull/512) | Perl `LWP::UserAgent` / `HTTP::Tiny` | Zero Header Strip on Cross-Host Redirect | — | NVD: RESERVED |
| 8 | [CVE-2026-45363](https://github.com/jwt/ruby-jwt/security/advisories/GHSA-c32j-vqhx-rx3x) | jwt/ruby-jwt | Empty-key HMAC Bypass | 7.4 | NVD: RESERVED |
| 9 | [CVE-2026-31899](https://nvd.nist.gov/vuln/detail/CVE-2026-31899) | CairoSVG | Exponential DoS — Recursive Amplification | **High (7.5)** | Published |
| 10 | [CVE-2026-44840](https://github.com/dgraph-io/dgraph/security/advisories/GHSA-q2m9-6jp9-c6mc) | Dgraph | DQL Injection via `checkUserPassword` GraphQL Query | **High** | Published |
| 11 | [CVE-2026-33693](https://nvd.nist.gov/vuln/detail/CVE-2026-33693) | activitypub-federation-rust | SSRF — `0.0.0.0` Bypass | Medium (6.5) | Published |
| 12 | [CVE-2026-32885](https://nvd.nist.gov/vuln/detail/CVE-2026-32885) | ddev/ddev | ZipSlip | Medium (6.5) | Published |
| 13 | [CVE-2026-32809](https://www.cve.org/CVERecord?id=CVE-2026-32809) | ouch (Rust) | Symlink Escape | **High (7.4)** | NVD: RESERVED |
| 14 | [CVE-2026-44217](https://nvd.nist.gov/vuln/detail/CVE-2026-44217) | sse-channel (npm) | SSE Injection — Unsanitized Fields | Moderate | Published |
| 15 | [CVE-2026-48022](https://github.com/advisories/GHSA-x426-x7cc-3fpc) | @hapi/wreck (npm) | Credential Header Leak on Cross-Port / Cross-Scheme Redirect | Moderate | Published |
| 16 | [CVE-2026-46627](https://snailsploit.com/security-research/cves/cve-2026-46627/) | Twig (PHP) | Sandbox Resource Exhaustion — CPU/Memory DoS | Moderate | Published |
| 17 | [CVE-2026-43884](https://nvd.nist.gov/vuln/detail/CVE-2026-43884) | AVideo | SSRF Protection Bypass via DNS Rebinding | **High** | Published |
| 18 | [CVE-2026-45620](https://github.com/advisories/GHSA-vpfx-pxqw-2w79) | AVideo | CVE-2026-43881 Incomplete Fix | — | Published |
| 19 | CVE-2026-45619 | AVideo | CVE-2026-43884 Incomplete Fix — 6+ `isSSRFSafeURL()` sites discard `$resolvedIP` out-param at master HEAD post-`603e7bf` | — | Published |
| 20 | [CVE-2026-3596](https://nvd.nist.gov/vuln/detail/CVE-2026-3596) | Riaxe Product Customizer (WP) | Missing Auth → Priv Esc | **Critical (9.8)** | Published |
| 21 | [CVE-2026-3599](https://nvd.nist.gov/vuln/detail/CVE-2026-3599) | Riaxe Product Customizer (WP) | Unauthenticated SQLi | **High (7.5)** | Published |
| 22 | [CVE-2026-3594](https://nvd.nist.gov/vuln/detail/CVE-2026-3594) | Riaxe Product Customizer (WP) | Info Disclosure — `/orders` | Medium (5.3) | Published |
| 23 | [CVE-2026-3595](https://nvd.nist.gov/vuln/detail/CVE-2026-3595) | Riaxe Product Customizer (WP) | Unauthenticated User Deletion | Medium (5.3) | Published |
| 24 | [CVE-2026-1313](https://nvd.nist.gov/vuln/detail/CVE-2026-1313) | MimeTypes Link Icons (WP) | SSRF | **High (8.3)** | Published |
| 25 | [CVE-2025-9776](https://nvd.nist.gov/vuln/detail/CVE-2025-9776) | CatFolders (WP) | SQLi via CSV Import | Medium (6.5) | Published |
| 26 | [CVE-2025-12163](https://nvd.nist.gov/vuln/detail/CVE-2025-12163) | Omnipress (WP) | Stored XSS | Medium (6.4) | Published |
| 27 | [CVE-2026-2717](https://nvd.nist.gov/vuln/detail/CVE-2026-2717) | HTTP Headers (WP) | CRLF Injection | Medium (5.5) | Published |
| 28 | [CVE-2026-0811](https://nvd.nist.gov/vuln/detail/CVE-2026-0811) | Advanced CF7 DB (WP) | CSRF → Form Deletion | Medium (5.4) | Published |
| 29 | [CVE-2026-0814](https://nvd.nist.gov/vuln/detail/CVE-2026-0814) | Advanced CF7 DB (WP) | Missing Auth — Subscriber+ Export | Medium (4.3) | Published |
| 30 | [CVE-2026-1314](https://nvd.nist.gov/vuln/detail/CVE-2026-1314) | 3D FlipBook (WP) | Missing Auth | Medium (5.3) | Published |
| 31 | [CVE-2025-11171](https://nvd.nist.gov/vuln/detail/CVE-2025-11171) | Chartify (WP) | Missing Auth — Admin Function | Medium (5.3) | Published |
| 32 | [CVE-2025-11174](https://nvd.nist.gov/vuln/detail/CVE-2025-11174) | Document Library Lite (WP) | Missing Auth → Info Disclosure | Medium (5.3) | Published |
| 33 | [CVE-2025-12030](https://nvd.nist.gov/vuln/detail/CVE-2025-12030) | ACF to REST API (WP) | IDOR | Medium (4.3) | Published |
| 34 | [CVE-2026-1208](https://nvd.nist.gov/vuln/detail/CVE-2026-1208) | Welcart (WP) | CSRF → Settings Update | Medium (4.3) | Published |

---

## linux kernel

five patches across io_uring, IPC, Bluetooth, RDMA, and networking — all mainlined through the standard kernel maintainer process.

| # | Subsystem | Vulnerability | Status |
|---|---|---|---|
| 35 | `io_uring/zcrx` | Fix `user_ref` race between scrub and refill paths → double-free → OOB write (CVE-2026-43121) | Mainlined 7.0-rc1 |
| 36 | `net/tipc` | `tipc_mon_peer_up`/`down`/`remove_peer` UAF | Mainlined |
| 37 | `Bluetooth/hci_conn` | UAF in `create_big_sync` and `create_big_complete` | Mainlined |
| 38 | `RDMA/ionic` | Bound `node_desc` sysfs read with `%.64s` | Mainlined 2026-04-20 |
| 39 | `net/rtnetlink` | Zero `ifla_vf_broadcast` to avoid stack infoleak | Mainlined |

all patches on [lore.kernel.org →](https://lore.kernel.org/all/?q=Kai+Aizen)

---

## GHSAs, vendor findings & bounties

| # | ID | Target | Type | Status |
|---|---|---|---|---|
| 40 | — | [TelSender (WP)](https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/telsender) | Unauthenticated Stored XSS via Telegram Chat Title (7.2) | Plugin taken down by maintainer |
| 41 | [GHSA-j425-whc4-4jgc](https://github.com/advisories/GHSA-j425-whc4-4jgc) | OpenClaw | `system.run` env override RCE — allowlist bypass (6.3) | Published |
| 42 | [GHSA-gxhx-2686-5h9g](https://github.com/slack-go/slack/security/advisories/GHSA-gxhx-2686-5h9g) | slack-go/slack | Security advisory | Published |
| 43 | [GHSA-x426-x7cc-3fpc](https://github.com/advisories/GHSA-x426-x7cc-3fpc) | @hapi/wreck (npm) | Credential header leak on cross-port/cross-scheme redirect (CVE-2026-48022) | Published |
| 44 | — | `@linear/sdk` | `LinearWebhooks.verify` accepts empty secret without precondition | Merged ($400 bounty) |

---

## summary

| Metric | Count |
|---|---|
| Published / assigned CVEs | 34 |
| — of which NVD-reserved (CVE-assigned, not yet on NVD) | 3 |
| Mainlined Linux kernel patches | 5 |
| GHSAs / vendor disclosures / bounties | 5 |

> CVE-2026-43121 is the assigned CVE for the mainlined `io_uring/zcrx` patch — counted once under CVEs (#3); it is the same finding as kernel patch #35. CVE-2026-48022 (@hapi/wreck) is counted once under CVEs (#15); its GHSA (#43) is the same finding.

**sources of record:** [Wordfence](https://www.wordfence.com/threat-intel/vulnerabilities/researchers/kai-aizen) · [GHSA Credit](https://github.com/advisories?query=credit%3ASnailSploit) · [GitHub](https://github.com/SnailSploit) · [lore.kernel.org](https://lore.kernel.org/all/?q=Kai+Aizen)

---

## more tools

| Tool | Description |
|---|---|
| [**SnailHunter**](https://github.com/SnailSploit/SnailHunter) | AI-powered bug bounty automation — LLM analysis combined with traditional security scanning. |
| [**KubeRoast**](https://github.com/SnailSploit/KubeRoast_v1) | Red-team Kubernetes misconfiguration & attack-path scanner. |
| [**Xposure**](https://github.com/SnailSploit/Xposure) | Autonomous credential intelligence platform for attack-surface recon. |
| [**SnailSploit Recon**](https://github.com/SnailSploit/SnailSploit_Recon_extension) | Chrome MV3 extension — passive recon, security headers, IP intel, CPE→CVE enrichment. |
| [**Awesome-Snail-OSINT**](https://github.com/SnailSploit/AwesomeSnailsOsint) | Curated OSINT resource collection for offensive recon. |

---

<p align="center">
  <a href="https://snailsploit.com"><img src="https://img.shields.io/badge/read_the_research-snailsploit.com-E07A4A?style=flat-square&labelColor=0E0E0F" alt="snailsploit"></a>
</p>

<p align="center">
  <code>same attack. different substrate.</code>
</p>
