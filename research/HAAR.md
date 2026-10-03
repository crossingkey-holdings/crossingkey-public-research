# HAAR: High-Agency Agentic Runtime

**A proposed architecture for bounded, verifiable AI execution**

CrossingKey Intelligence | crossingkey_

## Summary

HAAR is a design for agent runtimes that translate an authorized task into structured execution, check the state of the environment, constrain retries, and verify the result. It is a research and engineering proposal. The public description does not claim that the full runtime is implemented or that its performance targets have been measured.

## The problem

An agent can report that it sent a command without knowing whether the intended outcome occurred. Long conversations can also carry stale assumptions into new tasks. Repeated attempts may duplicate effects when the result of an earlier attempt is uncertain. HAAR treats these as execution problems that require explicit state, evidence, and stopping rules.

## Design principles

1. **Structured intent.** Normalize the operator's objective, allowed actions, inputs, and completion criteria before execution. “Direct Binary Injection” is the working name for this structured handoff; it does not require literal binary encoding.
2. **Fresh state.** Check relevant files, APIs, and services at the time of action. Retain past context only when it is deliberately selected and verified.
3. **Adversarial review.** Use distinct planning, risk, and synthesis perspectives for consequential decisions. A separate model call is a design choice, not an inherent requirement.
4. **State shadowing.** Record the relevant state before a mutation, specify the expected outcome, then inspect actual state afterward.
5. **Idempotent recovery.** Use operation identifiers and reconciliation so uncertain results can be investigated without blindly repeating effects.
6. **Bounded attempts.** Stop when a retry budget is exhausted or new attempts cease to produce evidence. Preserve the last verified state and escalate the unresolved decision.
7. **Human authority.** Publishing, sending, spending, deleting, changing permissions, and other consequential actions require the operator's defined approval.

## Execution outline

`Authorize → Normalize → Inspect → Plan → Review → Execute → Verify → Record or Escalate`

Each stage should emit enough evidence to explain what was attempted, what changed, and what remains uncertain. A successful tool response alone is not proof of the intended business result.

## Current status

This document presents the architecture and a proposed evaluation program. It is not a performance benchmark, audited security design, production deployment claim, or substitute for transaction-specific safety controls.

## Evaluation agenda

- Compare elapsed time and resource consumption against a conventional conversational workflow on the same tasks.
- Measure incorrect completion claims, duplicate side effects, and recovery from ambiguous outcomes.
- Test whether adversarial review reduces consequential errors without unacceptable cost or latency.
- Verify that stopping rules preserve evidence and allow a human to resume safely.

Publish measured results separately, with task definitions, environment, baselines, and failure cases.

## Relationship to CrossingKey MCP

HAAR is a research architecture. CrossingKey MCP is a separately versioned implementation surface for governed machine commerce. They share engineering concerns including explicit authorization, idempotency, state verification, reconciliation, receipts, entitlements, and bounded execution, but publication of HAAR does not claim that the MCP implements the full HAAR architecture.

- CrossingKey MCP: https://github.com/crossingkey-holdings/crossingkey-mcp
- Professional evidence: https://github.com/crossingkey-holdings/experience

## Rights and contact

Copyright © 2026 Jeremy Paul Allen. All rights reserved. This document is available for reading and discussion; no software or commercial license is granted by its publication.

Research, licensing, or implementation inquiries: **founder@crossingkeyintelligence.com**
