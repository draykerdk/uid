# UID

> Identity, revocable representation and contextual contribution records.

UID separates the person, the agent authorised to act for them and the record of their contributions. It proposes identity and attribution that preserve personal authority across the ecosystem.

An account, an automated representative and a contribution history answer different questions. Combining them can obscure consent and turn a limited record into a judgement of the whole person.

## Three distinct responsibilities

### The person and their cryptographic identity

The identity layer should let a member authenticate and demonstrate the credentials needed for an interaction while disclosing only the required information. The proposal explores zero-knowledge proofs and separate identifiers for different relationships. Their protection depends on protocol design, metadata exposure, recovery procedures and implementation; distinct keys alone do not prevent every form of correlation.

A person's standing as a member is distinct from the state of a credential. Lost keys, compromised devices and contested access require recovery and human recourse. Automated enforcement must not become a way to erase the person or make their basic rights contingent on a technical record.

Membership rests on personhood. Only a UID holder can access the system, and each UID corresponds to one living person. Personhood is established by multi-factor biometrics, certified by people at enrolment and verified continuously afterwards, which makes fabricating or duplicating members close to impossible. That is what keeps coordinated crowds of fake accounts out of the network's debates. Whoever certifies a UID puts part of their own reputation at stake, but only for proven fraud or collusion, never for an honest error, so that the door stays open to new members. The biometric data belongs to the member, who can see what is collected and what it is used for. It is not kept in a central database, and what other members see stays minimal, so anonymity towards them remains possible, as with the justified veto. The protocol, its threat model and recovery still have to be specified and evaluated here.

Rights and duties apply to the active member, who uses Drayker as their base supersystem. A member who holds a UID and does not use the network remains a member, inactive: the UID stays inactive until it is used again, Dk Personal is active only for active members, the member's state is kept, and there is no penalty.

UID is also the primary application of the system: the base from which the other Drayker applications are built, the super app in which DkApps run. It works as a living record of the member’s life inside Drayker, under the member’s control.

### The agent and its mandate

