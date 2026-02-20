<div align="center">

# SnailSploit

**GenAI Security Researcher · AI Red Teamer · Offensive Security Writer**

*Social engineering and prompt injection are the same attack. Different substrate.*

[![Website](https://img.shields.io/badge/snailsploit.com-000?style=for-the-badge&logo=astro&logoColor=white)](https://snailsploit.com)
[![The Jailbreak Chef](https://img.shields.io/badge/The_Jailbreak_Chef-FF6B35?style=for-the-badge&logo=fireship&logoColor=white)](https://thejailbreakchef.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/kaiaizen)

</div>

---

## About

I'm Kai Aizen — an independent GenAI security researcher exploring **inherited vulnerabilities**: the observation that LLMs exhibit the same trust reflexes as humans because they learned from human-generated data. Authority, reciprocity, social proof, urgency — the psychological levers that social engineers have exploited for decades — appear to function similarly in AI systems.

This principle shapes everything I build.

`Creator of AATMF · Author of Adversarial Minds · NVD Contributor · Offensive Security Writer @ Hakin9`

---

## Frameworks & Research

| Project | Description |
|---------|-------------|
| [**AATMF**](https://github.com/SnailSploit/AATMF-Adversarial-AI-Threat-Modeling-Framework) | Adversarial AI Threat Modeling Framework — 15 tactics, 240 techniques, 2,152+ attack procedures. Maps to OWASP LLM Top-10, NIST AI RMF, MITRE ATLAS. |
| [**LLM Red Teamer's Playbook**](https://github.com/SnailSploit/The-LLM-Red-Teamer-s-Playbook) | Diagnostic methodology for bypassing LLM defense layers — input filters → alignment → identity → output → agentic trust. Maps to AATMF v3. |
## Experiments & PoCs
| Project | Description |
|---|---|
| [**ChatGPT-DNS-Exfill**](https://github.com/SnailSploit/ChatGPT-DNS-Exfill) | DNS exfiltration via ChatGPT Canvas — rendered content triggers DNS lookups without HTTP requests. |
| [**chatgpt-rce-dns**](https://github.com/SnailSploit/chatgpt-rce-dns) | Validating DNS exfiltration and Python Pickle RCE attack chains in AI code execution sandboxes. |

## Offensive Tools

| Tool | Description |
|------|-------------|
| [**KubeRoast**](https://github.com/SnailSploit/KubeRoast_v1) | Red-team Kubernetes misconfiguration & attack-path scanner. Built from scratch for real-world escalation paths. |
| [**Xposure**](https://github.com/SnailSploit/Xposure) | Credential intelligence platform for attack surface reconnaissance and exposed secret detection. |
| [**SnailHunter**](https://github.com/SnailSploit/SnailHunter) | AI-powered bug bounty automation platform combining LLM analysis with traditional security scanning. |
| [**Burp MCP Toolkit**](https://github.com/SnailSploit/Burp-MCP-Security-Analysis-Toolkit) | MCP security analysis toolkit for Burp Suite — test Model Context Protocol servers for prompt injection and tool poisoning. |
| [**SnailSploit Recon**](https://github.com/SnailSploit/SnailSploit_Recon_extension) | Chrome MV3 extension for passive reconnaissance and bug bounty recon automation. |

## Vulnerability Disclosures (NVD)

| CVE | Target | Type |
|-----|--------|------|
| [CVE-2026-1208](https://github.com/SnailSploit/CVE-2026-1208) | Welcart (WordPress) | CSRF to Settings Update |
| [CVE-2025-12163](https://github.com/SnailSploit/CVE-2025-12163) | Flavor WordPress Plugin | Stored Cross-Site Scripting |
| [CVE-2025-12030](https://github.com/SnailSploit/CVE-2025-12030) | ACF to REST API (WordPress) | Insecure Direct Object Reference |
| [CVE-2025-11171](https://nvd.nist.gov/vuln/detail/CVE-2025-11171) | WordPress Plugin | Authentication Bypass |
| [CVE-2025-9776](https://nvd.nist.gov/vuln/detail/CVE-2025-9776) | WordPress Plugin | Access Control Vulnerability |

## Publications

- **Adversarial Minds: The Anatomy of Social Engineering and the Psychology of Manipulation** — Book
- **Hakin9 Magazine** — Contributing author on AI security and adversarial research
- **OWASP GenAI Security Project** — AATMF accepted into 2026 roadmap

---

<div align="center">

*Built on the principle that the vulnerabilities we find in AI are the ones we inherited from ourselves.*

</div>
