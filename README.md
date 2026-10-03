# CrossingKey Public Research

**Public-safe research notes, architecture studies, experiments, and evidence methods from CrossingKey Intelligence.**

This repository is not the documentation mirror for CrossingKey MCP and it is not a single-paper showcase. It is the research surface for questions that sit underneath multiple CrossingKey systems: how humans express intent to machines, how agents retain and qualify context, how autonomous systems prove what happened, how machine commerce survives ambiguous outcomes, how local AI can remain useful under constrained hardware, and how experimental architectures move from hypothesis to evidence.

## Research map

| Program | Central question | Public status |
| --- | --- | --- |
| Human–AI interaction | How should intent, correction, uncertainty, review, and operator authority be represented when AI can act? | Active research |
| Agent execution & orchestration | How can tool-using systems plan, act, challenge their own plans, stop safely, and recover from failure? | Active research |
| Memory, context & provenance | How can persistent context retain origin, freshness, confidence, and auditability without pretending model context is durable memory? | Active research |
| Machine commerce | What state, authorization, reconciliation, entitlement, receipt, and replay controls are needed when software participates in commerce? | Active research + production-informed study |
| Verification & evidence | What evidence is sufficient to distinguish an attempted action from a completed and verified outcome? | Active research |
| Protocol discovery & interoperability | How do agents discover capabilities, understand requirements, compare offers, and cross protocol boundaries without hidden assumptions? | Active research |
| Local/private AI | Which workloads can move toward local models, embeddings, memory, policy, and tooling under real hardware constraints? | Active research |
| Governed languages & execution formats | Can structured documents and execution envelopes make authority, provenance, validation, and intent more inspectable? | Exploratory research |
| Product & interface architecture | How should complex technical capability expose state, price, boundaries, failure, delivery, and proof to humans and agents? | Applied research |

These programs overlap, but they are not aliases for one another.

## Published research

### HAAR: High-Agency Agentic Runtime

[Read the public paper](research/HAAR.md).

HAAR is one research program inside this repository. It proposes a bounded execution architecture built around structured intent, fresh-state inspection, adversarial review, state shadowing, idempotent recovery, stopping rules, and human authority. It is published as research, not as a claim that the complete architecture is deployed or benchmarked.

## Research lineages under review

The CrossingKey archive contains additional documented lines of investigation that are being reduced into public-safe research notes before publication:

- **Human–AI Interaction Architecture:** intent, operator authority, interaction correction, review, escalation, and the transition from conversational assistance toward tool-using systems.
- **CCMB / persistent-context research:** working, transactional, and longer-lived context; source/provenance labels; local persistence; retrieval; and the distinction between loaded state and model memory.
- **NavigatorFS / evidence-bearing state:** integrity inventories, hashes, logs, receipts, exports, validation, diagnostics, and reconstructable local state.
- **XKEY / `.xkey` research:** structured command/document envelopes, validation, governance, execution boundaries, and portable machine-readable intent. Archive material includes prototypes and unverified components, so no runtime-completeness claim is made here.
- **Machine-commerce research:** x402, payment requirements, settlement verification, idempotency, replay prevention, entitlement issuance, receipts, provider state, and ambiguous-outcome reconciliation.
- **Agent discovery research:** MCP discovery, registries, capability metadata, machine-readable requirements, quoting, and the gap between being callable and being safely purchasable.
- **Local-first agent systems:** local models, embeddings, persistent state, policy components, constrained compute, privacy boundaries, and selective use of cloud models.
- **Verification systems:** evidence ledgers, read-back checks, manifests, checksums, receipts, API responses, smoke tests, failure injection, and the question of what constitutes proof of completion.
- **Applied evidence engines:** experiments such as property/public-record verification that separate physical evidence, official records, permit evidence, and marketing claims rather than collapsing them into a single confidence statement.

A lineage appearing here means there is archive evidence of research or experimentation. It does **not** mean every named system is complete, deployed, validated, commercially available, or suitable for public source release.

## Research boundary

This repository publishes conclusions and abstractions, not the private archive.

Public material must not include credentials, private customer information, personal records, private infrastructure topology, wallet secrets, seed material, unpublished security-sensitive implementation detail, proprietary datasets, or personal biographical material that is unnecessary to the technical claim.

Names from experimental archives are not treated as proof of implementation. Where source material describes a component as proposed, recovered, prototype, specified, unverified, or incomplete, the public record preserves that uncertainty.

## Evidence classes

- **Standards fact:** explicitly defined by an authoritative specification or standards source.
- **Observed result:** directly supported by a reproducible experiment, artifact, test, or system output.
- **Implementation fact:** directly observable in source or a running implementation.
- **Market observation:** observed across current services, registries, repositories, or developer activity.
- **Community signal:** useful evidence of a problem or pattern, but insufficient alone to establish fact.
- **Working hypothesis:** a proposed explanation, design, or opportunity that still requires testing.
- **Experiment:** a controlled attempt to support or reject a hypothesis.
- **Editorial analysis:** reasoned synthesis, clearly separated from established fact.

## Publication rule

Research moves toward publication through:

`Question → Evidence → Classification → Experiment or Analysis → Limitations → Public-safe Note`

It moves toward engineering only when the evidence supports that transition:

`Research → Specification → Implementation → Verification → Production claim`

Those stages must not be collapsed.

## Start here

- [Research index](RESEARCH_INDEX.md)
- [Research methodology](METHODOLOGY.md)
- [HAAR](research/HAAR.md)

## Related public surfaces

- Production MCP implementation: https://github.com/crossingkey-holdings/crossingkey-mcp
- Open specifications: https://github.com/crossingkey-holdings/crossingkey-open-specifications
- Developer documentation: https://github.com/crossingkey-holdings/crossingkey-developer-documentation
- Professional evidence: https://github.com/crossingkey-holdings/experience
- Company: https://crossingkeyintelligence.com

## Contact

Research, technical, licensing, or collaboration inquiries: **founder@crossingkeyintelligence.com**
