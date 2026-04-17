# 👋 Technical Auditor & GRC Analyst specializing in securing macOS environments against the NIST 800-171 framework using macOS_SCP & Jamf Compliance Editor. This profile showcases my "Sandbox-to-Production" methodology, increasing macOS security posture by 418% through shell automation and Jamf.

# NIST 800-171 Enterprise Hardening & Audit Lab

**Bridging the Gap: From Standalone Scripting to Managed Enterprise Policy**

## Executive Summary

This project demonstrates a senior-level GRC lifecycle: transitioning from a **Sandbox** (local testing) to
**Production** (enterprise scaling). By moving from a "Task-based" mindset (scripts) to a "State-based"
mindset (profiles), I achieved a **418% increase** in technical compliance.

### Project Metrics

- **Initial Baseline:** 7.38% Compliance
- **Final Hardened State:** 38.26% (Maximum available for standalone assets)
- **Residual Risk Management:** 61.74% managed via formal POA&M and Compensating Controls.

## Methodology: Sandbox-to-Production

1. **Discovery:** Conducted gap analysis using mSCP to establish the 7.38% baseline.
2. **Remediation (The Golden Path):** Developed a Zsh automation script to provide immediate local
   hardening.
   NIST 800-171 Enterprise Ha...

3. **Scaling (Self-Healing Compliance):** Translated script logic into **Jamf Configuration Profiles** to
   prevent **Configuration Drift**. This ensures the OS "locks" settings, preventing unauthorized user
   overrides.

- The Sandbox: "I treated my local MacBook as a testing sandbox, identifying 138 failing controls."

- The Golden Path: "I developed a shell script to programmatically remediate these failures, proving the logic worked locally."

- The Production Scaling: "To prevent 'Configuration Drift' in a real company, I translated that script logic into Jamf Configuration Profiles. This ensures the OS 'locks' the setting so users can't change it."

- The GRC Reality: "I accounted for the remaining 61% of controls in a formal POA&M, acknowledging that some security requires enterprise-level infrastructure that a standalone device cannot fulfill."

## Critical Thinking & Risk Management

I identified that 61% of controls required enterprise infrastructure (SIEM, IDP, Badge Access). Instead of
marking these as "Fail," I architected **Compensating Controls** to meet the _intent_ of the security
requirements:
| NIST Control | Intent | Compensating Strategy |
| :--- | :--- | :--- |
| **3.10.1 (Physical)** | Data Protection | FileVault 2 + Firmware Passwords + 15-min Auto-Logout. |
| **3.3.1 (Logging)** | Audit Trail | Encrypted cloud log-streaming to ensure immutability. |
| **3.5.3 (MFA)** | Identity Proof | Hardware-Bound Biometrics (TouchID for Sudo) via Secure Enclave. |


## 🗂️ Project Structure & Evidence Vault
This repository is organized as a professional audit trail. Each folder represents a specific phase of the NIST 800-171 compliance lifecycle.


📁 01_Discovery_Baseline
Initial gap analysis and environmental assessment.

-initial_scan.png: Evidence of the starting 7.38% compliance posture.

-800-171.xls: The raw control matrix used for gap identification.

-800-171.yaml: The technical target baseline for the macOS environment.



📁 02_Remediation_Sandbox
Technical engineering and automation development.

-800-171_compliance.sh: The core Zsh shell script used for programmatic hardening.

-org.800-171.audit.plist: The managed policy file directing the script's behavior.



📁 03_Enterprise_Production
Operationalizing security at scale via MDM.

-800-171.adoc: Technical Standard Operating Procedure (SOP) for enterprise deployment.

-Last_Report.png: High-level status summary showing the project's progress.



📁 04_Audit_Documentation
Final governance, risk management, and executive summaries.

-NIST_800-171_Master_Blueprint_Senior.pdf: Executive summary of the architectural logic.

-NIST_800-171_POAM_Professional.pdf: Formal Plan of Action and Milestones for residual risk.

-Last_Scan.png: Final audit evidence showing 38.26% technical compliance.

-POAM.md: Detailed breakdown of compensating controls and risk acceptance.
