## Almost all money is somebody's promise.

A banknote, a bank deposit, a gift card, an IOU between neighbours: in each
case someone has said they will pay.

This is a derivation of the smallest object that can carry a promise, a
protocol built from it, and the code that implements it.

```
  one object   a backing    B = (K, P, R, E)
                 K  who owes
                 P  what one unit pays
                 R  what must be handed over alongside it
                 E  who says a claim has not already been spent

  one carrier  a claim      a quantity held against a backing.
                            Bearer: whoever holds it, owns it.
  one holding  a wallet     a set of claims, plus any bare assets

  the law      nothing you owe (your written maximum) grows
               without your signature.
               nothing you hold leaves without your signature.
```

Making money is a licensed activity. The usual answers are to fix the
institution, which keeps the licence, or to escape it with money fully backed
by something scarce — which builds something real, and stays small, because it
creates almost no money. This takes a third route: a **grammar** instead of a
money. One object, general enough to write fiat, a bank deposit, a bill of
exchange, a stablecoin and a neighbour's word.

## Where things are

| | |
|---|---|
| **[money-from-first-principles](https://github.com/mediumofexchange/money-from-first-principles)** | The paper — why, the derivation, the law, what emerges, the limits. And the protocol: [Construction](https://github.com/mediumofexchange/money-from-first-principles/blob/main/construction.md) is the normative core, [Extensions](https://github.com/mediumofexchange/money-from-first-principles/blob/main/extensions.md) the optional profiles on top of it. |
| **[reference-ts](https://github.com/mediumofexchange/reference-ts)** | Experimental shielded-pool implementation: private notes, public supply replay, canonical history, receipt readers and durable sequencing. Recovery is modeled; the wallet and external witness write side remain to be built. |
| **[mediumofexchange.github.io](https://github.com/mediumofexchange/mediumofexchange.github.io)** | The front door at [mediumofexchange.org](https://mediumofexchange.org). |

## Three names, three jobs

They change at different rates, so they are kept apart.

- **Money from First Principles** is the paper, and keeps its name. An argument
  is cited, not versioned.
- **The Medium of Exchange Protocol** is what Construction and Extensions
  define: the object, the law, and the machinery around them. This is the thing
  that gets built.
- **mediumofexchange.org** is the front door, with this org and the
  `@mediumofexchange` npm scope behind it.

## Status

The protocol has one experimental reference implementation, building
Construction's core claim layer, the shielded pool, rule by rule. The API and
wire format can change; there has been no completed security audit.

The package is not published to npm. Follow the implementation's
[setup and verification instructions](https://github.com/mediumofexchange/reference-ts#readme)
to build from source. Its
[local pilot](https://github.com/mediumofexchange/reference-ts/blob/main/docs/PILOT.md)
remains a transparent-path integration harness with a trusted local witness.

## Licence

CC0 1.0 Universal across everything here — public domain dedication. No
permission needed, for anything, ever. If you build a money on this, you owe
nobody here a thing.
