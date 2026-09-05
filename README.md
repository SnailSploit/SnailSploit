[![snailsploit — same attack. different substrate.](https://github.com/SnailSploit/SnailSploit/raw/main/banner.png)](https://snailsploit.com)

**adversarial ai research · llm red teaming · kernel · vulnerability research**

[![Website](https://img.shields.io/badge/snailsploit.com-0E0E0F?style=flat-square&logo=astro&logoColor=E9E7E1&labelColor=0E0E0F)](https://snailsploit.com) [![The Jailbreak Chef](https://img.shields.io/badge/the_jailbreak_chef-0E0E0F?style=flat-square&logo=fireship&logoColor=E9E7E1&labelColor=0E0E0F)](https://thejailbreakchef.com) [![LinkedIn](https://img.shields.io/badge/linkedin-0E0E0F?style=flat-square&logo=linkedin&logoColor=E9E7E1&labelColor=0E0E0F)](https://linkedin.com/in/kaiaizen) [![Medium](https://img.shields.io/badge/medium-0E0E0F?style=flat-square&logo=medium&logoColor=E9E7E1&labelColor=0E0E0F)](https://medium.com/@snailsploit)

---

same attack. different substrate.

snailsploit is an independent adversarial research group — vulnerability research, framework development, and offensive tooling across kernels, language models, and everything between them.

92 publicly attributable CVEs · 4 linux kernel CVEs · 5 mainlined kernel patches · 27+ distinct targets

[snailsploit.com →](https://snailsploit.com)

---

## CVEs (92)

sorted by target class — infrastructure and AI first, then libraries, then CMS plugins. severity is the secondary sort within each tier.

### AI / ML platforms

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 1 | [CVE-2026-47393](https://snailsploit.com/security-research/cves/cve-2026-47393/) | PraisonAI | Authentication disabled by default | **Critical (9.8)** | Published |
| 2 | [CVE-2026-57127](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | `recipe serve` auth middleware disables itself with no secret | **Critical (9.8)** | Published |
| 3 | [CVE-2026-57131](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | Jobs API exposes agent-execution endpoints with no auth | **Critical (9.8)** | Published |
| 4 | [CVE-2026-57147](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | Hardcoded default JWT signing secret enables token forgery | **Critical (9.8)** | Published |
| 5 | [CVE-2026-47398](https://snailsploit.com/security-research/cves/cve-2026-47398/) | PraisonAI | Code injection via `exec_module` (YAML-controlled module paths) | **High (8.1)** | Published |
| 6 | [CVE-2026-57126](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | SSRF guard validates literal IPs only — never resolves DNS | **High (8.5)** | Published |
| 7 | [CVE-2026-55528](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-7g3p-92qq-8wvh) | PraisonAI | `AgentServer` declares `auth_token` but never enforces it on any route (CWE-862) | **High (8.2)** | Published |
| 8 | [CVE-2026-57120](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | `execute_code` sandbox bypass via `str.format` dunder access | Medium (6.5) | Published |
| 9 | [CVE-2026-55530](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-cfxv-8fw8-rwpv) | PraisonAI | `ast_grep_rewrite` rewrites arbitrary files without `@require_approval` gate (CWE-862) | Moderate (6.1) | Published |
| 10 | [CVE-2026-62164](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-29r9-67vg-qj56) | PraisonAI | HITL tool approval cached by tool name — silently reused for subsequent calls with arbitrary arguments | — | CVE Assigned |
| 11 | [CVE-2026-62171](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-4r3p-w3mc-5v34) | PraisonAI | Prompt-injection defense blocks only when 3+ detector families fire simultaneously; single-vector injections pass through | — | CVE Assigned |
| 12 | [CVE-2026-48814](https://snailsploit.com/security-research/cves/cve-2026-48814/) | Network AI | Empty default secret accepted → authentication bypass (CWE-287/1188) | **High** | Published |
| 13 | [CVE-2026-54236](https://github.com/vllm-project/vllm/security/advisories/GHSA-hgg8-fqqc-vfmw) | vLLM | Incomplete CVE-2026-22778 fix → PIL repr ASLR-bypass infoleak via Anthropic router (CWE-532) | Medium (5.3) | Published |
| 14 | [CVE-2026-48782](https://github.com/pydantic/pydantic-ai/security/advisories) | pydantic-ai | SSRF — metadata blocklist bypass via IPv6 transition forms | Medium (6.8) | Published |

### linux kernel

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 15 | [CVE-2026-43121](https://nvd.nist.gov/vuln/detail/CVE-2026-43121) | Linux Kernel io_uring/zcrx | `user_ref` race → double-free → OOB write | Medium (4.7) | Published |
| 16 | [CVE-2026-46111](https://www.cve.org/CVERecord?id=CVE-2026-46111) | Linux Kernel Bluetooth/hci_conn | Use-After-Free in `create_big_sync` and `create_big_complete` handlers | Moderate (5.5) | Mainlined |
| 17 | [CVE-2026-46132](https://www.cve.org/CVERecord?id=CVE-2026-46132) | Linux Kernel net/rtnetlink | `ifla_vf_broadcast` stack infoleak via Netlink RTM_GETLINK | Low | Published |
| 18 | [CVE-2026-53371](https://www.cve.org/CVERecord?id=CVE-2026-53371) | Linux Kernel RDMA/ionic | Unbounded `%s` in `hca_type_show` reads past `node_desc[64]` — userspace-triggerable OOB read via sysfs | — | Published |

### infrastructure & orchestration

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 19 | [CVE-2026-3288](https://nvd.nist.gov/vuln/detail/CVE-2026-3288) | Kubernetes ingress-nginx | Config injection → RCE | **High (8.8)** | Published |
| 20 | [CVE-2026-30911](https://nvd.nist.gov/vuln/detail/CVE-2026-30911) | Apache Airflow Core | Missing auth (HITL) | **High (8.1)** | Published |
| 21 | [CVE-2026-32794](https://nvd.nist.gov/vuln/detail/CVE-2026-32794) | Apache Airflow (Databricks Provider) | TLS verification bypass → MitM | Medium (4.8) | Published |
| 22 | [CVE-2026-55070](https://github.com/argoproj/argo-workflows/security/advisories/GHSA-rcgr-27rh-g56w) | argoproj/argo-workflows | Informer-cache auth-bypass fix incomplete — Lint/Create resolve templates without per-caller auth (CWE-285) | Moderate (5.3) | CVE Assigned |
| 23 | [CVE-2026-48130](https://github.com/tektoncd/pipeline/security/advisories/GHSA-q6jr-jfqg-8m28) | tektoncd/pipeline | Hub resolver reads HTTP response body via unbounded `io.ReadAll` → OOM DoS (CWE-770) | Moderate (6.5) | CVE Assigned |

### CI/CD

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 24 | [CVE-2026-57303](https://www.jenkins.io/security/advisories/) | Jenkins Assembla plugin | XXE | **High** | Published |
| 25 | [CVE-2026-57297](https://www.jenkins.io/security/advisories/) | Jenkins Contrast CAS plugin | Missing permission check — connection-test → credential capture / SSRF | Medium | Published |
| 26 | [CVE-2026-57299](https://www.jenkins.io/security/advisories/) | Jenkins Contrast CAS plugin | Missing permission checks — metadata enumeration | Medium | Published |
| 27 | [CVE-2026-57304](https://www.jenkins.io/security/advisories/) | Jenkins Assembla plugin | Missing permission check | Medium | Published |
| 28 | [CVE-2026-57298](https://www.jenkins.io/security/advisories/) | Jenkins Contrast CAS plugin | CSRF | Medium | Published |
| 29 | [CVE-2026-57305](https://www.jenkins.io/security/advisories/) | Jenkins Assembla plugin | CSRF | Medium | Published |

### libraries & frameworks

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 30 | [CVE-2026-49853](https://github.com/tornadoweb/tornado/security/advisories/GHSA-3x9g-8vmp-wqvf) | tornadoweb/tornado | `Authorization` header forwarded across cross-origin redirects in `SimpleAsyncHTTPClient` | **High (7.7)** | Published |
| 31 | [CVE-2026-49353](https://github.com/decolua/9router/security/advisories/GHSA-6g2f-w7g3-77vf) | decolua/9router | Incomplete fix for CVE-2026-46339 — local-only access gate bypass via Host header spoofing (CWE-290) | **High (7.5)** | Published |
| 32 | [CVE-2026-31899](https://nvd.nist.gov/vuln/detail/CVE-2026-31899) | CairoSVG | Exponential DoS — recursive amplification | **High (7.5)** | Published |
| 33 | [CVE-2026-44840](https://github.com/dgraph-io/dgraph/security/advisories/GHSA-q2m9-6jp9-c6mc) | Dgraph | DQL injection via `checkUserPassword` GraphQL query | **High** | Published |
| 34 | [CVE-2026-52775](https://github.com/advisories) | yeswiki/yeswiki | Authenticated SQL injection via ReactionManager | **High** | Published |
| 35 | [CVE-2026-32809](https://www.cve.org/CVERecord?id=CVE-2026-32809) | ouch (Rust) | Symlink escape | **High (7.4)** | NVD: RESERVED |
| 36 | [CVE-2026-45363](https://github.com/jwt/ruby-jwt/security/advisories/GHSA-c32j-vqhx-rx3x) | jwt/ruby-jwt | Empty-key HMAC bypass | 7.4 | NVD: RESERVED |
| 37 | [CVE-2026-48022](https://github.com/advisories/GHSA-x426-x7cc-3fpc) | @hapi/wreck (npm) | Credential header leak on cross-port / cross-scheme redirect | Moderate | Published |
| 38 | [CVE-2026-54171](https://github.com/advisories) | Excon (RubyGems) | Sensitive/risky headers not redacted on redirect | Moderate | Published |
| 39 | [CVE-2026-33693](https://nvd.nist.gov/vuln/detail/CVE-2026-33693) | activitypub-federation-rust | SSRF — `0.0.0.0` bypass | Medium (6.5) | Published |
| 40 | [CVE-2026-32885](https://nvd.nist.gov/vuln/detail/CVE-2026-32885) | ddev/ddev | ZipSlip | Medium (6.5) | Published |
| 41 | [CVE-2026-8368](https://github.com/libwww-perl/libwww-perl/pull/512) | Perl `LWP::UserAgent` / `HTTP::Tiny` | Zero header strip on cross-host redirect | — | NVD: RESERVED |
| 42 | [CVE-2026-44217](https://nvd.nist.gov/vuln/detail/CVE-2026-44217) | sse-channel (npm) | SSE injection — unsanitized fields | Moderate | Published |
| 43 | [CVE-2026-46627](https://snailsploit.com/security-research/cves/cve-2026-46627/) | Twig (PHP) | Sandbox resource exhaustion — CPU/memory DoS | Moderate | Published |

### video / media platforms

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 44 | [CVE-2026-43884](https://nvd.nist.gov/vuln/detail/CVE-2026-43884) | AVideo | SSRF protection bypass via DNS rebinding | **High** | Published |
| 45 | [CVE-2026-43881](https://nvd.nist.gov/vuln/detail/CVE-2026-43881) | AVideo | Unauthenticated user enumeration via `isCompany` parameter | Medium (5.3) | Published |
| 46 | [CVE-2026-45619](https://github.com/advisories) | AVideo | CVE-2026-43884 incomplete fix — 6+ `isSSRFSafeURL()` call sites discard `$resolvedIP` out-param | — | Published |
| 47 | [CVE-2026-45620](https://github.com/advisories/GHSA-vpfx-pxqw-2w79) | AVideo | CVE-2026-43881 incomplete fix | — | Published |

### wordpress plugins

| # | CVE | Target | Type | Severity | Status |
|---|-----|--------|------|----------|--------|
| 48 | [CVE-2026-3596](https://nvd.nist.gov/vuln/detail/CVE-2026-3596) | Riaxe Product Customizer | Missing auth → priv esc | **Critical (9.8)** | Published |
| 49 | [CVE-2026-1313](https://nvd.nist.gov/vuln/detail/CVE-2026-1313) | MimeTypes Link Icons | SSRF | **High (8.3)** | Published |
| 50 | [CVE-2026-3599](https://nvd.nist.gov/vuln/detail/CVE-2026-3599) | Riaxe Product Customizer | Unauthenticated SQLi | **High (7.5)** | Published |
| 51 | [CVE-2025-9776](https://nvd.nist.gov/vuln/detail/CVE-2025-9776) | CatFolders | SQLi via CSV import | Medium (6.5) | Published |
| 52 | [CVE-2025-12163](https://nvd.nist.gov/vuln/detail/CVE-2025-12163) | Omnipress | Stored XSS | Medium (6.4) | Published |
| 53 | [CVE-2026-2717](https://nvd.nist.gov/vuln/detail/CVE-2026-2717) | HTTP Headers | CRLF injection | Medium (5.5) | Published |
| 54 | [CVE-2026-0811](https://nvd.nist.gov/vuln/detail/CVE-2026-0811) | Advanced CF7 DB | CSRF → form deletion | Medium (5.4) | Published |
| 55 | [CVE-2026-3594](https://nvd.nist.gov/vuln/detail/CVE-2026-3594) | Riaxe Product Customizer | Info disclosure — `/orders` | Medium (5.3) | Published |
| 56 | [CVE-2026-3595](https://nvd.nist.gov/vuln/detail/CVE-2026-3595) | Riaxe Product Customizer | Unauthenticated user deletion | Medium (5.3) | Published |
| 57 | [CVE-2026-1314](https://nvd.nist.gov/vuln/detail/CVE-2026-1314) | 3D FlipBook | Missing auth | Medium (5.3) | Published |
| 58 | [CVE-2025-11171](https://nvd.nist.gov/vuln/detail/CVE-2025-11171) | Chartify | Missing auth — admin function | Medium (5.3) | Published |
| 59 | [CVE-2025-11174](https://nvd.nist.gov/vuln/detail/CVE-2025-11174) | Document Library Lite | Missing auth → info disclosure | Medium (5.3) | Published |
| 60 | [CVE-2025-12030](https://nvd.nist.gov/vuln/detail/CVE-2025-12030) | ACF to REST API | IDOR | Medium (4.3) | Published |
| 61 | [CVE-2026-0814](https://nvd.nist.gov/vuln/detail/CVE-2026-0814) | Advanced CF7 DB | Missing auth — subscriber+ export | Medium (4.3) | Published |
| 62 | [CVE-2026-1208](https://nvd.nist.gov/vuln/detail/CVE-2026-1208) | Welcart | CSRF → settings update | Medium (4.3) | Published |
| 63 | [CVE-2026-15298](https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/telsender) | TelSender | Unauthenticated stored XSS via Telegram chat title | High (7.2) | Published |

---

## expanded attribution corpus

The CVE table above contains the core SnailSploit inventory plus the 16th WordPress finding. The following **9 additional CVEs** were identified through independent attribution sources (vendor/CNA/upstream/GitHub advisory records) during the broader reconciliation pass. They are included in the **92-CVE public attribution total** and are intentionally separated here so the provenance of the expanded count is explicit.

| CVE | Target | Attribution / source trail | Status |
|------|--------|---------------------------|--------|
| [CVE-2026-52778](https://snailsploit.com/cves) | YesWiki | SnailSploit disclosure ledger | Attributed |
| [CVE-2026-61308](https://www.oracle.com/security-alerts/cspuaug2026.html) | Oracle Java / `HttpURLConnection` | Oracle Critical Patch Update explicitly credits Kai Aizen | Confirmed |
| [CVE-2026-69261](https://snailsploit.com/cves) | Git LFS | SnailSploit disclosure ledger | Attributed |
| [CVE-2026-8661](https://snailsploit.com/cves) | Rapid7 InsightConnect | SnailSploit disclosure ledger | Attributed |
| [CVE-2026-54076](https://github.com/ArcadeData/arcadedb/security/advisories/GHSA-vg6x-6pg9-6qwg) | ArcadeDB | Upstream GitHub advisory explicitly credits Kai Aizen / SnailSploit | Confirmed |
| [CVE-2026-17351](https://www.pgadmin.org/docs/pgadmin4/9.17/release_notes_9_17.html) | pgAdmin 4 | Upstream pgAdmin release notes report Kai Aizen | Confirmed |
| [CVE-2026-70445](https://www.jenkins.io/security/advisory/2026-08-05/) | Jenkins Sauce OnDemand Plugin | Jenkins security advisory credits Kai Aizen / SnailSploit | Confirmed |
| [CVE-2026-19017](https://app.opencve.io/cve/CVE-2026-19017) | HashiCorp Consul | CNA record explicitly credits Kai Aizen / SnailSploit | Confirmed |
| [CVE-2026-60087](https://www.vulncheck.com/advisories/praisonai-before-tool-approval-cache-bypass) | PraisonAI | Independent advisory databases credit SnailSploit | Confirmed |

**Attribution note:** "92" is the expanded public-attribution corpus, not the number currently enumerated in the SnailSploit GitHub repository alone. The GitHub repository remains a 63-CVE core inventory; the expanded total incorporates independently located CVE records and the additional WordPress finding.

---

## linux kernel patches

five patches mainlined through the standard kernel maintainer process — four with assigned CVEs.

| Subsystem | Fix | CVE | Status |
|-----------|-----|-----|--------|
| `io_uring/zcrx` | Fix `user_ref` race between scrub and refill → double-free → OOB write | CVE-2026-43121 | Mainlined 7.0-rc1 |
| `Bluetooth/hci_conn` | UAF in `create_big_sync` and `create_big_complete` | CVE-2026-46111 | Mainlined |
| `net/rtnetlink` | Zero `ifla_vf_broadcast` to avoid stack infoleak | CVE-2026-46132 | Mainlined |
| `RDMA/ionic` | Bound `node_desc` sysfs read with `%.64s` — unbounded `%s` OOB read | CVE-2026-53371 | Mainlined |
| `net/tipc` | `tipc_mon_peer_up`/`down`/`remove_peer` UAF | — | Mainlined |

all patches on [lore.kernel.org →](https://lore.kernel.org/all/?q=Kai+Aizen)

---

## GHSAs, vendor findings & bounties

| ID | Target | Type | Status |
|----|--------|------|--------|
| — | [TelSender (WP)](https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/telsender) | Unauthenticated stored XSS via Telegram chat title (7.2) | Plugin taken down |
| [GHSA-j425-whc4-4jgc](https://github.com/advisories/GHSA-j425-whc4-4jgc) | OpenClaw | `system.run` env override RCE — allowlist bypass (6.3) | Published |
| [GHSA-gxhx-2686-5h9g](https://github.com/slack-go/slack/security/advisories/GHSA-gxhx-2686-5h9g) | slack-go/slack | Security advisory | Published |
| [GHSA-985r-q3qp-299h](https://github.com/advisories/GHSA-985r-q3qp-299h) | phpmyfaq/phpmyfaq | Incomplete fix — `editUser()` and `updateUserRights()` lack auth guards | Published |
| — | `@linear/sdk` | `LinearWebhooks.verify` accepts empty secret without precondition | Merged ($400 bounty) |

---

## frameworks & tooling

| Project | Description |
|---------|-------------|
| [**AATMF v3.1**](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) | Adversarial AI Threat Modeling Framework — 20 tactics, 240+ techniques, 2,152+ procedures, 4,980+ prompts. Crosswalks to OWASP LLM Top-10, NIST AI RMF, MITRE ATLAS, EU AI Act. On OWASP GenAI Security 2026 roadmap. YARA + Sigma detection signatures included. |
| [**AATMF Toolkit**](https://github.com/SnailSploit/aatmf-toolkit) | Python CLI for systematic LLM safety testing — three-layer evaluation pipeline, defense fingerprinting, regression tracking, attack chain planning. |
| [**Claude-Red**](https://github.com/SnailSploit/Claude-Red) | 58 offensive security skills across 13 categories for the Claude skills system. Drop a `SKILL.md` and Claude operates as a specialist — SQLi to shellcode, EDR evasion to ADCS abuse. |
| [**LLM Red Teamer's Playbook**](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) | Diagnostic methodology for bypassing LLM defense layers — input filters → alignment → identity → output → agentic trust. |
| [**Burp MCP Toolkit**](https://github.com/SnailSploit/Burp-MCP-Security-Analysis-Toolkit) | Skills-based security analysis — Burp Suite traffic capture with Claude Code reasoning via MCP. |
| [**JystDastIt**](https://github.com/SnailSploit/JystDastIt) | The Burp You Can Afford — open-source CLI DAST toolkit. |
| [**SnailObfuscator**](https://github.com/SnailSploit/SnailObfuscator) | Structurally-aware code obfuscation engine — polymorphic payload generation. |
| [**SnailHunter**](https://github.com/SnailSploit/SnailHunter) | AI-powered bug bounty automation — LLM analysis + traditional scanning. |
| [**KubeRoast**](https://github.com/SnailSploit/KubeRoast_v1) | Red-team Kubernetes misconfiguration & attack-path scanner. |
| [**Xposure**](https://github.com/SnailSploit/Xposure) | Autonomous credential intelligence platform for attack-surface recon. |
| [**SnailSploit Recon**](https://github.com/SnailSploit/SnailSploit_Recon_extension) | Chrome MV3 extension — passive recon, security headers, IP intel, CPE→CVE enrichment. |
| [**Awesome-Snail-OSINT**](https://github.com/SnailSploit/AwesomeSnailsOsint) | Curated OSINT resource collection for offensive recon. |
| [**P.R.O.M.P.T**](https://snailsploit.com/frameworks/prompt/) | Adversarial prompt engineering methodology — structured attack phases with Cialdini influence principles. |
| [**SEF**](https://snailsploit.com/frameworks/sef/) | Social Engineering Framework — organizational gap analysis, pretext selection, MITRE ATT&CK mapping. |

---

## research

published at [snailsploit.com](https://snailsploit.com), [Hakin9 Magazine](https://hakin9.org), and [Medium](https://medium.com/@snailsploit).

| Paper | Summary |
|-------|---------|
| [Self-Replicating Memory Worm](https://snailsploit.com/ai-security/self-replicating-memory-worm/) | Autonomous persistence — skill injection + memory poisoning = self-healing implant. Four-stage kill chain, no jailbreak. |
| [Memory Injection Through Nested Skills](https://snailsploit.com/ai-security/nested-skill-injection/) | Dual-persistence architecture: memory slots and skill files, each restoring the other on boot. |
| [Weaponized AI Supply Chain](https://snailsploit.com/ai-security/weaponized-ai-supply-chain/) | End-to-end supply chain attack through AI agent skill injection, validated against DVWA and Juice Shop. |
| [AI Gateway Threat Model (TC-21)](https://snailsploit.com/ai-security/ai-gateway-threat-model/) | First generalized threat model for AI gateways — 8 attack vectors, proposed as AATMF v3 TC-21. |
| [MCP vs A2A Attack Surface](https://snailsploit.com/ai-security/mcp-vs-a2a/) | Comparative threat model — where MCP and Agent-to-Agent diverge in trust boundaries. |
| [The 30% Blind Spot](https://snailsploit.com/ai-security/llm-safety-judges/) | LLM-as-judge safety classifiers miss ~30% of adversarial output classes. |
| [AI Breach Detection Gap](https://snailsploit.com/ai-security/ai-breach-detection-gap/) | Detection blind spots in AI-integrated production systems. |
| [AI Coding Agent Attack Surface](https://snailsploit.com/ai-security/ai-coding-agent-attack-surface/) | Attack surface analysis of AI-powered coding assistants and their tool-use capabilities. |
| [Agentic AI Threat Landscape](https://snailsploit.com/ai-security/agentic-ai-threat-landscape/) | Threat landscape survey of autonomous AI agent architectures. |
| [Adversarial Prompting: Complete Guide](https://snailsploit.com/ai-security/adversarial-prompting/) | End-to-end methodology — direct, indirect, multi-turn, and agentic prompt injection. |
| [Computational Countertransference](https://snailsploit.com/ai-security/computational-countertransference/) | The psychology of human–AI manipulation dynamics. |
| [AATMF v3.1 vs MITRE ATLAS](https://snailsploit.com/ai-security/aatmf-vs-mitre-atlas/) | Framework comparison — coverage gaps in existing AI threat taxonomies. |
| [The Memory Manipulation Problem](https://snailsploit.com/ai-security/jailbreaking/memory-manipulation-attacks/) | How attackers exploit persistent context to compromise future interactions. |
| [ChatGPT Canvas DNS Exfiltration](https://github.com/SnailSploit/ChatGPT-DNS-Exfill) | DNS exfil via ChatGPT Canvas — rendered content triggers DNS lookups without outbound HTTP. |
| [ChatGPT Sandbox RCE + DNS Exfil](https://github.com/SnailSploit/chatgpt-rce-dns) | Pickle deserialization RCE chained with DNS exfiltration to escape Code Interpreter sandbox. |
| [Double AI, Triple Mechanism](https://snailsploit.com/ai-security/cloud-obfuscator/) | Cloud-based obfuscator attack research. |
| [Linux Kernel io_uring/zcrx Race Condition](https://snailsploit.com/security-research/general/io-uring-zcrx-race-condition/) | Race condition → double-free → OOB write in io_uring zero-copy receive. Mainlined; CVE-2026-43121. |

---

## summary

| Metric | Count |
|--------|-------|
| Publicly attributable CVEs | 92 |
| — critical | 5 |
| — high | 18 |
| Distinct targets | 27 |
| Mainlined linux kernel patches | 5 |
| Kernel CVEs | 4 |
| GHSAs / vendor disclosures / bounties | 5+ |
| Published frameworks | 3 (AATMF, SEF, P.R.O.M.P.T) |
| Open-source tools | 11 |

> **cross-reference note:** CVE-2026-43121, CVE-2026-46111, CVE-2026-46132, and CVE-2026-53371 each appear once in the CVE table and once in the kernel patches section — same finding, listed in both places for discoverability. CVE-2026-48022 (@hapi/wreck) appears once in the CVE table; its GHSA is the same finding.

**sources of record:** [Wordfence](https://www.wordfence.com/threat-intel/vulnerabilities/researchers/kai-aizen) · [GHSA Credit](https://github.com/advisories?query=credit%3ASnailSploit) · [GitHub](https://github.com/SnailSploit) · [lore.kernel.org](https://lore.kernel.org/all/?q=Kai+Aizen)

---

[![snailsploit](https://img.shields.io/badge/read_the_research-snailsploit.com-E07A4A?style=flat-square&labelColor=0E0E0F)](https://snailsploit.com)

`same attack. different substrate.`
