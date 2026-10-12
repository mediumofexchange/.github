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

The reference implements the shielded pool (pool-v3): private notes, public supply
replay, canonical history, receipt readers, durable sequencing, single-backing
recovery, a seed-restorable wallet and Ergo publication. Lit notes (`moe/lit/v1`),
the transparent profile, run beside it. Both formats are adopted by name; a change
to one is a new version. The `moe` commands run a wallet, an operator, a supply
reader, a replica and a relay, with real proofs on a synthetic Ergo chain; the
pool's commands have also run live on the Ergo testnet. A
[release record](https://github.com/mediumofexchange/reference-ts/blob/main/docs/RELEASE.md)
rebuilds the package byte for byte, and a
[security argument](https://github.com/mediumofexchange/reference-ts/blob/main/docs/SECURITY_ARGUMENT.md)
states what a release claims for an external review to check. Statements spending
several backings, a phone-first wallet, qualified custody and mainnet use remain
open. There is no published npm release or completed security audit; the API can change.

See the [implementation status](https://github.com/mediumofexchange/reference-ts/blob/main/docs/IMPLEMENTATION_STATUS.md)
for evidence and limits, and the [decision index](https://github.com/mediumofexchange/reference-ts/blob/main/DECISIONS.md)
for design rationale.

CC0 1.0 Universal — public domain dedication across the project.
