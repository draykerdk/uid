# UID — Universal Identity Drayker

> Self-sovereign human identity, agentic proxy delegation, and contextual reputation without panopticon surveillance.

UID is the architectural specification for identity, representation, and attribution across the Drayker ecosystem. As established in *Do animal à superinteligência* (Chapters 34–38, 41–43), sustainable human sovereignty in the age of autonomous machines requires an absolute structural separation between who a person is, how their software acts on their behalf, and how their contributions are recognized.

---

## 1. The Three Structural Layers

UID decomposes "identity" into three distinct, non-fungible layers to prevent bureaucratic capture, behavioral profiling, and algorithmic totalitarianism:

```
┌────────────────────────────────────────────────────────────────────────┐
│ 1. CRYPTOGRAPHIC ROOT (Self-Sovereign Personhood)                      │
│    Zero-knowledge proofs, ephemeral session keys, non-correlatable     │
│    pairwise identifiers. No central registry, no biometric lock-in.   │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │ Authorizes & mandates
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│ 2. REPRESENTATIVE PROXY AGENT (Bounded Agency)                         │
│    Local and edge autonomous agents operating on the member's behalf.  │
│    Executes routines, negotiates tasks, carries revocable mandates.    │
│    *The proxy is an instrument, never the sovereign human.*            │
└───────────────────────────────────┬────────────────────────────────────┘
                                    │ Delivers verified work
                                    ▼
┌────────────────────────────────────────────────────────────────────────┐
│ 3. CONTEXTUAL REPUTATION CLUSTERS (Empirical Domain Lineage)          │
│    Verified track record earned through delivered functions.           │
│    Segmented by domain; cannot be aggregated into a single score.      │
│    *Non-transferable, non-financializable, cannot be bought.*          │
└────────────────────────────────────────────────────────────────────────┘
```

### 1.1 Layer 1: Cryptographic Identity (Self-Sovereign Personhood)
- **Zero-Knowledge Validity:** Proof of authenticated presence ([PAP](https://pap.drayker.org)) and credential verification without revealing real-world identities, biometric records, or central registry identifiers.
- **Pairwise Non-Correlation:** Separate interactions utilize distinct cryptographic pairwise keys, mathematically preventing platforms from constructing an omnipresent behavioral dossier.
- **Inalienable Primacy:** Human sovereignty precedes any protocol. An identity cannot be revoked or locked out by automated algorithmic enforcement.

### 1.2 Layer 2: Representative Proxy Agent (Bounded Agency)
- **Delegated Execution:** A member's personal agent ([Dk Personal](https://github.com/draykerdk/dk-personal)) acts as an authorized proxy in network negotiations, assembly coordination, and automated workflows.
- **Strict Bounded Mandates:** Proxies operate under explicit, revocable parameters defined by the member. A proxy cannot commit a member to irreversible constitutional liabilities without active cryptographic sign-off.
- **Instrument vs. Human:** A proxy is a tool for thought and execution. It possesses zero legal, moral, or constitutional personhood within the ecosystem.

### 1.3 Layer 3: Contextual Reputation Clusters (Empirical Lineage)
- **Domain Segmentation:** Reputation is earned through verifiable delivered functions ([DFMP](https://dfmp.drayker.org)). A high reputation in cryptographic auditing grants zero unearned authority in biomedical research or economic parameter design.
- **No Monolithic Social Credit:** UID explicitly prohibits the collapse of multi-dimensional human contributions into a single scalar "social credit" or "worthiness" score.
- **Strict Anti-Financialization:** Reputation cannot be bought, sold, rented, staked for passive return, or transferred. Financial contribution (such as holding or donating Dktron) grants zero reputation and zero voting leverage.

---

## 2. Inalienable Human Safeguards

1. **Vital Floor Independence:** Basic support, access to public knowledge, and participation rights are never contingent upon reputation metrics. Human dignity is not an earned privilege.
2. **Right to Metacognitive Defusion and Privacy:** As detailed in *Do animal à superinteligência*, a person has the absolute right to internal contradiction, doubt, rest, and complete absence from public attribution. Private personal growth is never extracted as network collateral.
3. **Situated Contextual Veto:** The member retains the sovereign right to halt any automated action executed within their immediate bodily, cognitive, or domestic perimeter.

---

## 3. Scope & Non-Scope

### Scope
- Architecture and interfaces for zero-knowledge self-sovereign authentication.
- Bounded delegation protocols between human keys and autonomous proxy agents.
- Specifications for isolated, domain-specific contextual reputation graphs.
- Non-correlatable multi-persona cryptographic signing standards.

### Non-Scope
- Centralized KYC/AML database integration.
- Monolithic credit scoring, surveillance telemetry, or behavioral tracking.
- Tokenized identity NFTs or financialized reputation markets.

---

## 4. Ecosystem Dependencies

- **[`living-cryptography`](https://lc.drayker.org):** Cryptographic primitives, verifiable sortition, and zero-knowledge relation proofs.
- **[`dk-personal`](https://github.com/draykerdk/dk-personal):** The local personal agent executing proxy mandates under human attention sovereignty.
- **[`pap`](https://pap.drayker.org):** Proof of Authenticated Presence verifying living human uniqueness without centralized biometrics.
- **[`value-unit`](https://value.drayker.org):** Strict separation between economic capacity (Dktron) and constitutional voice (UID).

---

## 5. Governance & Contribution

Drayker is an open, primarily volunteer R&D initiative. The current founding-phase governance is documented in [`draykerdk/.github`](https://github.com/draykerdk/.github/blob/master/GOVERNANCE.md). Public proposals follow [DFMP](https://dfmp.drayker.org).

Content licensed [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).
