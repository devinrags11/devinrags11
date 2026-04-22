# 👋 Technical Auditor & GRC Analyst specializing in securing macOS environments against the NIST 800-171 framework using macOS_SCP & Jamf Compliance Editor. This profile showcases my "Sandbox-to-Production" methodology, increasing macOS security posture by 418% through shell automation and Jamf. 
Multi-Environment NIST 800-171 Validation Lab - Engineered a 4-Tier Audit Strategy: Validated macOS security controls across 
* UTM Virtualization
* APFS Volumes
* New User Accounts
* Actual Mac Production M4 hardware.
---

## 🚀 Project: NIST 800-171 Enterprise Hardening Lab
*Bridging the Gap: From Standalone Scripting to Managed Enterprise Policy*

### 📊 Performance Metrics
| Metric | Status | Result |
| :--- | :--- | :--- |
| **Initial Baseline** | 🔴 Critical | 7.38% Compliance |
| **Hardened State** | 🟢 Optimized | 38.26% (Standalone Max) |
| **Risk Coverage** | 🛡️ Managed | 100% via POA&M |

---

## 🛠️ Methodology: Sandbox-to-Production
1. **Discovery:** Conducted gap analysis using **mSCP** to establish the initial posture.
2. **Scaling:** Translated script logic into **Jamf Configuration Profiles** to prevent **Configuration Drift**.

---

## 🧠 Critical Thinking & Risk Management
I identified that **61%** of controls required enterprise infrastructure. I architected **Compensating Controls** to meet the security *intent*:

* **3.10.1 (Physical):** FileVault 2 + Firmware Passwords + 15-min Auto-Logout.
* **3.3.1 (Logging):** Encrypted cloud log-streaming to ensure audit trail immutability.
* **3.5.3 (MFA):** Hardware-Bound Biometrics (TouchID for Sudo) via Secure Enclave.

---

## 🗂️ Project Structure & Evidence Vault
*Each folder represents a specific phase of the NIST 800-171 compliance lifecycle.*

### 📁 01_Discovery_Baseline
`initial_scan.png` | `800-171.xls` | `800-171.yaml`

### 📁 02_Remediation_Sandbox
`800-171_compliance.sh` | `org.800-171.audit.plist`

### 📁 03_Enterprise_Production
`800-171.adoc` | `Last_Report.png`

### 📁 04_Audit_Documentation
`NIST_800-171_Master_Blueprint_Senior.pdf` | `NIST_800-171_POAM_Professional.pdf` | `Last_Scan.png` | `POAM.md`

---

## 🚀 Project recap: use the Jamf Compliance Editor to decide on the rules, and use mSCP to generate the files,

### macOS Security Compliance Project (mSCP)
* This is the "Engine" and the industry standard. It is the raw Python-based framework that generates the
scripts and profiles.
* Maximum Authority: This is the most "official" way to audit; it’s what government agencies
and major enterprises rely on.
* Total Customization: You can modify the .yaml files to add or remove specific controls that
don't apply to your business.
* Always Current: It is updated frequently by Apple and NIST engineers to match the latest
macOS releases (like Sonoma or Sequoia).

### Jamf Compliance Editor (JCE)
* This is the "Architect." It provides a graphical user interface (GUI) on top of the mSCP engine.
* You can see every NIST rule in a list with checkboxes. No coding is required to build the policy.
* Enterprise Integration: It is built specifically to export .mobileconfig files that plug directly
into Jamf Pro or other MDMs.
* Educational: It provides "Rationale" text for every rule, explaining why a setting is required.
* The app itself doesn't "run" the fix; it just builds the files. You still need a
way to get those files onto the Mac using mSCP project.
* You are relying on Jamf to update the app to keep pace with the mSCP
project.


