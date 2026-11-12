# 5. DPDP checklist for AI systems

The Digital Personal Data Protection Act, 2023 and the DPDP Rules apply to AI systems the same way they apply to any other processing of digital personal data. AI adds new places where data hides: embeddings, caches, prompt logs, fine-tuned models and agent memory. This checklist maps the main duties to those places.

> Not legal advice. Confirm current obligations, timelines and any sector rules with your legal team.

## Notice and consent

- [ ] The notice given to the person covers the AI use, in plain language, in a language they can read.
- [ ] Consent (or another lawful basis) covers **this purpose**. Data collected for one purpose is not reused for another AI purpose without a valid basis.
- [ ] Withdrawal of consent is as easy as giving it, and the AI system **stops using** the data after withdrawal.

## Purpose limitation in retrieval

- [ ] Documents and records carry the purpose they were collected for.
- [ ] Retrieval (RAG) only returns data whose purpose matches the request.
- [ ] Records that mention several people respect **every** person's consent, not only the requester's.

## Data in AI-specific places

| Place | Question | Done |
|---|---|---|
| Vector store / embeddings | Can one person's data be found and deleted? | [ ] |
| Response cache | Are cached answers containing personal data purged on erasure? | [ ] |
| Prompt and output logs | Is personal data masked, and are logs kept only as long as needed? | [ ] |
| Agent memory | Can a person's memories be listed and deleted? | [ ] |
| Fine-tuned models | Was personal data used to train? If so, how will erasure be honoured? | [ ] |
| Vendor / model provider | Does the vendor store or train on prompts? Is that allowed by contract? | [ ] |

## Rights of the person

- [ ] Access: you can tell a person what personal data the AI system holds about them and for which purposes.
- [ ] Correction and erasure work across all the places above, and you can **show evidence** that erasure happened.
- [ ] A grievance route exists and is visible to users.

## Children

- [ ] If children may use the system, the rules on verifiable parental consent and on tracking, monitoring and targeted advertising are addressed.

## Security and breach

- [ ] Reasonable security safeguards are documented, including for vendors.
- [ ] Prompt injection and data-leak testing has been done (see the [pre-launch checklist](04-pre-launch-checklist.md)).
- [ ] The breach process covers AI incidents, such as a model revealing someone's personal data, and meets the notification duties to the Board and affected people.

## Data leaving India

- [ ] You know where model inference and storage happen, and that any transfer outside India is allowed under current rules and sector directions.

## Evidence to keep

- Consent records with notice version and purpose
- Erasure logs with proof of deletion per store
- Test reports for leakage and injection
- Vendor data-processing terms
