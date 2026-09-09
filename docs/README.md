# UID

> Identity, revocable representation and contextual contribution records.

UID separates the person, the agent authorised to act for them and the record of their contributions. It proposes identity and attribution that preserve personal authority across the ecosystem.

An account, an automated representative and a contribution history answer different questions. Combining them can obscure consent and turn a limited record into a judgement of the whole person.

## Three distinct responsibilities

### The person and their cryptographic identity

The identity layer should let a member authenticate and demonstrate the credentials needed for an interaction while disclosing only the required information. The proposal explores zero-knowledge proofs and separate identifiers for different relationships. Their protection depends on protocol design, metadata exposure, recovery procedures and implementation; distinct keys alone do not prevent every form of correlation.

A person's standing as a member is distinct from the state of a credential. Lost keys, compromised devices and contested access require recovery and human recourse. Automated enforcement must not become a way to erase the person or make their basic rights contingent on a technical record.

### The agent and its mandate

A [Dk Personal](https://personal.drayker.org) agent may act as a proxy within permissions the member gives it. A mandate should state its scope, limits and duration, and provide a way to revoke it. Actions that exceed those limits need renewed authorisation. The agent represents the person within that mandate; constitutional authority remains with the person.

A useful worked case would show a mandate being issued, used, withdrawn and checked by another participant before a later action is accepted. That sequence must be demonstrated in the protocol, including what happens during disconnection or delayed revocation delivery.

### Contributions in context

Reputation records concern evidence of contribution within a domain. They should preserve enough context to evaluate the work and correct errors. Expertise in one field does not by itself establish authority in another, and the proposal rejects a single score purporting to measure a person's worth.

Reputation cannot be purchased or transferred. Holding financial capacity does not buy constitutional voice. The current proposal also excludes financial contribution from reputation; any refinement of how material contributions are documented belongs in an explicit governance proposal. Basic support and participation rights remain independent of those records.

## Personal authority and review

UID supports the member's authority over their body, private context and delegated actions. A situated refusal must be assessed in its actual scope, including any effects on other members and shared commitments. The [independent member panel](https://advices.drayker.org) is the proposed human review path for contested decisions.

Privacy includes room to rest, reconsider and keep personal exploration outside public attribution. The specification must explain how consent, disclosure and record correction are carried across connected systems.

## How UID connects to the ecosystem

[Projects & Applications (PAP)](https://pap.drayker.org) would use UID for attributable participation in projects. PAP names that project environment; it does not name a proof-of-personhood protocol. Personhood verification remains an identity-design question to specify and evaluate here.

[Living Cryptography](https://lc.drayker.org) researches relevant security mechanisms. [Dk Personal](https://personal.drayker.org) develops the personal proxy, and [Value Unit](https://value.drayker.org) preserves the distinction between material capacity and constitutional standing.

## What needs to be demonstrated

The published architecture requires protocol work and evaluation. Priority cases are credential recovery, bounded delegation and revocation, selective disclosure, resistance to correlation, and correction of a contextual contribution record. Each needs explicit assumptions, failure cases and an accessible review path.

## Participation and sources

This repository develops a proposal through public documentation and review. Read the [contribution guide](https://github.com/draykerdk/.github/blob/master/CONTRIBUTING.md) and [current governance](https://github.com/draykerdk/.github/blob/master/GOVERNANCE.md), or find a bounded contribution on the [open-functions board](https://drayker.org/fn/).

Part of [Drayker](https://drayker.org). Content licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
