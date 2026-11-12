# 8. AI incident response

## What counts as an AI incident

- The system reveals personal data, secrets or internal instructions
- It gives harmful, unsafe or clearly wrong guidance in a sensitive domain
- An agent takes a wrong, duplicate or unauthorised action
- It is manipulated by prompt injection
- It discriminates against a group of users
- A large, unexpected jump in cost or errors

## Severity

| Level | Example | Response time |
|---|---|---|
| **Sev 1** | Personal data leaked; money moved wrongly; harmful advice at scale | Act within 1 hour; AI council within 48 hours |
| **Sev 2** | Wrong answers in a sensitive domain, few users affected; guardrail bypass found | Same working day |
| **Sev 3** | Quality drop, odd outputs, no harm | Within a week |

## First hour (Sev 1)

1. **Contain:** pause the feature, disable the tool, or switch to the safe fallback. Use the kill switch.
2. **Preserve evidence:** save prompts, outputs, tool calls and versions involved.
3. **Notify:** owner, CAIO, CISO and DPO. If personal data is involved, the DPO starts the breach process.
4. **Size it:** how many users, which data, which actions?

## Within 72 hours

5. Find the root cause: model change, prompt change, data change, new attack, tool failure.
6. Fix and **add a test** so the same failure is caught before the next release.
7. Reverse or compensate affected actions; tell affected people where required.
8. Decide with the AI council whether to resume, and under what conditions.

## Post-incident review (blameless)

| Question | Answer |
|---|---|
| What happened, in plain words? | |
| How did we find out? Could we have found out sooner? | |
| Why did existing tests and guardrails not catch it? | |
| What test, guardrail or process change prevents a repeat? | |
| Owner and due date for each change | |