A [Dk Personal](https://personal.drayker.org) agent may act as a proxy within permissions the member gives it. A mandate should state its scope, limits and duration, and provide a way to revoke it. Actions that exceed those limits need renewed authorisation. The agent represents the person within that mandate; constitutional authority remains with the person.

A useful worked case would show a mandate being issued, used, withdrawn and checked by another participant before a later action is accepted. That sequence must be demonstrated in the protocol, including what happens during disconnection or delayed revocation delivery.

#### Least privilege and audit

A mandate is one case of a general principle: every privilege in the system should be minimal, temporary, contextual and auditable. It covers only what the action needs, lasts only as long as it is needed, holds only in the context it was granted for, and can be reviewed afterwards.

Every privileged action follows one sequence:

1. **identity** — who or what is acting is established;
2. **permission** — the privilege held is checked against what the action requires;
3. **authorised context** — the action is confirmed to fall within the context the permission was granted for;
4. **action**;
5. **record** — a high-impact action is recorded;
6. **audit** — matching the level of access;
7. **review or revocation** — and the cycle starts again.

Compartmentalisation and operation with isolated parts, the detection of anomalous behaviour and fault tolerance belong to [Dk Network](https://dknetwork.drayker.org) and [Living Cryptography](https://lc.drayker.org).

### Contributions in context

[Contextual reputation](https://dknowledge.drayker.org/papers/main-projects/ecosystem/value-management-ecosystem#reputation) records concern evidence of contribution within a domain. They should preserve enough context to evaluate the work and correct errors. Expertise in one field does not by itself establish authority in another, and the proposal rejects a single score purporting to measure a person's worth.

The reputation of work cannot be purchased or transferred. Holding financial capacity does not buy constitutional voice. The reward is a specific kind of reputation and the one exception: contributing capacity, such as computing, or financing the network earns the only transferable reputation, which can give faster or priority access to resources. It never carries weight in the members’ constitutional choices. Base representation and the veto remain rights of every active member, independent of those records. The common capacity floor also belongs to every active member. While the network cannot sustain it for everyone, mainly when resources are scarce, access depends on an endorsement that works more like a queue weighted by context, such as need and urgency, than like an approval; at the start, contextual reputation helps protect the network against abuse. As capacity grows, what depended on the queue becomes part of the floor ([Distributed Support](https://support.drayker.org)).

## Personal authority and review

UID supports the member's authority over their body, private context and delegated actions. Each member holds an absolute veto: power over their own life and their own Dk Personal (what stays private, what Dk represents, refusing a task, leaving). It holds only within the vetoer's own sphere, and what also affects others goes through the contextual veto. A situated refusal must be assessed in its actual scope, including any effects on other members and shared commitments. [Member councils](https://advices.drayker.org), convened for each question, are the proposed human review path for contested decisions.

Privacy includes room to rest, reconsider and keep personal exploration outside public attribution. The specification must explain how consent, disclosure and record correction are carried across connected systems.

## The veto chain

A veto only protects anyone if it cannot be lost, forged or quietly ignored, and it only teaches the system something if it carries its reasons. The proposal records every act of constitutional authority as a signed entry in a shared chain of signatures: a signed, hash-linked, append-only record, carried by the Drayker architecture rather than by an external token network.

**What enters the chain.** A situated veto, a justified veto against a collective decision, the revocation of a mandate, a member's signature on a constitutional ratification, the conclusion of a [member council](https://advices.drayker.org), and the outcome of every triage described below. The contested decision is referenced by its cryptographic address: in the [Dk Network](https://dknetwork.drayker.org) architecture every function, module and block of information already has a unique address derived from a signature, so a veto points at exactly the decision it contests.

**A veto comes with its grounds.** Every veto carries its real justification: the intention and the motives behind it, the scope it claims — which action, who is affected, what interrupting it would cost others — and the facts or conditions it rests on. A veto without reasons teaches the system nothing; a veto with reasons can reveal a condition no data showed. The author can stay anonymous: the entry proves that its signer is a member with standing in the affected context without revealing who they are. Anonymity protects the person, never the absence of reasons. Where the grounds touch someone's body, home or private context, those details can be sealed so that only the triage examining them can read them — they are still weighed.

**How vetoes are weighed.** Vetoes are not counted like votes. Their grounds are weighed together: the intentions and motives each one carries, each person's relation to the decision, the certainty on each side and what the vetoes reveal in common. A person counts once, however many contexts they belong to. Many vetoes repeating the same grounds add weight to those grounds, not new information. And one veto can be enough: when its grounds bring information beyond the scope considered before the decision was taken, it can by itself lead to an adjustment — an exception, a narrower scope, a new test or the revision of the rule.

**From veto to adjustment.** A contextual veto reaches an adjustment through a rite that makes it possible to:

- **situate its reach** — which action, who is affected, what interrupting it would cost others;
- **delimit the veto** — state exactly what it contests;
- **examine the effects in dispute**;
- **look for another way to fulfil the common purpose**;
- **adjust** — by an exception, a narrower scope, a new test or the revision of the rule.

The advanced triage below safeguards the grounds that the rite relies on.

**Advanced triage.** Because a single well-founded veto can change a decision, its grounds pass through safeguards before they do:

- **verification** of the facts claimed, against records, sensors and independent sources, and with the people and local Dks of the affected context;
- **interpretation** of what the new information actually means for this decision, not only whether it is true;
- **detection** of error, misunderstanding and manipulation, including coordinated vetoes and fabricated grounds;
- **proportion**: a bounded test or a temporary exception before a general change;
- **human recourse**: a contested triage goes to a member council convened for that question.

The triage outcome is appended to the chain with its own reasons, so whoever vetoed can see how their grounds were read. A veto that does not pass triage stays in the record and can be reconsidered when new evidence appears.

**How the chain survives failure.** No node holds the chain alone. It is replicated across Dk Network nodes and accepted by propagation: independent nodes on the route — at least three, the same threshold the network uses to authenticate modules — check the signature, the standing of the signer and the link to the previous entry before relaying it. [Living Cryptography](https://lc.drayker.org) protects the channels between them. A device can sign while disconnected; the entry propagates on reconnection with its original order preserved. Conflicting histories are not silently resolved by majority: they are kept visible and taken to a member council.

**What it binds.** Before executing a decision, the operational layer — Dk Global included — checks the chain for vetoes against that decision's address and for the state of their triage. A justified veto obliges the decision to be revised until consensus; an action that ignores one is detectable by any node, because the veto and the action carry the same address. Constitutional ratifications need member signatures and independent keys that no Dk process holds: Dk Global can append a proposal to the chain, never a ratification, and each change follows the constitutional procedure, built with Dk Global and within the kernel.

**Where it runs today.** Nowhere yet. The closest working precedent is the DAF's Phase 0, where Git history is the ledger and anyone can recompute it ([DAF-001](https://github.com/draykerdk/daf/blob/master/dafp/daf-001-phase-0-github-federation.md)). The veto chain is a requirement for the stage in which a well-deployed Dk Global can no longer be switched off and the justified veto becomes the switch — so it has to exist, and be tested, before that stage.

## How UID connects to the ecosystem

[Projects & Applications (PAP)](https://pap.drayker.org) would use UID for attributable participation in projects. PAP names that project environment; it does not name a proof-of-personhood protocol. Personhood verification belongs to UID, through the multi-factor biometrics described above.

[Living Cryptography](https://lc.drayker.org) researches relevant security mechanisms. [Dk Personal](https://personal.drayker.org) develops the personal proxy, and [Value Unit](https://value.drayker.org) preserves the distinction between material capacity and constitutional standing.

## What needs to be demonstrated

The published architecture requires protocol work and evaluation. Priority cases are credential recovery, bounded delegation and revocation, selective disclosure, resistance to correlation, correction of a contextual contribution record, resistance to collusion among validators — a validation weighs more when it comes from independent contexts (see [Reputation](https://dknowledge.drayker.org/papers/main-projects/ecosystem/value-management-ecosystem#reputation) in the economy of capacity) — and one veto carried end to end: signed offline with its grounds, propagated, checked by independent nodes, triaged, and honoured by the layer that would have executed the contested decision. Each needs explicit assumptions, failure cases and an accessible review path.

## Participation and sources

This repository develops a proposal through public documentation and review. Read the [contribution guide](https://github.com/draykerdk/.github/blob/master/CONTRIBUTING.md) and [current governance](https://github.com/draykerdk/.github/blob/master/GOVERNANCE.md), or find a bounded contribution on the [open-functions board](https://drayker.org/fn/).

Part of [Drayker](https://drayker.org). Content licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
