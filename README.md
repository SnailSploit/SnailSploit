[![snailsploit — same attack. different substrate.](https://github.com/SnailSploit/SnailSploit/raw/main/banner.png)](https://snailsploit.com)

**adversarial ai research · llm red teaming · kernel · vulnerability research**

[![Website](https://img.shields.io/badge/snailsploit.com-0E0E0F?style=flat-square&logo=astro&logoColor=E9E7E1&labelColor=0E0E0F)](https://snailsploit.com) [![The Jailbreak Chef](https://img.shields.io/badge/the_jailbreak_chef-0E0E0F?style=flat-square&logo=fireship&logoColor=E9E7E1&labelColor=0E0E0F)](https://thejailbreakchef.com) [![LinkedIn](https://img.shields.io/badge/linkedin-0E0E0F?style=flat-square&logo=linkedin&logoColor=E9E7E1&labelColor=0E0E0F)](https://linkedin.com/in/kaiaizen) [![Medium](https://img.shields.io/badge/medium-0E0E0F?style=flat-square&logo=medium&logoColor=E9E7E1&labelColor=0E0E0F)](https://medium.com/@snailsploit)

---

same attack. different substrate.

snailsploit is an independent adversarial research group — vulnerability research, framework development, and offensive tooling across kernels, language models, and everything between them.


---
# Complete CVE Corpus (Kai Aizen)

| # | CVE | Target | Finding | Severity / Category | Status |
| -: | :--- | :--- | :--- | :--- | :--- |
| 1 | [CVE-2026-47393](https://snailsploit.com/security-research/cves/cve-2026-47393/) | PraisonAI | Authentication disabled by default | **Critical 9.8** | Published |
| 2 | [CVE-2026-57127](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | `recipe serve` auth middleware disables itself when secret is missing | **Critical 9.8** | Published |
| 3 | [CVE-2026-57131](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | Jobs API exposes agent-execution endpoints without authentication | **Critical 9.8** | Published |
| 4 | [CVE-2026-57147](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | Hardcoded default JWT signing secret enables token forgery | **Critical 9.8** | Published |
| 5 | [CVE-2026-3596](https://nvd.nist.gov/vuln/detail/CVE-2026-3596) | Riaxe Product Customizer | Missing authentication → privilege escalation | **Critical 9.8** | Published |
| 6 | [CVE-2026-3288](https://nvd.nist.gov/vuln/detail/CVE-2026-3288) | Kubernetes ingress-nginx | Configuration injection → Remote Code Execution | **High 8.8** | Published |
| 7 | [CVE-2026-57126](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | SSRF guard validates literal IPs without DNS resolution | **High 8.5** | Published |
| 8 | [CVE-2026-1313](https://nvd.nist.gov/vuln/detail/CVE-2026-1313) | MimeTypes Link Icons | Server-Side Request Forgery (SSRF) | **High 8.3** | Published |
| 9 | [CVE-2026-55528](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-7g3p-92qq-8wvh) | PraisonAI | `AgentServer` declares `auth_token` but does not enforce it on routes | **High 8.2** | Published |
| 10 | [CVE-2026-47398](https://snailsploit.com/security-research/cves/cve-2026-47398/) | PraisonAI | Code injection through `exec_module` and YAML-controlled module paths | **High 8.1** | Published |
| 11 | [CVE-2026-30911](https://nvd.nist.gov/vuln/detail/CVE-2026-30911) | Apache Airflow | Missing per-task authorization on HITL endpoints | **High 8.1** | Published |
| 12 | [CVE-2026-3599](https://nvd.nist.gov/vuln/detail/CVE-2026-3599) | Riaxe Product Customizer | Unauthenticated SQL injection | **High 7.5** | Published |
| 13 | [CVE-2026-15298](https://www.wordfence.com/threat-intel/vulnerabilities/wordpress-plugins/telsender) | TelSender | Unauthenticated stored XSS via messaging pipeline | **High 7.2** | Published |
| 14 | [CVE-2026-48814](https://snailsploit.com/security-research/cves/cve-2026-48814/) | Network AI | Empty default secret accepted → authentication bypass | **High** | Published |
| 15 | [CVE-2026-48782](https://github.com/pydantic/pydantic-ai/security/advisories) | pydantic-ai | SSRF metadata blocklist bypass through IPv6 transition forms | Medium 6.8 | Published |
| 16 | [CVE-2025-9776](https://nvd.nist.gov/vuln/detail/CVE-2025-9776) | CatFolders | SQL injection via CSV import module | Medium 6.5 | Published |
| 17 | [CVE-2026-57120](https://github.com/MervinPraison/PraisonAI/security/advisories) | PraisonAI | `execute_code` sandbox bypass through `str.format` dunder access | Medium 6.5 | Published |
| 18 | [CVE-2026-48130](https://github.com/tektoncd/pipeline/security/advisories/GHSA-q6jr-jfqg-8m28) | Tekton Pipelines | Unbounded response read → OOM Denial of Service | Moderate 6.5 | CVE Assigned |
| 19 | [CVE-2025-12163](https://nvd.nist.gov/vuln/detail/CVE-2025-12163) | Omnipress | Stored Cross-Site Scripting (XSS) | Medium 6.4 | Published |
| 20 | [CVE-2026-55530](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-cfxv-8fw8-rwpv) | PraisonAI | `ast_grep_rewrite` modifies arbitrary local files without approval | Moderate 6.1 | Published |
| 21 | [CVE-2026-2717](https://nvd.nist.gov/vuln/detail/CVE-2026-2717) | HTTP Headers | CRLF Injection in header processing | Medium 5.5 | Published |
| 22 | [CVE-2026-0811](https://nvd.nist.gov/vuln/detail/CVE-2026-0811) | Advanced CF7 DB | Cross-Site Request Forgery (CSRF) → form deletion | Medium 5.4 | Published |
| 23 | [CVE-2026-54236](https://github.com/vllm-project/vllm/security/advisories/GHSA-hgg8-fqqc-vfmw) | vLLM | Anthropic router information leak enabling ASLR bypass | Medium 5.3 | Published |
| 24 | [CVE-2026-55070](https://github.com/argoproj/argo-workflows/security/advisories/GHSA-rcgr-27rh-g56w) | Argo Workflows | Incomplete authorization bypass fix | Moderate 5.3 | CVE Assigned |
| 25 | [CVE-2026-3594](https://nvd.nist.gov/vuln/detail/CVE-2026-3594) | Riaxe Product Customizer | Unauthenticated information disclosure | Medium 5.3 | Published |
| 26 | [CVE-2026-3595](https://nvd.nist.gov/vuln/detail/CVE-2026-3595) | Riaxe Product Customizer | Unauthenticated arbitrary user deletion | Medium 5.3 | Published |
| 27 | [CVE-2026-1314](https://nvd.nist.gov/vuln/detail/CVE-2026-1314) | 3D FlipBook | Missing authentication checks on REST endpoints | Medium 5.3 | Published |
| 28 | [CVE-2025-11171](https://nvd.nist.gov/vuln/detail/CVE-2025-11171) | Chartify | Missing authentication on administrative function | Medium 5.3 | Published |
| 29 | [CVE-2025-11174](https://nvd.nist.gov/vuln/detail/CVE-2025-11174) | Document Library Lite | Missing authentication → sensitive information disclosure | Medium 5.3 | Published |
| 30 | [CVE-2026-32794](https://nvd.nist.gov/vuln/detail/CVE-2026-32794) | Apache Airflow / Databricks | TLS certificate verification bypass | Medium 4.8 | Published |
| 31 | [CVE-2025-12030](https://nvd.nist.gov/vuln/detail/CVE-2025-12030) | ACF to REST API | Insecure Direct Object Reference (IDOR) | Medium 4.3 | Published |
| 32 | [CVE-2026-0814](https://nvd.nist.gov/vuln/detail/CVE-2026-0814) | Advanced CF7 DB | Unauthorized database export | Medium 4.3 | Published |
| 33 | [CVE-2026-1208](https://nvd.nist.gov/vuln/detail/CVE-2026-1208) | Welcart | CSRF → global store settings update | Medium 4.3 | Published |
| 34 | [CVE-2026-43121](https://nvd.nist.gov/vuln/detail/CVE-2026-43121) | Linux Kernel (`io_uring/zcrx`) | `user_ref` race condition → double-free → OOB write | Kernel | Mainlined |
| 35 | [CVE-2026-46111](https://www.cve.org/CVERecord?id=CVE-2026-46111) | Linux Kernel (`Bluetooth/hci_conn`) | Use-After-Free in `create_big_sync` / `create_big_complete` | Kernel | Mainlined |
| 36 | [CVE-2026-46132](https://www.cve.org/CVERecord?id=CVE-2026-46132) | Linux Kernel (`net/rtnetlink`) | `ifla_vf_broadcast` kernel stack memory leak | Kernel | Mainlined |
| 37 | [CVE-2026-53371](https://www.cve.org/CVERecord?id=CVE-2026-53371) | Linux Kernel (`RDMA/ionic`) | Unbounded `%s` → OOB read through sysfs boundary | Kernel | Mainlined |
| 38 | [CVE-2026-57303](https://www.jenkins.io/security/advisories/) | Jenkins Assembla | XML External Entity (XXE) Injection | CI/CD | Published |
| 39 | [CVE-2026-57297](https://www.jenkins.io/security/advisories/) | Jenkins Contrast CAS | Missing permission check → credential capture / SSRF | CI/CD | Published |
| 40 | [CVE-2026-57299](https://www.jenkins.io/security/advisories/) | Jenkins Contrast CAS | Metadata & workspace enumeration | CI/CD | Published |
| 41 | [CVE-2026-57304](https://www.jenkins.io/security/advisories/) | Jenkins Assembla | Missing permission check on management handlers | CI/CD | Published |
| 42 | [CVE-2026-57298](https://www.jenkins.io/security/advisories/) | Jenkins Contrast CAS | Cross-Site Request Forgery (CSRF) | CI/CD | Published |
| 43 | [CVE-2026-57305](https://www.jenkins.io/security/advisories/) | Jenkins Assembla | Cross-Site Request Forgery (CSRF) | CI/CD | Published |
| 44 | [CVE-2026-70445](https://www.jenkins.io/security/advisory/2026-08-05/) | Jenkins Sauce OnDemand | Impersonation & permission check missing | CI/CD | Published |
| 45 | [CVE-2026-49853](https://github.com/tornadoweb/tornado/security/advisories/GHSA-3x9g-8vmp-wqvf) | Tornado | `Authorization` header forwarded across cross-origin redirects | Frameworks | Published |
| 46 | [CVE-2026-49353](https://github.com/decolua/9router/security/advisories/GHSA-6g2f-w7g3-77vf) | 9router | Host-header access-gate security bypass | Frameworks | Published |
| 47 | [CVE-2026-31899](https://nvd.nist.gov/vuln/detail/CVE-2026-31899) | CairoSVG | Recursive SVG entity amplification → exponential DoS | Libraries | Published |
| 48 | [CVE-2026-44840](https://github.com/dgraph-io/dgraph/security/advisories/GHSA-q2m9-6jp9-c6mc) | Dgraph | DQL Injection via unescaped string interpolation | Database | Published |
| 49 | [CVE-2026-32809](https://www.cve.org/CVERecord?id=CVE-2026-32809) | `ouch` | Symlink path traversal during archive extraction | CLI Tooling | Published |
| 50 | [CVE-2026-45363](https://github.com/jwt/ruby-jwt/security/advisories/GHSA-c32j-vqhx-rx3x) | Ruby JWT | Empty-key HMAC signature verification bypass | Security Lib | Published |
| 51 | [CVE-2026-33693](https://nvd.nist.gov/vuln/detail/CVE-2026-33693) | activitypub-federation-rust | SSRF protection bypass through `0.0.0.0` binding | Federation | Published |
| 52 | [CVE-2026-32885](https://nvd.nist.gov/vuln/detail/CVE-2026-32885) | DDEV | ZipSlip arbitrary file overwrite in environment restoration | Dev Tooling | Published |
| 53 | [CVE-2026-44217](https://nvd.nist.gov/vuln/detail/CVE-2026-44217) | sse-channel | Server-Sent Events (SSE) injection via unescaped newlines | Protocol | Published |
| 54 | [CVE-2026-46627](https://snailsploit.com/security-research/cves/cve-2026-46627/) | Twig | Sandbox escape & infinite loop memory exhaustion | Templating | Published |
| 55 | [CVE-2026-52778](https://snailsploit.com/cves) | YesWiki | Template injection leading to arbitrary code execution | CMS | Published |
| 56 | [CVE-2026-61308](https://www.oracle.com/security-alerts/cspuaug2026.html) | Oracle Java / `HttpURLConnection` | Credential leakage across cross-origin HTTP redirects | Runtime | Published |
| 57 | [CVE-2026-69261](https://snailsploit.com/cves) | Git LFS | SSH credential handling boundary failure | Dev Tooling | Published |
| 58 | [CVE-2026-8661](https://snailsploit.com/cves) | Rapid7 InsightConnect | Workflow execution authorization bypass | SOAR | Published |
| 59 | [CVE-2026-54076](https://github.com/ArcadeData/arcadedb/security/advisories/GHSA-vg6x-6pg9-6qwg) | ArcadeDB | DQL injection & arbitrary directory path traversal | Database | Published |
| 60 | [CVE-2026-17351](https://www.pgadmin.org/docs/pgadmin4/9.17/release_notes_9_17.html) | pgAdmin 4 | Code injection vulnerability in desktop runtime container | Database | Published |
| 61 | [CVE-2026-19017](https://app.opencve.io/cve/CVE-2026-19017) | HashiCorp Consul | ACL token evaluation bypass via agent RPC route | Orchestration | Published |
| 62 | [CVE-2026-60087](https://www.vulncheck.com/advisories/praisonai-before-tool-approval-cache-bypass) | PraisonAI | Tool approval caching bypass across parameter changes | AI Security | Published |
| 63 | [CVE-2026-62164](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-29r9-67vg-qj56) | PraisonAI | HITL approval cached by tool name and reused across distinct arguments | AI Security | CVE Assigned |
| 64 | [CVE-2026-62171](https://github.com/MervinPraison/PraisonAI/security/advisories/GHSA-4r3p-w3mc-5v34) | PraisonAI | Prompt-injection defense requires three detector families simultaneously | AI Security | CVE Assigned |
| 65 | [CVE-2026-21401](https://snailsploit.com/cves) | OpenClaw | Environment variable override allowlist bypass → RCE | Agent Framework | Published |
| 66 | [CVE-2026-28912](https://snailsploit.com/cves) | LangChain | Unsafe deserialization in persistent agent state loader | AI Framework | Published |
| 67 | [CVE-2026-31044](https://snailsploit.com/cves) | LlamaIndex | Local file disclosure via malicious template rendering | AI Framework | Published |
| 68 | [CVE-2026-34190](https://snailsploit.com/cves) | AutoGen | Unauthenticated RPC agent state execution | Agent Framework | Published |
| 69 | [CVE-2026-38201](https://snailsploit.com/cves) | CrewAI | Tool output indirect prompt injection leading to local file exfiltration | Agent Framework | Published |
| 70 | [CVE-2026-41092](https://snailsploit.com/cves) | Ollama WebUI | SSRF via remote model pull API endpoint | AI Platform | Published |
| 71 | [CVE-2026-43901](https://snailsploit.com/cves) | AnythingLLM | Path traversal in multi-tenant document parser pipeline | AI Platform | Published |
| 72 | [CVE-2026-45120](https://snailsploit.com/cves) | LocalAI | Command injection in audio processing extension handler | AI Platform | Published |
| 73 | [CVE-2026-47802](https://snailsploit.com/cves) | FastChat | Arbitrary file write via worker registration protocol | AI Framework | Published |
| 74 | [CVE-2026-50119](https://snailsploit.com/cves) | Flowise | Unauthenticated workflow execution via missing API key verification | Low-Code AI | Published |
| 75 | [CVE-2026-52310](https://snailsploit.com/cves) | LangFlow | RCE via sandbox bypass in Custom Python Function node | Low-Code AI | Published |
| 76 | [CVE-2026-54801](https://snailsploit.com/cves) | Haystack | Directory traversal in document store file indexer | AI Orchestration | Published |
| 77 | [CVE-2026-56902](https://snailsploit.com/cves) | Semantic Kernel | Unescaped prompt template variable injection | AI Framework | Published |
| 78 | [CVE-2026-59104](https://snailsploit.com/cves) | Guidance | Remote code execution via unsafe template evaluation | AI Tooling | Published |
| 79 | [CVE-2026-61201](https://snailsploit.com/cves) | Outlines | Regex state-machine exhaustion Denial of Service | AI Security | Published |
| 80 | [CVE-2026-63412](https://snailsploit.com/cves) | Text Generation WebUI | Stored XSS via raw Markdown chat history export | AI Platform | Published |
| 81 | [CVE-2026-65109](https://snailsploit.com/cves) | LM Studio | Local API CORS wildcard authorization bypass | AI Tooling | Published |
| 82 | [CVE-2026-67801](https://snailsploit.com/cves) | Jan AI | Arbitrary binary execution via untrusted extension loader | AI Desktop | Published |
| 83 | [CVE-2026-69110](https://snailsploit.com/cves) | Open WebUI | IDOR in session context memory persistence layer | AI Interface | Published |
| 84 | [CVE-2026-71204](https://snailsploit.com/cves) | Dify | Server-Side Template Injection (SSTI) in custom tools handler | Agent Orchestration | Published |
| 85 | [CVE-2026-73901](https://snailsploit.com/cves) | Coze SDK | HMAC signature spoofing via null key acceptance | Agent Platform | Published |
| 86 | [CVE-2026-75122](https://snailsploit.com/cves) | TaskingAI | Privilege escalation in multi-tenant team workspaces | Agent Platform | Published |
| 87 | [CVE-2026-78105](https://snailsploit.com/cves) | VectorAdmin | Unauthenticated collection deletion via exposed debug handler | Vector Infra | Published |
| 88 | [CVE-2026-80211](https://snailsploit.com/cves) | ChromaDB | Path traversal in collection local storage initialization | Vector DB | Published |
| 89 | [CVE-2026-82904](https://snailsploit.com/cves) | Qdrant WebUI | Reflected XSS in snapshot recovery dashboard | Vector DB | Published |
| 90 | [CVE-2026-84110](https://snailsploit.com/cves) | Milvus | Unauthenticated gRPC memory consumption Denial of Service | Vector DB | Published |
| 91 | [CVE-2026-87102](https://snailsploit.com/cves) | Weaviate | GraphQL query recursion stack overflow Denial of Service | Vector DB | Published |
| 92 | [CVE-2026-89001](https://snailsploit.com/cves) | PGVector Extensions | SQL injection via unescaped cosine distance vector input | Vector DB | Published |

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


**sources of record:** [Wordfence](https://www.wordfence.com/threat-intel/vulnerabilities/researchers/kai-aizen) · [GHSA Credit](https://github.com/advisories?query=credit%3ASnailSploit) · [GitHub](https://github.com/SnailSploit) · [lore.kernel.org](https://lore.kernel.org/all/?q=Kai+Aizen)

---

[![snailsploit](https://img.shields.io/badge/read_the_research-snailsploit.com-E07A4A?style=flat-square&labelColor=0E0E0F)](https://snailsploit.com)

`same attack. different substrate.`
