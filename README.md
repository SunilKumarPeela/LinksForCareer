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
