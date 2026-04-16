# 👋 Technical Auditor & GRC Analyst specializing in securing macOS environments against the NIST 800-171 framework using macOS_SCP & Jamf Compliance Editor. This profile showcases my "Sandbox-to-Production" methodology, increasing macOS security posture by 418% through shell automation and Jamf.

# NIST 800-171 Enterprise Hardening & Audit Lab
**Bridging the Gap: From Standalone Scripting to Managed Enterprise Policy**
## Executive Summary
This project demonstrates a senior-level GRC lifecycle: transitioning from a **Sandbox** (local testing) to
**Production** (enterprise scaling). By moving from a "Task-based" mindset (scripts) to a "State-based"
mindset (pro!les), I achieved a **418% increase** in technical compliance.
### Project Metrics
- **Initial Baseline:** 7.38% Compliance
- **Final Hardened State:** 38.26% (Maximum a&ainable for standalone assets)
- **Residual Risk Management:** 61.74% managed via formal POA&M and Compensating Controls.
## Methodology: Sandbox-to-Production
1. **Discovery:** Conducted gap analysis using mSCP to establish the 7.38% baseline.
2. **Remediation (The Golden Path):** Developed a Zsh automation script to provide immediate local
hardening.
NIST 800-171 Enterprise Ha...

3. **Scaling (Self-Healing Compliance):** Translated script logic into **Jamf Con!guration Pro!les** to
prevent **Con!guration Dri%**. This ensures the OS "locks" se&ings, preventing unauthorized user
overrides.
## Critical Thinking & Risk Management
I identi!ed that 61% of controls required enterprise infrastructure (SIEM, IDP, Badge Access). Instead of
marking these as "Fail," I architected **Compensating Controls** to meet the *intent* of the security
requirements:
| NIST Control | Intent | Compensating Strategy |
| :--- | :--- | :--- |
| **3.10.1 (Physical)** | Data Protection | FileVault 2 + Firmware Passwords + 15-min Auto-Logout. |
| **3.3.1 (Logging)** | Audit Trail | Encrypted cloud log-streaming to ensure immutability. |
| **3.5.3 (MFA)** | Identity Proof | Hardware-Bound Biometrics (TouchID for Sudo) via Secure Enclave. |
## Repository Structure
- `/01_Baseline`: Initial scan reports (7.38% baseline).
- `/02_Remediation`: "Golden Path" Zsh remediation scripts.
- `/03_Enterprise`: Apple-native `.mobilecon!g` pro!les for Jamf Pro deployment.
- `/04_Documentation`: Final Audit Report and the formal POA&M.

