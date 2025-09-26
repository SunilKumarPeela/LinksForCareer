# 📚 The Mozilla Developer Network (MDN)

The **Mozilla Developer Network (MDN)** is a trusted, open-source resource for web developers, offering comprehensive documentation and examples for technologies like HTML, CSS, JavaScript, and more. Originally created for browser documentation, MDN has evolved into the central hub for web standards and best practices, supported by major companies such as Microsoft and Google. It is an invaluable reference for learning syntax, exploring code examples, and understanding core concepts—helping developers build cleaner, more efficient applications. Whether you’re troubleshooting, learning new features, or enhancing your skills

## 🔗 Useful Link
- [Visit MDN Documentation](https://developer.mozilla.org/)
---

# 🔒 The Common Criteria (CC)

The **Common Criteria (CC)** is an international standard for evaluating the security of IT products and systems, first developed in 1994. It provides a structured framework for assessing whether a product meets specific security requirements. While most modern software does not undergo a formal CC evaluation—because the process can be expensive and time-consuming—teams can still benefit from its guidance to design stronger security requirements.

## 🧭 What’s Inside
- **Part 1** – Introduction & framework overview  
- **Part 2** – Security Functional Requirements (SFRs): a catalog of *“security functions you might require.”*  
- **Part 3** – Assurance Requirements (SARs): criteria for confidence that controls are correctly designed and implemented

> 💡 **Tip:** If you suspect your system needs special security requirements and aren’t sure where to start, browse **Part 2** for ideas. Some terminology is arcane, but there’s a glossary to help.

## 🔗 Useful Link
- [Visit Common Criteria Portal](https://www.commoncriteriaportal.org/index.cfm)
---

# 🐞 NIST National Vulnerability Database (NVD)

The **NIST National Vulnerability Database (NVD)** is the U.S. government’s public repository of standardized vulnerability information. It builds on the CVE® list by adding analysis and metadata—such as severity scoring, affected products, and weakness classifications—to help teams assess risk and prioritize remediation. Even if you track advisories elsewhere, NVD is a central, authoritative reference for vulnerability research and reporting.

## 🧭 What’s Inside
- **CVE Records** – Standardized entries for publicly disclosed vulnerabilities
- **CVSS Metrics** – Severity scores with vector details for impact/exploitability analysis
- **CWE Mapping** – Underlying weakness classifications to guide secure fixes
- **CPE Matching** – Structured identifiers for affected vendors/products/versions
- **References & Patches** – Links to advisories, exploits, and remediation guidance
- **Feeds & API** – JSON data feeds and endpoints for automation and dashboards

> 💡 **Tip:** Start with a **CVE ID**, review the **CVSS vector** to understand risk, then use **CPE** filters to verify whether your exact product/version is affected. Map to **CWE** to inform secure coding and long-term mitigations.

## 🔗 Useful Link
- [Visit NIST NVD](https://nvd.nist.gov/)
---

# 🛡️ OWASP Top Ten (Web Application Security Risks)

The **OWASP Top Ten** is a community-driven, industry-recognized awareness document that highlights the most critical security risks to web applications. Updated periodically, it synthesizes real-world data from industry sources to help teams prioritize defenses, guide secure development, and structure AppSec programs. Even if you follow other standards, the Top Ten is a practical starting point for risk-based training, threat modeling, and control selection.

## 🧭 What’s Inside
- **Top Ten Risk Categories** – The current list of high-impact web app risks with descriptions, examples, and mitigations
- **Data & Methodology** – How categories are selected from industry incident data and expert input
- **Mappings** – Links to **CWE**, **ASVS**, and related OWASP resources for deeper technical alignment
- **Guidance & Mitigations** – Practical prevention strategies, verification steps, and references
- **Training Aids** – Cheat sheets, labs, and project resources for developer education
- **Downloads & Artifacts** – PDFs, translations, and companion materials for teams

> 💡 **Tip:** Use the Top Ten to seed your **SSDL/SDLC** requirements, align findings to **CWE** for root-cause analysis, and verify controls against **OWASP ASVS** to move from awareness to measurable assurance.

## 🔗 Useful Link
- [Visit OWASP Top Ten](https://owasp.org/www-project-top-ten/)

---
# 🧩 MITRE CWE Top 25 (Most Dangerous Software Weaknesses)

The **MITRE CWE Top 25** is an annually updated, data-driven ranking of the most prevalent and impactful software weaknesses. Derived from real-world vulnerability data (e.g., CVEs analyzed via NVD), it helps teams prioritize secure coding practices, focus code reviews, tune SAST/DAST rules, and guide developer training. Even if you follow other frameworks, the Top 25 is a practical, high-signal list to reduce the most common root causes of vulnerabilities.

## 🧭 What’s Inside
- **Ranked Weakness List** – The current Top 25 CWEs with descriptions, consequences, and examples
- **Methodology** – How incidence and severity are combined to compute scores and rankings
- **Mappings** – Cross-references to **CVE**, related **CWE** entries, and attack patterns (**CAPEC**)
- **Mitigations & Detection** – Recommended coding practices, test ideas, and review guidance
- **Historical Lists** – Prior years’ rankings for trend analysis and program benchmarking
- **Downloads & Assets** – Pages, data tables, and references for automation or reporting

> 💡 **Tip:** Map your findings to CWE categories and align remediation sprints to the Top 25. Use it to seed **secure coding checklists**, calibrate **SAST rules**, and target **developer training** where it removes the most risk.

## 🔗 Useful Link
- [Visit CWE Top 25](https://cwe.mitre.org/top25/)
---
---

# 🧪 Application Security Testing

**Application Security Testing (AST)** is the practice of identifying, analyzing, and mitigating security weaknesses within software applications. It ensures vulnerabilities are detected early in the **Software Development Life Cycle (SDLC)** and prevents them from reaching production. AST includes approaches such as **Static Application Security Testing (SAST)**, **Dynamic Application Security Testing (DAST)**, and **Interactive Application Security Testing (IAST)**, along with modern practices like **secret scanning** and dependency analysis.

## 🧭 What’s Inside
- **SAST & DAST** – Detect vulnerabilities at code and runtime  
- **IAST & RASP** – Hybrid and runtime protection mechanisms  
- **Secret Scanning** – Prevent exposure of API keys, tokens, and credentials  
- **Dependency Checks** – Identify risks in third-party libraries  
- **CI/CD Integration** – Automate scans as part of DevSecOps pipelines  

> 💡 **Tip:** Introduce AST tools into your build pipeline to **“shift security left”**—catching issues earlier, reducing cost, and increasing developer awareness.

---

## 🕵️ Secret Scanning

**Secret scanning** is a vital AST practice that identifies exposed credentials such as API keys, tokens, and private certificates inside code repositories. Since these secrets can be exploited to gain unauthorized access, scanning prevents accidental leaks before they cause harm.

## 🔧 Useful Tools
- [**git-secrets**](https://github.com/awslabs/git-secrets) – AWS Labs tool that scans Git commits for secrets and blocks pushes if sensitive patterns (like AWS keys) are detected.  
- [**TruffleHog**](https://github.com/trufflesecurity/trufflehog) – Advanced scanner that searches commit history and file systems for high-entropy strings and credential patterns, uncovering secrets missed by simple regex checks.  

> 💡 **Tip:** Integrate tools like **git-secrets** and **TruffleHog** into your **CI/CD pipelines** to automatically block risky commits and alert teams for remediation.

---

---

# 🧑‍💻 Static Application Security Testing (SAST)

**Static Application Security Testing (SAST)** is a white-box testing method that analyzes source code, bytecode, or binaries to detect security vulnerabilities without executing the program. It is typically integrated early in the **Software Development Life Cycle (SDLC)**, allowing developers to catch issues before deployment. SAST tools scan codebases for insecure coding patterns, compliance violations, and potential flaws such as **SQL injection, XSS, hardcoded secrets, and buffer overflows**.

## 🧭 What’s Inside
- **Source Code Scanning** – Automated review of application code for vulnerabilities  
- **IDE Integration** – Feedback to developers as they code  
- **CI/CD Integration** – Automated scans during build pipelines  
- **Policy Enforcement** – Ensure compliance with standards like **OWASP ASVS**, **CWE**, and **NIST**  
- **Developer Enablement** – Early detection reduces remediation costs and improves secure coding skills  

> 💡 **Tip:** SAST is most effective when combined with **secret scanning** and **DAST** to cover both code and runtime vulnerabilities.

---

## 🔧 Useful Tools
- [**SonarQube**](https://www.sonarsource.com/products/sonarqube/) – Industry-standard platform for continuous code quality and security. It integrates with IDEs, CI/CD pipelines, and supports multiple programming languages with rulesets aligned to CWE and OWASP Top Ten.  
- [**CodeSweep**](https://marketplace.visualstudio.com/items?itemName=ContrastSecurity.codesweep) – A free Visual Studio Code extension by Contrast Security that provides real-time security feedback to developers, highlighting insecure coding patterns directly within the IDE.  

> 💡 **Tip:** Use **SonarQube** for enterprise-wide codebase scanning and governance, while **CodeSweep** is ideal for giving instant feedback to developers during coding.

---
---

# 📦 Software Composition Analysis (SCA)

**Software Composition Analysis (SCA)** is the process of identifying and managing open-source components, libraries, and dependencies within an application. Since modern software often relies heavily on third-party code, SCA ensures that vulnerabilities, outdated packages, and licensing risks are discovered and addressed. It helps teams prevent known exploits (like those in the **NVD CVE database**) from creeping into their applications.

## 🧭 What’s Inside
- **Dependency Scanning** – Detect vulnerable open-source components  
- **Version Management** – Identify outdated or insecure package versions  
- **License Compliance** – Ensure usage aligns with legal requirements (e.g., GPL, MIT, Apache)  
- **Integration** – Works with GitHub, GitLab, Jenkins, and other CI/CD pipelines  
- **Automation** – Automatically raise pull requests for fixes/upgrades  

> 💡 **Tip:** SCA should be combined with **SAST** and **DAST** to provide full coverage of custom code and third-party risks.

---

## 🔧 Useful Tools
- [**Dependabot**](https://github.com/dependabot) – A GitHub-native tool that scans repositories for outdated or vulnerable dependencies and automatically generates pull requests to update them. It integrates seamlessly with GitHub workflows, making dependency management proactive and automated.  
- [**OWASP Dependency-Check**](https://owasp.org/www-project-dependency-check/) – An open-source tool that identifies project dependencies and checks for known vulnerabilities (CVE entries). It supports multiple build systems (Maven, Gradle, npm, etc.) and can be integrated into CI/CD pipelines.  

> 💡 **Tip:** Use **Dependabot** for continuous dependency updates and **Dependency-Check** for in-depth vulnerability scanning across build systems.

---
---

# 🌐 Dynamic Application Security Testing (DAST)

**Dynamic Application Security Testing (DAST)** is a black-box testing method that analyzes a running application from the outside to identify security vulnerabilities. Unlike SAST, which inspects code, DAST simulates real-world attacks against the deployed app—without needing access to the source code. It is highly effective at finding runtime issues such as **SQL injection, XSS, authentication flaws, insecure redirects, and misconfigurations**.

## 🧭 What’s Inside
- **Runtime Testing** – Evaluates apps in execution rather than source code  
- **Vulnerability Simulation** – Mimics real-world attacker techniques  
- **Protocol & Input Testing** – Identifies weak validation and unsafe endpoints  
- **CI/CD Integration** – Automates scans against staging environments  
- **Compliance Support** – Helps meet standards like PCI-DSS, ISO 27001, and NIST  

> 💡 **Tip:** Combine **DAST** with **SAST** and **SCA** for full coverage of both runtime and code-level vulnerabilities.

---

## 🔧 Useful Tools
- [**OWASP ZAP (Zed Attack Proxy)**](https://www.zaproxy.org/) – A free, open-source DAST tool maintained by OWASP. It can scan web apps for vulnerabilities, automate regression scans, and includes an active community and CI/CD plugins.  
- [**Burp Suite**](https://portswigger.net/burp) – A widely used commercial and community DAST tool offering advanced penetration testing features like intercepting proxies, automated scanning, fuzzing, and vulnerability exploitation.  

> 💡 **Tip:** Use **OWASP ZAP** for open-source, community-driven testing and **Burp Suite** for more advanced manual + automated penetration testing.

---
---
---

# 🧩 Interactive Application Security Testing (IAST)

**Interactive Application Security Testing (IAST)** acts like a *security expert looking over the shoulder of your application while it’s running*. It combines the strengths of **SAST** (code-level analysis) and **DAST** (runtime testing) by monitoring applications from inside as they execute. IAST provides deep, real-time feedback during functional testing, making it highly accurate and developer-friendly.

## 🧭 What’s Inside
- **Runtime Monitoring** – Observes applications during normal execution  
- **Hybrid Approach** – Combines benefits of SAST and DAST  
- **Context-Aware Findings** – Pinpoints vulnerabilities with detailed traces  
- **CI/CD Integration** – Continuous scanning during development and QA  
- **Actionable Feedback** – Provides developers with real-time security insights  

> 💡 **Tip:** IAST is especially powerful in **QA/staging environments** where apps are exercised with real workloads.

---

## 🔧 Useful Tools
- [**Contrast Assess (IAST)**](https://www.contrastsecurity.com/contrast-assess) – An enterprise-grade IAST tool by Contrast Security that integrates into applications and provides continuous security analysis in real time.  
- [**Seeker**](https://www.synopsys.com/software-integrity/security-testing/interactive-application-security-testing.html) – A Synopsys IAST solution that provides runtime vulnerability detection, dataflow analysis, and actionable remediation guidance.  

---
---

# 📦 Container Scanning

**Container Scanning** identifies vulnerabilities in container images, ensuring that applications built on Docker or Kubernetes are secure. Since containers often rely on base images and third-party packages, scanning helps detect CVEs, misconfigurations, and outdated dependencies before deployment.

## 🧭 What’s Inside
- **Image Analysis** – Scan Docker/Kubernetes images for known vulnerabilities  
- **Registry Integration** – Connect with DockerHub, ECR, GCR, and others  
- **Policy Enforcement** – Block vulnerable images from production  
- **CI/CD Integration** – Automate scans during build and deployment  
- **Compliance Support** – Ensure images meet organizational and industry standards  

> 💡 **Tip:** Always scan both **base images** and **application layers** for vulnerabilities.

---

## 🔧 Useful Tools
- [**Anchore**](https://anchore.com/) – Open-source and enterprise solutions for container image scanning and compliance checks, with CI/CD pipeline integration.  
- [**Privy**](https://github.com/privy-io) – Lightweight container security tool that scans for secrets and vulnerabilities in container environments.  

---
---

# 🏗️ Infrastructure as Code (IaC) Scanning

**Infrastructure as Code (IaC) Scanning** detects vulnerabilities and misconfigurations in IaC templates like **Terraform, CloudFormation, ARM, and Kubernetes manifests**. By catching risks before provisioning, IaC scanning ensures cloud environments are secure by design.

## 🧭 What’s Inside
- **Template Analysis** – Scan IaC files for risky configurations  
- **Policy Enforcement** – Apply guardrails aligned with CIS benchmarks  
- **Multi-Cloud Support** – AWS, Azure, GCP templates and Kubernetes configs  
- **CI/CD Integration** – Prevent insecure code from being deployed  
- **Shift-Left Security** – Embed scanning in the developer workflow  

> 💡 **Tip:** Use IaC scanning before provisioning to avoid misconfigurations in live environments.

---

## 🔧 Useful Tools
- [**Checkov**](https://www.checkov.io/) – Open-source tool by Bridgecrew for scanning Terraform, Kubernetes, CloudFormation, and other IaC frameworks against security policies.  
- [**Terascan**](https://github.com/accurics/terrascan) – A popular IaC security scanner that supports multiple providers and enforces compliance with industry standards.  

---
---

# 🌍 Infrastructure Scanning

**Infrastructure Scanning** evaluates live infrastructure components such as servers, networks, and endpoints for vulnerabilities. It helps organizations discover misconfigurations, outdated software, open ports, and exploitable services in on-premises and cloud environments.

## 🧭 What’s Inside
- **Network Scanning** – Identify open ports, services, and misconfigurations  
- **Server Vulnerability Detection** – Find outdated or unpatched software  
- **Cloud & On-Prem Support** – Works across hybrid environments  
- **Compliance Support** – Aligns with PCI-DSS, HIPAA, and CIS benchmarks  
- **Continuous Monitoring** – Detects new risks as infrastructure evolves  

> 💡 **Tip:** Schedule recurring scans to maintain ongoing visibility into infrastructure risks.

---

## 🔧 Useful Tools
- [**Nessus**](https://www.tenable.com/products/nessus) – A widely used vulnerability scanner that assesses servers, networks, and applications for thousands of known issues.  
- [**Nikto**](https://cirt.net/Nikto2) – An open-source web server scanner that detects dangerous files, outdated server software, and common misconfigurations.  
- [**AWS Inspector**](https://aws.amazon.com/inspector/) – A cloud-native vulnerability management service that continuously scans AWS workloads and identifies risks.  

---

---
## Open Policy Agent (OPA)

A lightweight, general-purpose **policy engine** that lets you define, enforce, and manage policies across microservices, Kubernetes, and CI/CD using a unified policy language (Rego).  

🔗 [Official site & documentation](https://www.openpolicyagent.org)
---
