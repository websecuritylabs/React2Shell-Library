# React2Shell Library

[![Awesome](https://awesome.re/badge.svg)]
![Web Security](https://img.shields.io/badge/topic-web%20security-brightgreen)
[![CVE-2025-55182](https://img.shields.io/badge/CVE-2025--55182-Critical-red)](https://nvd.nist.gov/vuln/detail/CVE-2025-55182)
![Resources](https://img.shields.io/badge/resources-updated%20regularly-blue)
![Community](https://img.shields.io/badge/community-welcome-orange)


A curated list of resources regarding **CVE-2025-55182**, the critical Remote Code Execution (RCE) vulnerability in React Server Components known as **"React2Shell"**.

> **Objective:** To document the history, mechanics, and remediation of the React2Shell vulnerability for researchers and security engineers.

## 📚 Library Contents

- [Core Intelligence](#core-intelligence)
- [Research & Analysis](#research--analysis)
- [Detection & Defense](#detection--defense)
- [Community & Discussion](#community--discussion)
- [Exploitation](#exploitation)
- [Media & Threat Intel](#media--threat-intel)

---

## Core Intelligence

*Official documentation and severity scoring.*

- [NVD - CVE-2025-55182 Detail](https://nvd.nist.gov/vuln/detail/CVE-2025-55182) - The official Common Vulnerability Scoring System (CVSS 10.0) entry and affected versions.
- [GitHub Security Advisory GHSA-fv66-9v8q-g76r](https://github.com/advisories/GHSA-fv66-9v8q-g76r) - Details the vulnerable packages: `react-server-dom-webpack`, `parcel`, and `turbopack`.
- [Next.js Security Advisory (CVE-2025-66478)](https://nextjs.org/blog/CVE-2025-66478) - Advisory tracking the downstream impact on Next.js applications using the App Router.

## Research & Analysis

*Technical deep dives into the root cause, exploitation chains, and the "Flight" protocol.*

- [React2Shell: Critical React Vulnerability](https://www.wiz.io/blog/critical-vulnerability-in-react-cve-2025-55182) - Deep technical analysis by **Wiz Research** on the unsafe deserialization flaw.
- [RCE via Flight Payload Deserialization](https://www.offsec.com/blog/cve-2025-55182/) - In-depth post from **Offensive Security** explaining the attack using Chunk objects and promise resolution.
- [CVE-2025-55182 (React2Shell): Remote code execution in React Server Components](https://securitylabs.datadoghq.com/articles/cve-2025-55182-react2shell-remote-code-execution-react-server-components/) - **Datadog Security Labs** analysis, including observed PoC injection parameters.

## Detection & Defense

*Rules, scripts, and WAF configurations to protect infrastructure.*

- [GitHub - Vercel Labs / fix-react2shell-next](https://github.com/vercel-labs/fix-react2shell-next) - Official Codemod by **Vercel** to automatically detect and patch vulnerable Next.js applications.
- [Cloudflare WAF proactively protects against React vulnerability](https://blog.cloudflare.com/waf-rules-react-vulnerability/) - All **Cloudflare** customers are automatically protected, including those on free and paid plans, as long as their React application traffic is proxied through the Cloudflare Web Application Firewall (WAF).
- [Responding to CVE-2025-55182](https://cloud.google.com/blog/products/identity-security/responding-to-cve-2025-55182) - Guidance from **Google Cloud** on using Cloud Armor `cve-canary` WAF rules.
- [Fastly's Proactive Protection](https://www.fastly.com/blog/fastlys-proactive-protection-critical-react-rce-cve-2025-55182) - Details on **Fastly's** WAF signals and virtual patching to gain time for patching.


## Community & Discussion

*Real-time analysis, threads, and commentary from the security community.*

- [@maple3142 (Dec 4, 2025)](https://x.com/maple3142/status/1996687157789155647) - *Release of the first working Proof of Concept (PoC) for Next.js 16.0.6, confirming the vulnerability was exploitable.*


## Exploitation

*Proof of Concepts (PoC).*

- [Vulhub - Docker Environment](https://github.com/vulhub/vulhub/tree/master/react/CVE-2025-55182) - Pre-built Docker container to safely reproduce the vulnerability locally.
- [Github - CVE-2025-55182-research Exploit research](https://github.com/ejpir/CVE-2025-55182-research) - PoC for CVE-2025-55182.
- [Github - Assetnote/react2shell-scanner](https://github.com/assetnote/react2shell-scanner) - High-fidelity detection script for confidently confirming vulnerability without full exploitation.
- [Github - CVE-2025-55182 PoC by maple3142](https://gist.github.com/maple3142/48bc9393f45e068cf8c90ab865c0f5f3) - PoC for CVE-2025-55182 that works on Next.js 16.0.6.
- [Github] - PoCs for CVE-2025-55182 by lachlan2k](https://github.com/lachlan2k/React2Shell-CVE-2025-55182-original-poc) - Original Proof-of-Concept's for React2Shell CVE-2025-55182
- [Github] - CVE-2025-55182-advanced-scanner by zack0x01](https://github.com/zack0x01/CVE-2025-55182-advanced-scanner-) - Simple command-line tool for detecting and exploiting CVE-2025-55182 (React Server Components RCE) in Next.js applications.


## Media & Threat Intel

*Active threat actor reporting and wider industry coverage.*

- [China-nexus cyber threat groups rapidly exploit React2Shell](https://aws.amazon.com/blogs/security/china-nexus-cyber-threat-groups-rapidly-exploit-react2shell-vulnerability-cve-2025-55182/) - **AWS Security Blog** report on exploitation by groups like Earth Lamia and Jackpot Panda.

---

## Contributing

This library is community-maintained. Please read [CONTRIBUTING.md](CONTRIBUTING.md) to add a resource.
