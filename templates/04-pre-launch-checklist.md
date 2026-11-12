# 4. Pre-launch checklist

Each line needs evidence: a test report, a log, a document link or a named owner. **L / M / H** marks the tiers that must complete the line.

## Quality

- [ ] **L M H** A test set of real (or realistic) questions with expected answers exists, owned by the business.
- [ ] **L M H** Accuracy on that test set meets the target agreed at intake.
- [ ] **M H** Quality is measured **in every supported language**, not only English.
- [ ] **M H** Known failure cases are listed, with what the system does in each.
- [ ] **H** A human-review sample of live outputs is planned for the first 30 days.

## Safety and domain rules

- [ ] **M H** Domain limits are written in plain words (for example: "gives market information, never buy or sell advice").
- [ ] **M H** Input and output guardrails enforce those limits, with a test showing they work.
- [ ] **H** The false-block rate is measured, so the guardrails do not block normal users.
- [ ] **H** The system says plainly when it cannot help, and hands over to a person.

## Security

- [ ] **M H** Prompt-injection testing, including **instructions hidden in retrieved documents**.
- [ ] **H** Injection and data-leak testing **in each supported language and script**, including disguised text.
- [ ] **M H** Secrets, keys and internal instructions are not reachable from user prompts.
- [ ] **H** Red-team exercise completed, findings fixed or formally accepted.

## Agents that take actions

- [ ] **H** Every tool has a written limit (amount, scope, rate).
- [ ] **H** Actions above a threshold need human approval.
- [ ] **H** Tested behaviour when tools fail: timeouts, garbage responses, **lost responses that could cause a duplicate action**.
- [ ] **H** Every action is logged with who, what, when and why, and can be reversed or compensated.
- [ ] **H** A kill switch exists and has been tested.

## Privacy and data

- [ ] **L M H** [DPDP checklist for AI](05-dpdp-for-ai.md) completed.
- [ ] **M H** Data minimisation: the system sees only the personal data it needs.
- [ ] **M H** Erasure works across vector stores, caches, logs and agent memory, and has been tested.

## Operations

- [ ] **L M H** Owner and on-call contact named.
- [ ] **M H** Monitoring dashboard: usage, cost, quality, guardrail blocks, errors.
- [ ] **M H** Cost per request and monthly budget agreed, with an alert.
- [ ] **H** Rollback plan tested.
- [ ] **L M H** Entry added to the [AI inventory](07-ai-inventory.csv).

## Sign-off

| Role | Name | Date | Conditions |
|---|---|---|---|
| Business owner | | | |
| Tech owner | | | |
| DPO (M, H) | | | |
| Security (M, H) | | | |
| AI council (H) | | | |
