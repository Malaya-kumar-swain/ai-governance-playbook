# 3. Approval matrix

R = responsible, A = approves, C = consulted, I = informed.

| Step | Business owner | Tech owner | Data protection (DPO) | Security | Legal | AI council / CAIO |
|---|---|---|---|---|---|---|
| Intake and tiering | R | C | C | | | I |
| **Low tier** go-live | A | R | I | I | | I |
| **Medium tier** go-live | A | R | C | C | | I |
| **High tier** go-live | R | R | C | C | C | **A** |
| Adding a new tool or action to an agent | C | R | C | C | | A |
| Model or vendor change | C | R | C | C | C (contract) | I (High: A) |
| Incident: severity 1 | I | R | C | C | C | A |

## AI council (for high-tier use cases)

- **Members:** CAIO or Head of AI (chair), CISO, DPO, Head of Risk, Legal, one business leader.
- **Meets:** monthly, plus within 48 hours for severity 1 incidents.
- **Decides:** high-tier launches, risk acceptance, policy changes, pausing a system.
- **Records:** every decision, with the evidence reviewed and any conditions.

## Rule of thumb

The person who approves a launch must be able to answer, in one sentence each: what can go wrong, how we would know, and how we would stop it.

Next: [pre-launch checklist](04-pre-launch-checklist.md).
