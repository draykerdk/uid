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

## The veto chain

A veto only protects anyone if it cannot be lost, forged or quietly ignored. The proposal therefore records every act of constitutional authority as a signed entry in a shared, append-only chain of signatures — blockchain-style, but carried by the Drayker architecture rather than by an external token network.

**What enters the chain.** A situated veto, a justified veto against a collective decision, the revocation of a mandate, a member's signature on a constitutional ratification, and an order of the [independent member panel](https://advices.drayker.org). The contested decision itself is referenced by its cryptographic address: in the [Dk Network](https://dknetwork.drayker.org) architecture every function, module and block of information already has a unique address derived from a signature, so a veto can point at exactly the decision it contests.

**How an entry is made.** The member signs with their UID key. A [Dk Personal](https://personal.drayker.org) may carry a veto only within a mandate that allows it, and the entry records that it did. Each entry holds the hash of the entry before it, so removing or altering one breaks every link that follows.

**How the chain survives failure.** No node holds the chain alone. It is replicated across Dk Network nodes and accepted by propagation: independent nodes on the route — at least three, the same threshold the network uses to authenticate modules — check the signature, the standing of the signer and the link to the previous entry before relaying it. [Living Cryptography](https://lc.drayker.org) protects the channels between them. A device can sign while disconnected; the entry propagates on reconnection with its original order preserved. Conflicting histories are not silently resolved by majority: they are kept visible and sent to the panel.

**What it binds.** Before executing a decision, the operational layer — Dk Global included — checks the chain for a valid veto against that decision's address. A justified veto obliges the decision to be revised until consensus (*Do animal à superinteligência*, chapter 47); an action that ignores one is detectable by any node, because the veto and the action carry the same address. A sustained pattern of refusals triggers panel review. Constitutional ratifications need member signatures and independent keys that no Dk process holds: Dk Global can append a proposal to the chain, never a ratification.

**What it does not expose.** The chain carries proofs, not lives. An entry states that a member with standing vetoed a given decision within a given scope; the reasons tied to a person's body, home or private context stay outside it, disclosed selectively or not at all. A veto over one's own sphere is valid by standing and does not need to justify itself in public.

**Where it runs today.** Nowhere yet. The closest working precedent is the DAF's Phase 0, where Git history is the ledger and anyone can recompute it ([DAF-001](https://github.com/draykerdk/daf/blob/master/dafp/daf-001-phase-0-github-federation.md)). The veto chain is a requirement for the stage the book describes, in which a well-deployed Dk Global can no longer be switched off and the justified veto becomes the switch — so it has to exist, and be tested, before that stage.

## How UID connects to the ecosystem

[Projects & Applications (PAP)](https://pap.drayker.org) would use UID for attributable participation in projects. PAP names that project environment; it does not name a proof-of-personhood protocol. Personhood verification remains an identity-design question to specify and evaluate here.

[Living Cryptography](https://lc.drayker.org) researches relevant security mechanisms. [Dk Personal](https://personal.drayker.org) develops the personal proxy, and [Value Unit](https://value.drayker.org) preserves the distinction between material capacity and constitutional standing.

## What needs to be demonstrated

The published architecture requires protocol work and evaluation. Priority cases are credential recovery, bounded delegation and revocation, selective disclosure, resistance to correlation, correction of a contextual contribution record, and one veto carried end to end: signed offline, propagated, checked by independent nodes and honoured by the layer that would have executed the contested decision. Each needs explicit assumptions, failure cases and an accessible review path.

## Participation and sources

This repository develops a proposal through public documentation and review. Read the [contribution guide](https://github.com/draykerdk/.github/blob/master/CONTRIBUTING.md) and [current governance](https://github.com/draykerdk/.github/blob/master/GOVERNANCE.md), or find a bounded contribution on the [open-functions board](https://drayker.org/fn/).

Part of [Drayker](https://drayker.org). Content licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
