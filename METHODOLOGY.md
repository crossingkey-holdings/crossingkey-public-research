# CrossingKey Research Methodology

CrossingKey research usually begins with a practical systems problem: an agent reports success without proving the outcome, context disappears between environments, a payment crosses several independent states, a protocol exposes a capability without making it understandable to another machine, or a local system behaves differently from its architectural model.

The research process turns those failures and questions into artifacts that can be inspected.

## The working loop

`Question → Inspect → Model → Experiment → Observe → Compare → Refine → Publish`

### Question

State the problem narrowly enough that evidence can change the answer.

### Inspect

Read the relevant specification, source, runtime state, logs, prior artifacts, and external implementations. Establish what is already known before designing a new abstraction.

### Model

Describe the system in terms of its important states, boundaries, actors, transitions, and failure modes. Diagrams, schemas, state machines, interface contracts, and small prototypes are often more useful here than prose alone.

### Experiment

Build the smallest useful test. Keep the environment, versions, inputs, and expected observations recoverable.

### Observe

Record what happened, including failures and unexpected behavior. Where the result depends on external state, inspect that state directly.

### Compare

Compare the observation with the hypothesis, specification, baseline, or competing architecture.

### Refine

Change the model when the evidence requires it. A failed idea that reveals the actual boundary of a system is useful research.

### Publish

Turn the result into the artifact best suited to it: research note, experiment record, schema, specification, implementation, benchmark, or engineering guide.

## Evidence vocabulary

CrossingKey research uses a small vocabulary to keep unlike evidence from being flattened together.

**Standards fact** comes directly from an authoritative specification.

**Implementation fact** is visible in source or a running implementation.

**Observed result** comes from an experiment, artifact, test, or direct system output.

**Market observation** describes behavior visible across current services, registries, repositories, or developer activity.

**Community signal** identifies a pattern worth investigating.

**Working hypothesis** is an idea that has not yet earned a stronger label.

**Experiment** is an attempt to change that.

**Analysis** connects the evidence and explains why it matters.

## Verification

The verification method depends on the claim.

Software behavior may require tests plus state inspection. A deployment may require a live endpoint and version evidence. A transaction may require external settlement state. A file may require hashes and provenance. A historical claim may require dated original artifacts. A performance claim requires a measured environment and baseline.

CrossingKey favors evidence that can survive the conversation in which it was produced.

## Negative results

Failed tests, incompatible assumptions, abandoned approaches, and missing evidence are part of the record when they change what the system teaches us.

Some of the most useful findings are boundaries: a protocol does not expose the expected primitive, a retry is unsafe after an ambiguous external result, a local model cannot satisfy the workload on available hardware, or an architectural component exists only as a specification.

## From research to implementation

Research can produce several different things:

`Research → Note / Experiment / Specification / Prototype → Implementation → Verification`

Not every research direction needs to become software. Some become vocabulary, interface conventions, test methods, or better questions.

## Publication

Public research is edited from the working archive rather than copied wholesale. The published artifact contains the technical idea, evidence, method, and useful context needed to understand it. Operational credentials, private records, and unrelated personal material remain outside the research publication.

Corrections and meaningful revisions are preserved through version history.

## Reproducibility

When practical, a research artifact should leave enough information to reconstruct:

- the question;
- environment and relevant versions;
- inputs;
- method;
- expected observation;
- actual observation;
- artifacts produced;
- limitations;
- conclusion.

The goal is simple: make the work inspectable enough that the next person can challenge it, reproduce it, extend it, or build from it.
