[![snailsploit — same attack. different substrate.](https://github.com/SnailSploit/SnailSploit/raw/main/banner.png)](https://snailsploit.com)

**adversarial ai research · llm red teaming · kernel · vulnerability research**

[![Website](https://img.shields.io/badge/snailsploit.com-0E0E0F?style=flat-square&logo=astro&logoColor=E9E7E1&labelColor=0E0E0F)](https://snailsploit.com) [![The Jailbreak Chef](https://img.shields.io/badge/the_jailbreak_chef-0E0E0F?style=flat-square&logo=fireship&logoColor=E9E7E1&labelColor=0E0E0F)](https://thejailbreakchef.com) [![LinkedIn](https://img.shields.io/badge/linkedin-0E0E0F?style=flat-square&logo=linkedin&logoColor=E9E7E1&labelColor=0E0E0F)](https://linkedin.com/in/kaiaizen) [![Medium](https://img.shields.io/badge/medium-0E0E0F?style=flat-square&logo=medium&logoColor=E9E7E1&labelColor=0E0E0F)](https://medium.com/@snailsploit)

---

same attack. different substrate.

snailsploit is an independent adversarial research group — vulnerability research, framework development, and offensive tooling across kernels, language models, and everything between them.


---
# Complete CVE Corpus (Kai Aizen)

Updated against master portfolio digest (2026-10-12). Joint findings with Avraham Shemesh marked. Reserved/unpublished noted. Rejected/dup omitted.

| # | CVE | Target | Finding | Severity | Status |
| -: | :--- | :--- | :--- | :--- | :--- |
| 1 | [CVE-2026-46111](https://www.cve.org/CVERecord?id=CVE-2026-46111) | Linux Kernel (Bluetooth/hci_conn) | Use-After-Free in create_big_sync / create_big_complete | High | Mainlined |
| 2 | [CVE-2026-64293](https://git.kernel.org/pub/scm/linux/kernel/git/torvalds/linux.git/commit/?id=be93d186ae88a92e7) | Linux Kernel (iommufd veventq) | High severity flaw | High | Mainlined |
| 3 | [CVE-2026-46132](https://www.cve.org/CVERecord?id=CVE-2026-46132) | Linux Kernel (net/rtnetlink) | ifla_vf_broadcast kernel stack memory leak | Medium | Mainlined |
| 4 | [CVE-2026-53371](https://lkml.iu.edu/hypermail/linux/kernel/2604.1/03379.html) | Linux Kernel (RDMA/ionic) | Unbounded %s → OOB read through sysfs | Medium | Mainlined |
| 5 | [CVE-2026-64233](https://www.cve.org/CVERecord?id=CVE-2026-64233) | Linux Kernel (usb: gadget: uvc) | Medium severity issue | Medium | Mainlined |
| 6 | [CVE-2026-43121](https://www.cve.org/CVERecord?id=CVE-2026-43121) | Linux Kernel (io_uring/zcrx) | user_ref race condition → double-free → OOB write | Medium | Mainlined (v6.18.16) |
| 7 | [CVE-2026-30911](https://www.cve.org/CVERecord?id=CVE-2026-30911) | Apache Airflow Core | Missing per-task authorization on HITL endpoints | High | Published |
| 8 | [CVE-2026-32794](https://www.cve.org/CVERecord?id=CVE-2026-32794) | Apache Airflow Databricks | TLS certificate verification bypass | Medium | Published |
| 9 | [CVE-2026-61308](https://openjdk.org/groups/vulnerability/advisories/2026-08-18) | Oracle Java / GraalVM | Networking / credential leakage across redirects | Medium | Published |
| 10 | [CVE-2026-3288](https://groups.google.com/g/kubernetes-security-announce/c/E9bLHAD6-eg) | Kubernetes ingress-nginx | Configuration injection → RCE | High | Published |
| 11 | [CVE-2026-19017](https://discuss.hashicorp.com/t/hcsec-2026-25-multiple-vulnerabilities-impacting-hashicorp-cons) | HashiCorp / IBM Consul | ACL token evaluation bypass | Medium | Published |
| 12 | [CVE-2026-93576](https://github.com/advisories/ghsa-5vh9-c45f-rf7p) | Netty (netty-codec-smtp) | High severity issue | High | Published |
| 13 | [CVE-2026-69261](https://github.com/advisories/ghsa-x7xj-4j4f-88xr) | Git LFS | SSH credential handling | — | not yet published |
| 14 | [CVE-2026-55070](https://github.com/advisories/ghsa-rcgr-27rh-g56w) | argoproj/argo-workflows | Incomplete authorization bypass | Medium | not yet published |
| 15 | [CVE-2026-57303](https://www.jenkins.io/security/advisory/2026-06-24/) | Jenkins Assembla | XML External Entity (XXE) Injection | High | Published |
| 16 | [CVE-2026-84674](https://www.jenkins.io/security/advisory/2026-09-02/) | Jenkins XebiaLabs XL Deploy | Medium severity | Medium | Published |
| 17 | [CVE-2026-57297](https://www.jenkins.io/security/advisory/2026-06-24/) | Jenkins Contrast CAS | Missing permission check | Medium | Published |
| 18 | [CVE-2026-57298](https://www.jenkins.io/security/advisory/2026-06-24/) | Jenkins Contrast CAS | CSRF | Medium | Published |
| 19 | [CVE-2026-57304](https://www.jenkins.io/security/advisory/2026-06-24/) | Jenkins Assembla | Missing permission check | Medium | Published |
| 20 | [CVE-2026-57305](https://www.jenkins.io/security/advisory/2026-06-24/) | Jenkins Assembla | CSRF | Medium | Published |
| 21 | [CVE-2026-70445](https://www.jenkins.io/security/advisory/2026-08-05/) | Jenkins Sauce OnDemand | Impersonation & permission check missing | Medium | Published |
| 22 | [CVE-2026-57299](https://www.jenkins.io/security/advisory/2026-06-24/) | Jenkins Contrast CAS | Metadata & workspace enumeration | Medium | Published |
| 23 | [CVE-2026-8661](https://www.cve.org/CVERecord?id=CVE-2026-8661) | Rapid7 InsightConnect | Markdown to PDF plugin issue | Medium | Published |
| 24 | [CVE-2026-48130](https://github.com/advisories/ghsa-q6jr-jfqg-8m28) | tektoncd/pipeline | Unbounded response read → OOM DoS | Medium | not yet published |
| 25 | [CVE-2026-17351](https://github.com/pgadmin-org/pgadmin4/commit/ef76102bcd1cdb544eb9b4ef18d3382f22b76752) | pgAdmin 4 | Code injection in desktop runtime | Critical | Published |
| 26 | [CVE-2026-46627](https://symfony.com/blog/cve-2026-46627-sandbox-does-not-protect-against-resource-exhaustion) | Twig (PHP) | Sandbox does not protect against resource exhaustion | Medium | Published |
| 27 | [CVE-2026-94608](https://github.com/advisories/ghsa-v445-fmf5-mhp8) | goauthentik/authentik | High severity | High | not yet published |
| 28 | [CVE-2026-54236](https://github.com/advisories/GHSA-hgg8-fqqc-vfmw) | vLLM | Information leak enabling ASLR bypass | Medium | Published |
| 29 | [CVE-2026-48782](https://github.com/advisories/GHSA-cg7w-rg45-pc59) | pydantic-ai | SSRF metadata blocklist bypass | Medium | Published |
| 30 | [CVE-2026-47393](https://github.com/advisories/GHSA-8444-4fhq-fxpq) | PraisonAI | Authentication disabled by default | Critical | Published |
| 31 | [CVE-2026-57127](https://github.com/advisories/GHSA-j4hj-7hfh-g2f4) | PraisonAI | recipe serve auth middleware disables itself | Critical | Published |
| 32 | [CVE-2026-57131](https://github.com/advisories/GHSA-fq2m-6wqh-x44g) | PraisonAI | Jobs API without authentication | Critical | Published |
| 33 | [CVE-2026-57147](https://github.com/advisories/GHSA-cwj8-7gp2-ggcw) | PraisonAI | Hardcoded default JWT signing secret | Critical | Published |
| 34 | [CVE-2026-57126](https://github.com/advisories/GHSA-vxgj-xg5c-p4h7) | PraisonAI | SSRF guard without DNS resolution | High | Published |
| 35 | [CVE-2026-55528](https://github.com/advisories/GHSA-7g3p-92qq-8wvh) | PraisonAI | AgentServer auth_token not enforced | High | Published |
| 36 | [CVE-2026-47398](https://github.com/advisories/GHSA-78r8-wwqv-r299) | PraisonAI | Code injection through exec_module | High | Published |
| 37 | [CVE-2026-57120](https://github.com/advisories/GHSA-pv2j-rghr-v5r9) | PraisonAI | execute_code sandbox bypass | Medium | Published |
| 38 | [CVE-2026-55530](https://github.com/advisories/GHSA-cfxv-8fw8-rwpv) | PraisonAI | ast_grep_rewrite modifies arbitrary files | Medium | Published |
| 39 | [CVE-2026-60087](https://github.com/advisories/GHSA-29r9-67vg-qj56) | PraisonAI | Tool approval caching bypass | Medium | Published |
| 40 | [CVE-2026-60086](https://github.com/advisories/GHSA-4r3p-w3mc-5v34) | PraisonAI | Medium severity | Medium | Published |
| 41 | [CVE-2026-49853](https://github.com/tornadoweb/tornado/blob/master/docs/releases/v6.5.6.rst) | tornadoweb/tornado | Authorization header forwarded across redirects | High | Published |
| 42 | [CVE-2026-79777](https://osv.dev/vulnerability/GO-2026-6181) | rclone (Go) | Low severity | Low | Published |
| 43 | [CVE-2026-44840](https://github.com/advisories/GHSA-q2m9-6jp9-c6mc) | Dgraph (Go) | DQL Injection | High | Published |
| 44 | [CVE-2026-54076](https://github.com/advisories/ghsa-vg6x-6pg9-6qwg) | ArcadeDB | High severity | High | Published |
| 45 | [CVE-2026-8368](https://lists.security.metacpan.org/cve-announce/msg/39974665/) | Perl LWP::UserAgent | Medium severity | Medium | Published |
| 46 | [CVE-2026-48022](https://github.com/advisories/GHSA-x426-x7cc-3fpc) | @hapi/wreck (npm) | Medium severity | Medium | Published |
| 47 | [CVE-2026-96754](https://github.com/advisories/ghsa-g4mf-q5hw-f9j9) | orval @orval/hono | High — credit dispute (correction pending) | High | Published |
| 48 | [CVE-2026-96757](https://github.com/advisories/ghsa-rcpr-mq4m-jx9j) | orval @orval/fetch / core | High — credit dispute (correction pending) | High | Published |
| 49 | [CVE-2026-107715](https://github.com/advisories/GHSA-2mwr-xjcg-37j7) | mechanize (RubyGems) | Medium severity | Medium | Published |
| 50 | [CVE-2026-54171](https://github.com/advisories/GHSA-48rx-c7pg-q66r) | Excon (RubyGems) | Medium severity | Medium | Published |
| 51 | [CVE-2026-45363](https://github.com/advisories/GHSA-c32j-vqhx-rx3x) | jwt (RubyGems) | Empty-key HMAC signature verification bypass | High | Published |
| 52 | [CVE-2026-31899](https://github.com/advisories/GHSA-f38f-5xpm-9r7c) | Kozea/CairoSVG | Recursive SVG amplification → exponential DoS | High | Published |
| 53 | [CVE-2026-32885](https://github.com/advisories/GHSA-x2xq-qhjf-5mvg) | github.com/ddev/ddev | ZipSlip / path traversal | Medium | Published |
| 54 | [CVE-2026-43884](https://github.com/advisories/GHSA-2hch-c97c-g99x) | WWBN/AVideo | High severity | High | Published |
| 55 | [CVE-2026-45619](https://github.com/advisories/GHSA-c3ch-22rq-xfwr) | WWBN/AVideo | Medium severity | Medium | Published |
| 56 | [CVE-2026-45620](https://github.com/advisories/GHSA-vpfx-pxqw-2w79) | WWBN/AVideo | Medium severity | Medium | Published |
| 57 | [CVE-2026-56396](https://www.cve.org/CVERecord?id=CVE-2026-56396) | phpMyFAQ | High severity | High | Published |
| 58 | [CVE-2026-52775](https://github.com/advisories/GHSA-4pf7-cc4r-g63h) | yeswiki/yeswiki | High severity | High | Published |
| 59 | [CVE-2026-33693](https://github.com/advisories/GHSA-q537-8fr5-cw35) | activitypub-federation-rust | SSRF via 0.0.0.0 bypass | Medium | Published |
| 60 | [CVE-2026-32809](https://github.com/advisories/ghsa-pcw6-cg54-qvm8) | ouch (Rust) | Symlink path traversal | High | not yet published |
| 61 | [CVE-2026-44217](https://github.com/advisories/GHSA-84hm-wfh8-c5pg) | sse-channel (npm) | SSE injection | Medium | Published |
| 62 | [CVE-2026-49353](https://github.com/advisories/GHSA-6g2f-w7g3-77vf) | decolua/9router | Host-header access-gate bypass | High | Published |
| 63 | [CVE-2026-48814](https://github.com/advisories/GHSA-r78r-rwrf-rjwp) | Network AI (npm) | Empty default secret → auth bypass | Critical | Published |
| 64 | [CVE-2026-1314](https://www.cve.org/CVERecord?id=CVE-2026-1314) | WordPress - 3D FlipBook | Missing authentication checks | Medium | Published |
| 65 | [CVE-2025-12030](https://www.cve.org/CVERecord?id=CVE-2025-12030) | WordPress - ACF to REST API | IDOR | Medium | Published |
| 66 | [CVE-2026-0811](https://www.cve.org/CVERecord?id=CVE-2026-0811) | WordPress - Advanced CF7 DB | CSRF → form deletion | Medium | Published |
| 67 | [CVE-2026-0814](https://www.cve.org/CVERecord?id=CVE-2026-0814) | WordPress - Advanced CF7 DB | Unauthorized database export | Medium | Published |
| 68 | [CVE-2025-9776](https://www.cve.org/CVERecord?id=CVE-2025-9776) | WordPress - CatFolders | SQL injection via CSV import | Medium | Published |
| 69 | [CVE-2025-11171](https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/chart-builder/chartify) | WordPress - Chartify (joint w/ Avraham Shemesh) | Missing authentication | Medium | Published |
| 70 | [CVE-2025-11174](https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/document-library-lite/) | WordPress - Document Library Lite (joint w/ Avraham Shemesh) | Missing authentication → info disclosure | Medium | Published |
| 71 | [CVE-2026-1208](https://www.cve.org/CVERecord?id=CVE-2026-1208) | WordPress - Friendly Functions for Welcart | CSRF → settings update | Medium | Published |
| 72 | [CVE-2026-2717](https://www.cve.org/CVERecord?id=CVE-2026-2717) | WordPress - HTTP Headers | CRLF Injection | Medium | Published |
| 73 | [CVE-2026-1313](https://www.cve.org/CVERecord?id=CVE-2026-1313) | WordPress - MimeTypes Link Icons | SSRF | High | Published |
| 74 | [CVE-2025-12163](https://www.cve.org/CVERecord?id=CVE-2025-12163) | WordPress - Omnipress | Stored XSS | Medium | Published |
| 75 | [CVE-2026-3596](https://www.cve.org/CVERecord?id=CVE-2026-3596) | WordPress - Riaxe Product Customizer | Missing authentication → privilege escalation | Critical | Published |
| 76 | [CVE-2026-3599](https://www.cve.org/CVERecord?id=CVE-2026-3599) | WordPress - Riaxe Product Customizer | Unauthenticated SQL injection | High | Published |
| 77 | [CVE-2026-3594](https://www.cve.org/CVERecord?id=CVE-2026-3594) | WordPress - Riaxe Product Customizer | Unauthenticated information disclosure | Medium | Published |
| 78 | [CVE-2026-3595](https://www.cve.org/CVERecord?id=CVE-2026-3595) | WordPress - Riaxe Product Customizer | Unauthenticated arbitrary user deletion | Medium | Published |
| 79 | [CVE-2026-15298](https://www.cve.org/CVERecord?id=CVE-2026-15298) | WordPress - TelSender | Unauthenticated stored XSS | High | Published |

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
| [Memory Injection Through Nested Skills](https://snailsploit.com/ai-security/memory-injection-nested-skills/) | Persistent autonomous operator via skills + memory + MCP. Submitted to Anthropic. |
| [AI Output Classifier Gap](https://snailsploit.com/ai-security/ai-output-classifier-gap/) | Classifiers miss ~30% of adversarial output classes. |
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

**sources of record:** [Wordfence](https://www.wordfence.com/threat-intel/vulnerabilities/researchers/kai-aizen) · [GHSA Credit](https://github.com/advisories?query=credit%3ASnailSploit) · [GitHub](https://github.com/SnailSploit) · [lore.kernel.org](https://lore.kernel.org/all/?q=Kai+Aizen)

---

[![snailsploit](https://img.shields.io/badge/read_the_research-snailsploit.com-E07A4A?style=flat-square&labelColor=0E0E0F)](https://snailsploit.com)

`same attack. different substrate.`
