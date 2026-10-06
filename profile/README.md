# Medium of Exchange

A protocol for issuing and exchanging claims against publicly defined promises.
The goal is open entry, private payments and independently verifiable supply.
Holders choose which promises to accept; the protocol does not guarantee repayment.

The project brings together an argument for the design, a normative specification
and an experimental implementation.

| Repository | Start here for |
|---|---|
| [Money from First Principles](https://github.com/mediumofexchange/money-from-first-principles) | The paper and protocol specification: the reasoning, rules and limits. |
| [TypeScript reference](https://github.com/mediumofexchange/reference-ts) | Executable protocol behavior, verification evidence and source setup. |
| [Website](https://github.com/mediumofexchange/mediumofexchange.github.io) | The static project overview at [mediumofexchange.org](https://mediumofexchange.org). |

The reference implements private notes, public supply replay, canonical history,
receipt readers, durable sequencing, runtime recovery, a seed-restorable pool
wallet and Ergo publication, with real proofs on reference venues and live on
the Ergo testnet. Qualified custody and mainnet use remain open. There is no published
npm release or completed security audit; API and wire formats can change.

See the [implementation status](https://github.com/mediumofexchange/reference-ts/blob/main/docs/IMPLEMENTATION_STATUS.md)
for evidence and limits, and the [decision index](https://github.com/mediumofexchange/reference-ts/blob/main/DECISIONS.md)
for design rationale.

CC0 1.0 Universal — public domain dedication across the project.
