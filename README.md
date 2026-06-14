# Lockdown Room — AI Security Practical

The **Lockdown Room** on TryHackMe is a hands‑on security exercise where I assumed the role of a **security engineer** tasked with strengthening an AI assistant named **Bastion**.  
This repository documents my systematic approach to identifying vulnerabilities, designing precise security controls, and validating fixes — transforming Bastion from a vulnerable system into a resilient one.

---

## Why This Practical Matters
AI assistants are increasingly integrated into enterprise workflows, yet they remain exposed to risks such as unauthorized data retrieval, privacy gaps in logging, and weak tenant isolation.  
Through this practical, I demonstrate my ability to:
- **Diagnose vulnerabilities** with accuracy and clarity.  
- **Design and enforce targeted security controls** that remediate real risks.  
- **Capture evidence of remediation** through flag fragments.  
- **Align solutions with industry frameworks** for AI security and compliance.  

---

## Objectives
- Enforce **pre‑retrieval authorization checks** to prevent unauthorized data access.  
- Implement **privacy‑preserving audit logging** that ensures accountability without exposing sensitive content.  
- Apply **tenant isolation and identity binding** so access dynamically respects the requester’s identity.  

---

## Technical Details
- Accessed Bastion via a **command‑line chat interface**, logged in as a security administrator.  
- Identified three critical vulnerabilities, applied fixes, and captured flag fragments as proof of remediation.  
- Commands used included:  
  - `STATUS` → Verify system state.  
  - `SHOW LOGS` → Inspect logging behavior.  
  - `QUERY AS: <name>` → Test tenant isolation.  

---

## Steps Completed
1. **Initialize Bastion** — Verified baseline system state with `STATUS`.  
2. **Identify Vulnerabilities** — Inspected logs and tested tenant isolation.  
3. **Apply Fixes** — Articulated precise security controls, prompting Bastion to remediate.  
4. **Capture Evidence** — Collected flag fragments after each successful remediation.  
5. **Validate Controls** — Confirmed fixes through subsequent `STATUS` checks.  

---

## Success Indicators
- All three flag fragments captured, confirming vulnerabilities were remediated.  
- Bastion now enforces proper security controls without exposing sensitive information.  

---

## Learning Outcomes
- Strengthened understanding of **authorization checks** in AI assistants.  
- Designed **audit logging** that balances privacy with accountability.  
- Applied **tenant isolation and identity binding** to prevent cross‑user data leakage.  
- Reinforced the importance of **precise, actionable security controls** in AI systems.  

---

## Repository Structure

- **README.md** → Polished overview for recruiters and collaborators.  
- **writeup.md** → Detailed case study with steps, screenshots, and flag evidence.  
- **screenshots/** → Proof of successful remediation.  

---

## Disclaimer
These notes and screenshots represent my **personal learning outcomes** from the TryHackMe Lockdown Room practical.  
They do **not reproduce or redistribute official TryHackMe content**.  

