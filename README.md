# CrossingKey Public Research

**Research into the systems that emerge between human intent and machine action.**

CrossingKey studies what happens when AI moves beyond answering questions and begins participating in sustained work: using tools, carrying context, coordinating actions, interacting with economic systems, and producing outcomes that need to be verified.

The work spans human–AI interaction, agent architecture, persistent context, machine commerce, verification, protocol discovery, local intelligence, structured execution, provenance, and interface design.

## Research programs

### Human–AI Co-Evolution

Repeated work with AI changes the human side of the system too. People learn new forms of abstraction, delegation, verification, and systems thinking; better structure from the human makes the machine more useful in return.

CrossingKey models this as a recursive loop:

`Interact → Observe → Adapt → Compress → Delegate → Verify → Repeat`

One useful concept emerging from the work is **interaction compression**: over time, a smaller amount of language can carry more operational meaning because vocabulary, constraints, roles, and working structures have accumulated.

[Read the Human–AI Co-Evolution Model](research/HUMAN_AI_COEVOLUTION.md)

### Human–AI Interaction Architecture

The interaction itself can be engineered. This research examines intent, context, correction, operator authority, shared vocabulary, tool use, and the transition from isolated prompts toward sustained human-machine work.

### Agentic Systems

How should an agent inspect state, plan, use tools, challenge a proposed action, recover from failure, and know when to stop? This program includes orchestration, bounded execution, state shadowing, recovery, and HAAR.

[Read HAAR](research/HAAR.md)

### Memory, Context & Provenance

Model context is not the same thing as durable memory. CrossingKey research explores persistent state, source-aware retrieval, local ledgers, semantic retrieval, canon-loading, freshness, confidence, and reconstructable context. CCMB and NavigatorFS grew from this line of work.

### Machine Commerce

Software increasingly needs to discover capabilities, understand price and requirements, authorize payment, execute work, reconcile settlement, receive entitlements, and verify fulfillment. CrossingKey studies that transaction as a state machine rather than a single payment event.

Production work in [CrossingKey MCP](https://github.com/crossingkey-holdings/crossingkey-mcp) provides a live engineering counterpart to this research.

### Verification & Evidence

A command being sent is not the same as an outcome being achieved. This program studies read-back verification, receipts, manifests, hashes, state inspection, failure injection, reconciliation, and evidence chains that make machine actions reviewable after the fact.

### Protocol Discovery & Interoperability

How does an agent find a capability, understand it, determine what it costs, learn what it requires, and decide whether it can safely use it? This work follows MCP discovery, registries, capability metadata, quoting, machine-readable requirements, and the missing connective tissue between protocols.

### Local & Private Intelligence

What useful parts of an agent system can live on ordinary hardware? Research includes local models, embeddings, persistence, policy, orchestration, privacy boundaries, constrained compute, and selective cloud/local division of labor.

### XKEY & Structured Execution

XKEY and `.xkey` explore machine-readable ways to carry intent, configuration, provenance, validation, and execution structure between systems. The work spans document formats, parsers, cartridges, command envelopes, and governance-aware execution.

### Evidence-Bearing Operational State

NavigatorFS and related work investigate filesystems and operational records as inspectable evidence: inventories, hashes, logs, receipts, exports, status, validation, and diagnostics that make state easier to reconstruct.

### Applied Verification

CrossingKey also tests these ideas against messy real-world information. Experiments in public-record and property verification, for example, keep physical evidence, official records, permits, supplied claims, and unresolved questions distinct instead of flattening them into one answer.

### Product & Interface Architecture

Human-facing and agent-facing systems both need legible state. This research asks how capability, authority, price, progress, failure, delivery, and proof should appear in an interface when software is doing consequential work.

## Research library

The [Research Index](RESEARCH_INDEX.md) maps the programs, artifacts, and open questions.

The [Research Methodology](METHODOLOGY.md) describes how CrossingKey investigates a question, runs experiments, records evidence, and publishes results.

## Connected work

- [CrossingKey MCP](https://github.com/crossingkey-holdings/crossingkey-mcp) — governed machine-commerce implementation
- [CrossingKey Open Specifications](https://github.com/crossingkey-holdings/crossingkey-open-specifications) — interoperable technical conventions
- [CrossingKey Developer Documentation](https://github.com/crossingkey-holdings/crossingkey-developer-documentation) — engineering guidance
- [Professional evidence](https://github.com/crossingkey-holdings/experience) — implementation and verification record
- [CrossingKey Intelligence](https://crossingkeyintelligence.com)

## Contact

Research, implementation, licensing, and collaboration: **founder@crossingkeyintelligence.com**
