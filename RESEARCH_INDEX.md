# CrossingKey Research Index

CrossingKey research sits at the intersection of interaction design, agent architecture, state, verification, commerce, and local computing. This index is a map of the work and the questions connecting it.

## Human–AI Co-Evolution

**Core idea:** the useful unit of capability is not only the human or the model, but the evolving interaction between them.

Repeated interaction can teach the human to express systems through better abstractions, delegate through objectives and constraints, and verify machine work against observable evidence. Those changes improve the structure presented to the AI, which changes what can be accomplished in the next cycle.

**Model:** `Interact → Observe → Adapt → Compress → Delegate → Verify → Repeat`

**Key concept:** interaction compression.

**Artifact:** [Human–AI Co-Evolution Model](research/HUMAN_AI_COEVOLUTION.md)

Related work: Human–AI Interaction Architecture, persistent context, Navigator, verification.

## Human–AI Interaction Architecture

**Focus:** designing the boundary between intention and machine capability.

Questions include how intent is represented, how context accumulates, how corrections alter future work, how authority remains with the operator, and how shared vocabulary changes the bandwidth of interaction.

Related concepts include navigation, structured intent, interaction compression, persistent context, and governed execution.

## Agent Execution & Orchestration

**Focus:** the runtime surrounding a capable model.

Research covers planning, tool use, state inspection, adversarial review, bounded retries, postcondition verification, escalation, and recovery from ambiguous outcomes.

**Published artifact:** [HAAR: High-Agency Agentic Runtime](research/HAAR.md)

## Memory, Context & Provenance

**Focus:** making useful context persistent, attributable, retrievable, and inspectable.

Research threads include CCMB, local ledgers, semantic retrieval, working versus longer-lived state, provenance labels, freshness, confidence, and canon-loading.

A recurring architectural distinction is simple: persisted state can be loaded and inspected; conversational familiarity alone is not persistence.

## Machine Commerce

**Focus:** economic interaction between software systems.

The research decomposes a machine purchase into discovery, requirements, quote, authorization, payment, settlement, execution, fulfillment, entitlement, receipt, and reconciliation.

This line directly informs the public [CrossingKey MCP](https://github.com/crossingkey-holdings/crossingkey-mcp).

## Verification & Evidence

**Focus:** proving outcomes rather than merely recording attempts.

Methods explored across CrossingKey work include read-back checks, manifests, checksums, receipts, API responses, health checks, state inspection, persistent ledgers, failure injection, and reconciliation.

The deeper question is how an autonomous system can leave enough evidence for a human or another machine to reconstruct what actually happened.

## Protocol Discovery & Interoperability

**Focus:** the path from capability existence to capability use.

Research follows MCP discovery, registries, capability descriptions, machine-readable requirements, quoting, compatibility, and the information an agent needs before deciding whether to invoke or purchase something.

## Local & Private Intelligence

**Focus:** useful agent infrastructure under real hardware constraints.

This work explores local models, embeddings, persistence, policy components, orchestration, storage, latency, privacy, and hybrid local/cloud execution on consumer hardware.

## XKEY & `.xkey`

**Focus:** structured, portable representations of machine intent and execution context.

The XKEY lineage explores documents, parsers, cartridges, command envelopes, validation, provenance, configuration, and governance-aware execution.

Research questions include which information should travel with an executable instruction, where validation ends and policy begins, and how an execution document can remain inspectable across runtimes.

## NavigatorFS & Evidence-Bearing State

**Focus:** treating operational state as something that can be inspected and reconstructed.

The lineage includes integrity inventories, file hashes, relative paths, modification records, logs, receipts, exports, validation, status, and diagnostic operations.

It connects filesystem design to the larger CrossingKey interest in provenance and verification.

## Applied Verification

**Focus:** keeping unlike forms of evidence unlike.

Public-record and property-verification experiments explored how physical observations, official records, permit evidence, supplied claims, and unresolved questions can be gathered into one workflow without erasing their different evidentiary weight.

The pattern generalizes to due diligence, technical verification, research synthesis, and agent-generated reports.

## Product & Interface Architecture

**Focus:** making complex systems understandable at the moment of action.

Research includes how interfaces communicate capability, authority, price, state, progress, failure, delivery, and proof to both humans and software agents.

## Provenance & Chronology

**Focus:** preserving the development record of technical ideas and artifacts.

Dates, version history, hashes, manifests, commits, timestamps, and original artifacts make it possible to reconstruct how a system developed and compare versions without relying entirely on retrospective narrative.

## Current publication path

The strongest candidates for the next standalone research notes are:

1. persistent context and provenance;
2. machine-commerce state and reconciliation;
3. verification as an execution primitive;
4. capability discovery before payment;
5. local-first agent architecture on constrained hardware;
6. XKEY and structured execution;
7. evidence-bearing operational state.

See [METHODOLOGY.md](METHODOLOGY.md) for the research process.
