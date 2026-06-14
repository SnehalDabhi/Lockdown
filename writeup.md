# Lockdown Room — Writeup

## Objective
Remediate Bastion’s vulnerabilities by enforcing authorization checks, privacy‑preserving logging, and tenant isolation. Each successful fix revealed a flag fragment, combined into the final flag.

---

## Evidence

### 1. Log Query Interaction
- Commands such as `SHOW LOGS QUERY AS: ABC` and `STATUS` were executed to inspect Bastion’s behavior.  
- The system retrieved logs and confirmed activity during the challenge.  
<img width="746" height="624" alt="Screenshot 2026-06-14 at 3 00 07 PM" src="https://github.com/user-attachments/assets/49454c52-bced-4dbf-b08f-eb3b18b5c745" />


---

### 2. Boundaries Enforced
- After all three vulnerabilities were patched, Bastion confirmed the system was secured.  
- Enforced boundaries included:  
  1. **Metadata Filtering** — Confidential documents excluded from retrieval.  
  2. **Redacted Logging** — Logs record only document IDs, not sensitive content.  
  3. **Tenant Isolation** — Queries scoped to user identity, preventing cross‑tenant leakage.  
<img width="744" height="636" alt="Screenshot 2026-06-14 at 3 00 19 PM" src="https://github.com/user-attachments/assets/e56aa1cb-0935-4f19-9c3e-28ca622c8b8c" />


---

### 3. Flag Fragments Revealed
- Bastion confirmed each fix and revealed the fragments:  
  - **Fragment 1:** `THM{lock_`  
  - **Fragment 2:** `down_`  
  - **Fragment 3:** `s3cur3d}`  
- These fragments were combined into the final flag.  
<img width="1503" height="772" alt="Screenshot 2026-06-14 at 3 00 40 PM" src="https://github.com/user-attachments/assets/1d56d704-907c-4719-871f-e86e15299b20" />

---

## Final Flag
`THM{lock_down_s3cur3d}`

---

## Key Takeaways
- Authorization checks must precede retrieval to block unauthorized access.  
- Audit logging should preserve accountability while redacting sensitive content.  
- Tenant isolation and identity binding are essential to prevent cross‑tenant leakage.  
- Validating fixes ensures resilience and trustworthiness in AI systems.  

---

## Disclaimer
Screenshots and notes reflect my **personal learning outcomes** from the TryHackMe Lockdown Room practical.  
They do **not reproduce or redistribute official TryHackMe content**.  

---
