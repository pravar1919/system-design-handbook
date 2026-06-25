# Glossary

A one-line definition for every term used across the handbook. Entries link to the chapter where the concept is explained in depth. This file grows as chapters are written.

> Format: **Term** — short definition. *(See: [chapter](path))*

---

## A

- **ACID** — Atomicity, Consistency, Isolation, Durability: the guarantees a database transaction provides. *(See: 03-databases/01-acid-transactions.md)*
- **Availability (CAP)** — Every request to a non-failing node returns a non-error response in finite time. *(See: [09-consistency-and-consensus/01-cap-theorem.md](09-consistency-and-consensus/01-cap-theorem.md))*

## C

- **CAP theorem** — During a network partition you must choose between consistency and availability. *(See: [09-consistency-and-consensus/01-cap-theorem.md](09-consistency-and-consensus/01-cap-theorem.md))*
- **Consistency (CAP)** — Linearizability: every read sees the latest committed write, on any node. Distinct from ACID's "C." *(See: [09-consistency-and-consensus/01-cap-theorem.md](09-consistency-and-consensus/01-cap-theorem.md))*

## P

- **Partition (network)** — A failure that splits a cluster into groups that cannot exchange messages. *(See: [09-consistency-and-consensus/01-cap-theorem.md](09-consistency-and-consensus/01-cap-theorem.md))*

## Q

- **Quorum** — A minimum number of nodes (usually a majority) that must acknowledge an operation for it to count. *(See: [09-consistency-and-consensus/01-cap-theorem.md](09-consistency-and-consensus/01-cap-theorem.md))*

<!--
Maintainers: keep entries alphabetical within each letter heading. Add the
relevant letter heading if it does not yet exist. Every new chapter should
contribute its key terms here.
-->
