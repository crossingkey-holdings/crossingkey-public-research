# CrossingKey Research Index

This index maps public research programs and documented research lineages. It intentionally distinguishes **published research**, **active research**, **exploratory work**, and **archive-backed lineages awaiting public-safe reduction**.

A named research direction is not automatically a shipped product, production capability, benchmark result, or claim of novelty.

## 1. Human–AI interaction

Research questions:

- How should an operator's intent, scope, constraints, and completion criteria be represented?
- How should systems expose uncertainty instead of masking it with fluent output?
- How should correction change system behavior without silently changing authority?
- Which actions may be autonomous, automated, assisted, or manual?
- How should retrieved or generated content remain subordinate to operator authority?

Archive evidence includes a documented Human–AI Interaction Architecture lineage and later governed-agent interaction work. Public publication should focus on technical interaction patterns rather than private biographical origins.

**Status:** active; additional public note planned.

## 2. Agent execution, orchestration & recovery

Research questions:

- What belongs in the runtime around a model rather than in a prompt?
- When does adversarial or multi-perspective review improve consequential decisions?
- How should retries be bounded?
- How should state be inspected before and after mutation?
- How should ambiguous outcomes stop or reconcile before another side effect occurs?

Published work:

- [HAAR: High-Agency Agentic Runtime](research/HAAR.md)

**Status:** active.

## 3. Memory, context & provenance

Research questions:

- What is the difference between model context, persisted state, and durable memory?
- How should stored context identify where it came from?
- How should freshness and confidence affect retrieval?
- How can local persistence reduce unnecessary disclosure to remote systems?
- How can an operator reconstruct why a piece of context influenced an action?

Archive-backed lines include CCMB concepts, source-qualified memory records, local ledgers, semantic retrieval, canon-loading, and state/evidence stores. Some source documents contain aspirational implementation claims; those are not reproduced as established facts.

**Status:** archive-backed research lineage; public note pending.

## 4. Machine commerce & economic state

Research questions:

- How should agents discover paid capabilities without spending?
- What separates quote, authorization, payment, settlement, execution, fulfillment, entitlement, and receipt?
- How should idempotency and replay protection behave around external settlement?
- What should happen when payment state is uncertain?
- What evidence allows a buyer, seller, or agent to verify fulfillment?

CrossingKey MCP provides a production-informed implementation surface, while this repository studies the underlying problems independently of any single release.

**Status:** active research + implementation feedback.

## 5. Verification, evidence & failure analysis

Research questions:

- What counts as evidence that an operation actually completed?
- When are logs sufficient, and when is external read-back required?
- How should failed experiments and negative results be preserved?
- Can a system reconstruct the chain from request through authority, action, resulting state, and verification?
- How should destructive recovery tests be designed without converting test settlement into revenue claims?

Methods under study include manifests, hashes, receipts, API responses, health checks, smoke tests, state inspection, persistent ledgers, failure injection, and reconciliation.

**Status:** active.

## 6. Protocol discovery & interoperability

Research questions:

- Where do agents discover MCP servers and capabilities?
- Which metadata helps an agent decide whether a capability is usable?
- How should requirements, price, expected result, authorization state, and payment methods be exposed before execution?
- Which gaps exist between protocol registration, discoverability, interoperability, and actual successful use?
- Which missing primitives are repeatedly rebuilt across agent systems?

**Status:** active.

## 7. Local/private AI & edge operation

Research questions:

- Which workloads can run usefully on consumer hardware?
- What belongs locally: models, embeddings, memory, policy, verification, or orchestration?
- How should quantization, memory, storage, latency, privacy, maintenance, and fallback be evaluated together?
- When is selective cloud use preferable to forcing every workload local?

No claim is made that local operation automatically provides privacy, accuracy, security, or adequate performance.

**Status:** active/applied.

## 8. Governed languages & execution formats

Archive-backed work includes XKEY and `.xkey` concepts around structured documents, command envelopes, validation, governance, cartridges, parsing, and execution.

The archive contains components marked recovered, prototype, specified, unverified, or incomplete. Accordingly, this repository does not claim a complete language implementation, compiler, runtime, or production deployment.

Research questions:

- Can intent be represented in a portable, inspectable structure before execution?
- Which fields should bind authority, provenance, expected effects, and validation?
- Where should parsing stop and policy enforcement begin?
- How can a structured execution document remain useful across runtimes?

**Status:** exploratory/archive-backed; formal public note pending.

## 9. Evidence-bearing filesystems & operational state

NavigatorFS and related archive material explore the idea that operational state should be inspectable as evidence rather than treated as invisible application internals.

Research themes include integrity inventories, relative-path records, size and modification metadata, hashes, logs, receipts, exports, validation, status, and diagnostics.

**Status:** archive-backed research lineage.

## 10. Applied public-data verification

CrossingKey experiments include evidence-first engines that gather public records and keep evidence classes separate. One documented property-verification experiment distinguished official parcel/GIS records, physical or imagery evidence, permit evidence, and supplied marketing claims, and generated both operator evidence and client-safe output.

The research interest is broader than the individual domain: how to prevent heterogeneous evidence from being flattened into a single unsupported conclusion.

**Status:** applied experimental research.

## 11. Product & interface architecture

Research questions:

- How should complex technical systems explain scope, state, price, delivery, failure, and verification?
- How should interfaces reveal what the machine may do versus what it is authorized to do?
- How can technical capability become a bounded offer without overstating maturity?
- Which interface conventions make agent-facing and human-facing commerce understandable at the same time?

**Status:** applied research.

## 12. Provenance & chronology

Research and engineering artifacts are preserved with dates, hashes, manifests, version history, or other evidence where available. Chronology can establish that a document or concept existed by a certain point when the underlying evidence supports it.

Chronology alone does not establish independent invention, external access, copying, legal ownership, infringement, or causal influence.

**Status:** ongoing evidence practice.

## Publication queue

The next public notes should be selected by evidence quality, technical value, and publication safety rather than by how dramatic an internal project name sounds.

Candidate subjects:

1. persistent context and provenance;
2. machine-commerce state and ambiguous settlement;
3. verification as an execution primitive;
4. capability discovery before payment;
5. local-first agent architecture under constrained hardware;
6. governed execution documents and XKEY/`.xkey` research.

Every note must pass [METHODOLOGY.md](METHODOLOGY.md) before publication.
