# Awesome-Intelligent-Threat-Detection

# Top Intelligent Threat Detection Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Cloud Threat Detection, Attack Path Analysis & Self-Hosted Security Analytics*  
**Last updated: October 2026**

This repository tracks notable **commercial intelligent threat detection platforms** and **open-source projects** that identify, prioritize, and respond to security threats across cloud infrastructure — from agentless posture scanning to runtime workload protection and attack path analysis.

**Examples** include Amazon GuardDuty, Microsoft Defender for Cloud, Google Cloud Security Command Center, Palo Alto Prisma Cloud, Datadog Cloud Security, Wiz, Orca Security, Lacework, CrowdStrike Falcon Cloud Security, and Sophos Cloud Optix (the category leaders).

**Open-source emphasis**: Intelligent threat detection is a strong open-source domain. **Prowler** leads with 300+ CIS and NIST checks across AWS, Azure, and GCP, serving as the de facto open-source CSPM scanner . **Steampipe** enables SQL-based cross-cloud querying for security posture assessment . **Kubescape** reached 4.0 with GA runtime threat detection using CEL-based rules and native AI agent integration . **Dredge** delivers multi-region CloudTrail hunting with attack path correlation . **Argus** provides MITRE ATT&CK attack chain correlation with forensic chain-of-custody . **Nexus Fleet** combines Wazuh-style detection with developer-aware web stack monitoring . **XCLOAK** offers an all-in-one SOC stack with 15+ detection modules . This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[Wiz](https://www.wiz.io/)**  
  **The leading CNAPP platform with graph-based attack path analysis** — agentless SideScanning™ technology scans cloud workloads without deploying agents . **Gartner Magic Quadrant CNAPP Leader 2024** with modern UX and contextual risk graph . **Google acquisition announced July 2025 for $32B** — the largest cybersecurity acquisition in history, pending finalization . **Pricing**: €80-300K/year for mid-to-large enterprises (500-1000 cloud resources) . **Best for multi-cloud organizations seeking modern UX and attack path context** .

- **[Palo Alto Prisma Cloud](https://www.paloaltonetworks.com/prisma/cloud)**  
  **The broadest coverage CNAPP platform** — built through acquisitions of Twistlock (containers), RedLock (CSPM), and Bridgecrew (IaC) . **Comprehensive multi-cloud security posture, workload protection, and compliance** . **Pricing**: €100-400K/year — highest in category due to complexity . **Best for large enterprises already aligned with Palo Alto ecosystem** .

- **[Microsoft Defender for Cloud](https://azure.microsoft.com/en-us/products/defender-for-cloud/)**  
  **Microsoft's cloud-native security platform** — free foundational CSPM with Defender CSPM and Defender for Servers paid plans . **Defender CSPM** adds agentless vulnerability scanning, attack path analysis, and cloud security explorer . **Defender for Servers Plan 2** includes agentless malware scanning and endpoint protection . **Pricing**: ~$15/server/month for Plan 2; €30-100K/year for typical enterprises . **Best for Microsoft-centric organizations already using Azure and M365 E5** .

- **[Orca Security](https://orca.security/)**  
  **Agentless CNAPP with SideScanning™ technology** — direct competitor to Wiz with strong technical quality . **Pricing**: €80-250K/year . **Best for mid-market and enterprises wanting agentless scanning** .

- **[CrowdStrike Falcon Cloud Security](https://www.crowdstrike.com/products/cloud-security/)**  
  **Cloud security integrated with CrowdStrike's EDR platform** — combines CNAPP with endpoint detection . **Pricing**: €80-250K/year . **Best for organizations already using CrowdStrike Falcon** .

- **[Amazon GuardDuty](https://aws.amazon.com/guardduty/)**  
  **AWS's managed threat detection service** — continuous monitoring for malicious activity and unauthorized behavior . **GuardDuty finding types include UnauthorizedAccess:EC2/SSHBruteForce, CryptoCurrency:EC2/BitcoinTool.B, and Recon:EC2/Portscan** . **Best for AWS-native threat detection** .

- **[Google Cloud Security Command Center](https://cloud.google.com/security-command-center)**  
  **Google's security and risk management platform** — unified visibility into cloud assets with threat detection . **SCC findings and notification workflows** for Google Cloud environments . **Best for GCP-native security** .

- **[Datadog Cloud Security](https://www.datadoghq.com/)**  
  **Cloud security integrated with Datadog observability** — threat detection, posture management, and workload protection . **Best for Datadog users wanting unified observability and security** .

- **[Lacework](https://www.lacework.com/)**  
  **Cloud security with behavioral analytics** — ML-based anomaly detection (acquired by Fortinet June 2024) . **Pricing**: €80-300K/year . **Best for organizations wanting behavioral threat detection** .

- **[Sophos Cloud Optix](https://www.sophos.com/)**  
  **Cloud security posture management** — agentless scanning and threat detection for AWS, Azure, and GCP . **Best for Sophos ecosystem users** .

## Open-Source GitHub Projects

### Cloud Security Posture Management (CSPM)

- **[Prowler](https://github.com/prowler-cloud/prowler)**  
  **The leading open-source CSPM scanner with 300+ checks**, Apache-2.0 licensed . **Covers AWS, Azure, and GCP against CIS Benchmarks and NIST standards** . **Fast CLI with CI/CD integration** — Prowler Pro adds commercial support since 2023 . **Open-source combination of Prowler + Steampipe covers 70-80% of basic CSPM needs for free** . **Best for organizations starting cloud security assessments** .

- **[Steampipe](https://github.com/turbot/steampipe)**  
  **Zero-ETL cloud API querying with SQL**, AGPL-3.0 licensed . **Query cloud resources like a database** — cross-cloud multi-provider SQL queries . **Rich plugin framework for AWS, Azure, GCP, and more** . **Powers custom security dashboards and compliance queries** . **Best for SQL-based cloud security analysis** .

- **[ScoutSuite](https://github.com/nccgroup/ScoutSuite)**  
  **Multi-cloud security auditing tool from NCC Group**, GPL-2.0 licensed . **Audits AWS, Azure, GCP, Alibaba Cloud, and Oracle Cloud** . **HTML report output with security findings** . **Best for multi-cloud security audits** .

- **[CloudQuery](https://github.com/cloudquery/cloudquery)**  
  **Open-source cloud asset inventory**, MPL-2.0 licensed . **Extracts, transforms, and loads cloud configuration** across accounts . **SQL-queryable inventory** for security analysis . **Best for multi-cloud asset visibility** .

- **[CloudSploit](https://github.com/aquasecurity/cloudsploit)**  
  **Cloud security scanner (acquired by Aqua Security)**, GPL-3.0 licensed . **Detects cloud misconfiguration alerts** . **Continues open-source development** . **Best for cloud misconfiguration detection** .

### Kubernetes & Container Threat Detection

- **[Kubescape](https://github.com/kubescape/kubescape)**  
  **The leading open-source Kubernetes security platform with GA runtime threat detection in 4.0**, Apache-2.0 licensed . **CEL-based detection rules with direct access to Application Profiles** (security baselines for workloads) . **Monitors system interactions (processes, capabilities, syscalls), connectivity (network/HTTP events), and storage (file system activities)** . **Rules and RuleBindings managed as Kubernetes CRDs** — export alerts to AlertManager, SIEM, Syslog, or HTTP webhooks . **Kubescape Storage uses Kubernetes Aggregated API** for SBOMs and vulnerability manifests at scale . **KAgent-native plug-in** enables AI assistants to analyze security posture and pull remediation guidance . **Best for Kubernetes-native runtime threat detection** .

- **[node-agent (Kubescape)](https://github.com/kubescape/node-agent)**  
  **Runtime threat detection agent for Kubernetes nodes**, Apache-2.0 licensed . **Uses eBPF-based image gadgets from Inspektor Gadget** for process execution, file operations, network connections, DNS queries, and syscall monitoring . **Detection rules defined as CEL expressions** in Kubernetes CRDs . **Built-in rule categories**: process rules (unexpected executables, shell spawning), file rules (sensitive file access), network rules (unexpected connections, DNS tunneling, data exfiltration), privilege rules (capability usage, privilege escalation), crypto rules (RandomX mining detection), and container rules (escape attempts, namespace manipulation) . **Feature toggles for application profiling, malware detection (ClamAV), SBOM generation, file integrity monitoring, and seccomp profiles** . **Best for Kubernetes node-level threat detection** .

### Cloud Forensics & Incident Response

- **[Dredge](https://pypi.org/project/dredge-ir/)**  
  **Cloud incident-response and threat-hunting toolkit for AWS, Kubernetes, GitHub, and GCP**, open-source . **Multi-region CloudTrail hunting** — queries all enabled AWS regions concurrently and merges results into a single time-sorted timeline, addressing the regional API blind spot attackers exploit . **Full hunt capabilities**: CloudTrail live + offline + all-region fan-out, GuardDuty, Security Hub, Config . **Containment actions**: IAM, EC2, RDS, ECS, S3, Lambda, KMS . **Forensics**: S3 log collection, snapshots, flow logs . **Kubernetes support** for hunt, containment (RBAC, pods, nodes, NetworkPolicy), and forensics . **GitHub audit-log hunting** for org/enterprise . **Best for multi-region cloud forensics and incident response** .

- **[Argus](https://github.com/nssriraam/argus)**  
  **Open-source AWS & Azure cloud forensics and threat detection platform**, open-source . **MITRE ATT&CK attack chain correlation** with live dashboard and automated PDF reports . **Zero infrastructure cost** — Python CLI with interactive shell . **Chain of custody** — case lifecycle states (OPEN → INVESTIGATING → CLOSED → ARCHIVED) with analyst attribution and timestamped notes . **Hardened architecture**: parameterized SQL queries prevent injection, deterministic cryptographic hashing prevents collisions . **Evidence store**: no UPDATE/DELETE on raw event data, per-case partitioned datasets, audit trail with `ingested_at` timestamps, and `verify` command for record count and hash validation . **Detection rules**: credential access (T1552, T1078), defense evasion (T1562), and Azure-specific detections . **Best for cloud forensic investigations with audit trails** .

### All-in-One SOC Platforms

- **[XCLOAK Security Suite](https://github.com/The-Abhishek1/XCLOAK-SECURITY-SUITE)**  
  **Open-source enterprise SOC platform combining SIEM, SOAR, EDR, DPI, MDM, and NGFW in one stack**, open-source . **Self-host in minutes** . **15+ detection modules** including DNS security (multi-factor DGA scoring, DNS tunneling), TLS anomaly (weak ciphers, deprecated TLS, SNI/host domain fronting), HTTP inspection (35+ malicious UA signatures, webshell paths), protocol anomaly, port scan/lateral movement, exfiltration, TLS/JA3 fingerprinting (10 known C2/malware profiles including Cobalt Strike, Metasploit, TrickBot, Emotet), credential attacks, privilege escalation, ransomware detection (FIM mass-modify + crypto extensions), LotL (Office→PowerShell chains, 8 LOLBins), impossible travel (Haversine >900 km/h), and UEBA behavioral baselining . **Enterprise firewall** with direction-aware rules, port ranges, tags, expiry, and per-tenant policy . **Go agent** for autonomous collection across Linux and Windows with eBPF TCP events . **Best for comprehensive self-hosted SOC** .

- **[Nexus Fleet](https://pypi.org/project/nexus-fleet/)**  
  **Offline-first security platform combining Wazuh-style detection with developer-aware monitoring**, open-source . **Telemetry never leaves your LAN** — ideal for compliance and on-prem . **Wazuh model** (FIM, log monitoring, SCA, vulnerability detection, active response) plus **developer-aware detections** for Laravel, Next.js, Nginx that traditional SIEMs miss . **15 detection domains** including SIEM (NQL query language), XDR (kill-chain correlation), EDR (process tree lineage), UEBA (behavioral baselines), SOAR (playbooks), Threat Intel (IOC store + feed import), NDR (beaconing/C2 detection), Cloud (CSPM with Prowler import), and AI (local Naive-Bayes triage) . **Every alert carries severity 0-15, MITRE technique, and remediation step** . **Posture score 0-100** for network, server, and website . **Pure-Python agent** (stdlib only) for any host with Python 3.8+ . **Best for offline-first compliance environments** .

### Additional Strong Open-Source Options

- **Magpie** — CSPM focused on cloud ransomware and supply chain attacks, Apache-2.0 licensed (188 GitHub stars) .
- **Kube-bench** — Kubernetes CIS Benchmark checks .
- **Trivy** — Container and IaC vulnerability scanner .
- **Checkov** — IaC security scanning for Terraform, CloudFormation, and Kubernetes .
- **tfsec** — Terraform security scanner .
- **Cartography** — Graph-based cloud infrastructure security analysis .
- **RITA** — Real Intelligence Threat Analytics for C2 detection through network traffic analysis .
- **Malcolm** — Network traffic analysis suite for full packet capture, Zeek logs, and Suricata alerts .
- **Wazuh** — Open-source SIEM and XDR with FIM, log monitoring, and vulnerability detection .
- **UTMStack** — Customizable SIEM and XDR with real-time correlation and threat intelligence (220 GitHub stars) .

**Frameworks for building custom intelligent threat detection solutions**: Combine **Prowler** for CSPM scanning across AWS, Azure, and GCP . Use **Kubescape** for Kubernetes runtime threat detection with CEL-based rules and AI agent integration . Deploy **Dredge** for multi-region CloudTrail hunting and cloud forensics . Integrate **Argus** for MITRE ATT&CK attack chain correlation with chain-of-custody audit trails . Choose **XCLOAK** for an all-in-one SOC stack with 15+ detection modules . Use **Nexus Fleet** for offline-first detection with developer-aware monitoring . Integrate **Steampipe** for SQL-based cross-cloud security queries . Note that true enterprise CNAPP with graph-based attack path analysis, agentless scanning, and executive UI (Wiz, Prisma Cloud, Orca) remains primarily commercial territory; open-source stacks provide strong CSPM scanning, runtime detection, and forensic investigation foundations that require integration for complete intelligent threat detection.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Intelligent threat detection platforms handle sensitive security telemetry and may access cloud infrastructure. Self-hosted solutions require proper security hardening, access controls, and compliance with data privacy regulations.
- **Open-source CSPM covers 70-80% of basic needs** — Prowler + Steampipe combination is often sufficient for PME/ETI under 500 cloud resources . Commercial CNAPP (Wiz, Prisma Cloud) justifies cost for >500 resources with dedicated security teams, providing attack path context and executive UI .
- **Google's acquisition of Wiz for $32B** (announced July 2025) represents the largest cybersecurity acquisition in history and will reshape the CNAPP market .
- **License considerations**: Prowler uses Apache-2.0, Steampipe uses AGPL-3.0, Kubescape uses Apache-2.0, Argus is open-source, XCLOAK is open-source, and Nexus Fleet is open-source . Verify licensing against your use case before committing.
- The open-source ecosystem provides strong CSPM scanning, runtime detection, and forensic investigation foundations, but **graph-based attack path analysis, agentless scanning, and executive UI** remain primarily commercial offerings.

---

**Made for security engineers, cloud architects, and organizations seeking intelligent threat detection sovereignty.**  
Let's make intelligent threat detection more open, transparent, and effective.
