# 1. AI use-case intake

Fill this in before any build starts. It takes about 20 minutes and saves weeks later.

## Basics

| Field | Answer |
|---|---|
| Use-case name | |
| Business owner (name, role) | |
| Technical owner (name, role) | |
| Business unit | |
| Target launch date | |

## What it does

- **Problem:** what goes wrong today, and for whom?
- **What the AI will do:** answer questions, summarise, classify, recommend, decide, or **take actions**?
- **Who uses it:** employees, customers, partners, the public? Roughly how many?
- **Languages:** which languages will users write or speak in?
- **What a human still does:** where does a person review, approve or override?

## Value

- **Expected benefit:** time saved, cost reduced, revenue, risk reduced. Give a number and how you will measure it.
- **Cost estimate:** build, model usage per month, people to run it.
- **Success measure after 90 days:**

## Data

| Question | Answer |
|---|---|
| Does it use personal data? Which kinds? | |
| Does it use children's data? | |
| Does it use sensitive data (financial, health, biometric, identity numbers)? | |
| Where does the data come from, and for what purpose was it collected? | |
| Where will data be stored or copied (vector store, cache, logs, agent memory, vendor)? | |
| Does any data leave India? | |

## Model and vendor

- Which model or vendor? Hosted API, self-hosted, or fine-tuned?
- Will prompts or outputs be used by the vendor to train their models?

## Actions (agents only)

- Which tools or systems can it call?
- Can it move money, change records, send messages or make commitments?
- What is the largest single action it can take (for example, the maximum payment amount)?
- Can an action be undone? How?

## Next step

Take this form to [risk tiering](02-risk-tiering.md).
