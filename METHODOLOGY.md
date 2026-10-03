# CrossingKey Research Methodology

CrossingKey public research is evidence-bound. The purpose of this repository is not to convert every internal idea into a public claim. It is to expose useful questions, experiments, architectures, negative results, and conclusions while preserving uncertainty and protecting private material.

## Source order

Prefer, in order appropriate to the question:

1. official specifications and standards;
2. standards organizations and official protocol repositories;
3. official registries, SDKs, source implementations, and documentation;
4. direct CrossingKey source or observed system behavior;
5. reproducible experiments and test artifacts;
6. authoritative security guidance and peer-reviewed research;
7. credible independent technical analysis;
8. developer issues, discussions, and community evidence as signals rather than proof.

## Research record

A publishable research note should identify:

- the question;
- why it matters;
- evidence class;
- relevant environment and version;
- method;
- observed result;
- competing explanations where material;
- limitations;
- negative evidence;
- conclusion;
- what would falsify or strengthen the conclusion;
- publication date and revision history.

## Evidence classes

**Standards fact**  
Explicitly defined by an authoritative specification.

**Observed result**  
Directly supported by a reproducible experiment, artifact, test, or system output.

**Implementation fact**  
Directly observable in current source or a running implementation.

**Market observation**  
Observed across current services, registries, repositories, packages, or developer activity.

**Community signal**  
Anecdotal evidence useful for identifying a problem or repeated workaround, but insufficient by itself to establish fact.

**Working hypothesis**  
A proposed explanation, architecture, or opportunity not yet demonstrated.

**Experiment**  
A controlled measurable attempt to support or reject a hypothesis.

**Editorial analysis**  
Reasoned synthesis that is explicitly not represented as established fact.

## Claim discipline

Do not silently promote:

- a design into an implementation;
- a prototype into a product;
- a test into production;
- a successful request into a verified business outcome;
- a payment challenge into settlement;
- testnet or simulated settlement into revenue;
- a local file name into proof of a complete system;
- chronology into proof of copying or derivation;
- similarity into causation;
- a planned benchmark into measured performance;
- self-published material into independent validation.

When source material contains stronger language than the evidence supports, the public note must reduce the claim to what can actually be established.

## Negative evidence

Preserve failed tests, incompatible assumptions, abandoned approaches, missing artifacts, and disproven hypotheses when they materially change the conclusion.

A useful research record may conclude:

- not reproduced;
- insufficient evidence;
- implementation incomplete;
- incompatible with current protocol behavior;
- hypothesis rejected;
- promising but unmeasured;
- blocked pending external evidence.

Those are valid outcomes.

## Public-safety review

Before publication, remove or generalize anything that would unnecessarily expose:

- credentials, API keys, tokens, cookies, secrets, private keys, seed phrases, mnemonics, or wallet signing material;
- customer or third-party private information;
- personal addresses, phone numbers, account identifiers, or unnecessary personal records;
- private infrastructure topology, internal hostnames, private IPs, sensitive filesystem locations, or security controls whose disclosure materially increases attackability;
- unpublished exploit detail;
- proprietary datasets or licensed material that cannot be republished;
- private conversations or deeply personal biographical material that is not necessary to establish the technical research claim;
- operational instructions that would convert a research abstraction into an unsafe capability.

Public notes should use synthetic examples or generalized structures when the real data is not necessary.

## Intellectual-property boundary

Publication should expose enough detail to make the research legible and useful without automatically publishing every private implementation artifact.

For archive-backed systems:

1. identify the research question;
2. extract the generalizable architecture or finding;
3. preserve the original status label;
4. remove secrets and unnecessary private context;
5. distinguish specification from implementation;
6. link to public source only when that source is intentionally public;
7. retain private originals outside this repository.

## Research-to-engineering boundary

Use this progression:

`Research → Specification → Implementation → Verification → Production claim`

A project may skip stages only when the evidence genuinely supports doing so. A research repository should not become a backdoor for making production claims that belong in an implementation repository.

## External comparisons

Comparisons with other organizations, products, or later publications must use dated sources and neutral language.

A chronology may establish that CrossingKey material existed before or after another public artifact. It must not infer access, copying, infringement, derivation, or motive without separate evidence.

## Revision policy

Corrections should be explicit. Material errors should be fixed with a commit that states what changed. Historical claims should not be silently strengthened as later systems mature.

## Publication checklist

Before committing a public research note, confirm:

- [ ] the central claim is narrower than or equal to the evidence;
- [ ] status is explicit;
- [ ] implementation and research are separated;
- [ ] sensitive information is absent;
- [ ] personal/private material is unnecessary and removed;
- [ ] third-party claims are sourced or omitted;
- [ ] negative evidence is retained where relevant;
- [ ] no unverified performance number is presented as measured;
- [ ] no prototype is described as production;
- [ ] links point only to intentionally public material;
- [ ] the note remains useful after sanitization.
