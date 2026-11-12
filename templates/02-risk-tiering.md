# 2. Risk tiering

Score each factor, then use the **highest** factor score as the tier. One high-risk factor makes the whole use case high risk.

| Factor | Low (1) | Medium (2) | High (3) |
|---|---|---|---|
| **Who sees the output** | Internal team only | Employees across the company | Customers or the public |
| **What the AI does** | Drafts for a human to edit | Recommends; a human decides | Decides or **takes actions** on its own |
| **Personal data** | None | Ordinary personal data | Sensitive data, children's data, or identity numbers |
| **Domain** | General productivity | Operations, HR, sales | Finance, health, legal, safety, credit or eligibility decisions |
| **Reversibility** | Easy to undo | Undo needs manual effort | Hard or impossible to undo (payments, messages sent, decisions communicated) |
| **Scale** | Under 100 users | 100 to 100,000 users | Over 100,000 users, or vulnerable groups |
| **Languages** | One language, tested | Several languages, some tested | Many languages, not all tested |

## Tiers

| Tier | What it means | Typical examples |
|---|---|---|
| **Low** | Fast track. Standard checklist, team-level approval. | Internal document search, meeting summaries |
| **Medium** | Full pre-launch checklist. Risk and data protection review. | Employee helpdesk bot, sales email drafts |
| **High** | Full checklist plus red-team testing, legal review and AI council approval. Staged rollout. | Customer-facing assistant, agents that take actions, credit or health guidance |

## Re-tier when

- the AI gets a new tool or a new kind of action,
- it moves from internal to customer-facing,
- it starts using a new kind of personal data,
- a serious incident happens.

Next: [approval matrix](03-approval-matrix.md).
