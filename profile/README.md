# Open Engineering Definition

**Define what it means to be Open Engineering.**

<p align="center">
  <img src="../assets/hero-banner.png" alt="Open Engineering Definition" width="100%" />
</p>

Open Engineering Definition is the normative foundation of the **Open Engineering** ecosystem.

It establishes the principles, requirements, vocabulary, and conformance criteria that determine when an engineering system, artifact, process, or implementation can meaningfully be called **Open Engineering**.

> **Definitions say what must be true. Implementations decide how to make it true.**

---

## Why a Definition?

Open source has taught us that access to source code matters.

Engineering requires more.

A modern engineered system can span software, hardware, infrastructure, data, models, automation, documentation, decisions, simulations, AI agents, operational state, and physical artifacts. Publishing one repository does not necessarily make that system understandable, reproducible, modifiable, interoperable, or independently operable.

Open Engineering therefore treats openness as a **property of the engineering system as a whole**.

The Open Engineering Definition provides a shared contract for that property.

It makes Open Engineering:

- **explicit** rather than implied;
- **testable** rather than aspirational;
- **machine-readable** where practical;
- **technology-independent** at the definition layer;
- **implementable** by multiple independent projects;
- **evolvable** through versioned definitions;
- **auditable** through evidence and conformance.

---

## Definition, Not Implementation

This organization owns the **definition** of Open Engineering.

It does not prescribe one mandatory implementation.

```text
Open Engineering Definition
            │
            │ defines
            ▼
   principles + semantics
   rules + requirements
   conformance criteria
            │
            │ implemented by
            ▼
    Open Engineering systems
            │
            ├── software
            ├── infrastructure
            ├── hardware
            ├── documentation
            ├── automation
            ├── AI
            └── physical systems
```

This separation is deliberate.

A definition should remain stable enough to become a contract while implementations remain free to innovate.

---

## The Four Dimensions

Open Engineering is considered across four complementary dimensions.

### 1. Ontology

**What things mean.**

The ontology establishes the shared concepts and relationships used to describe engineering systems.

It enables humans, software, and AI agents to reason about engineering artifacts using common semantics rather than relying on application-specific interpretations.

### 2. Product Model

**What the engineered thing is.**

The Product Model represents the composition, structure, identity, interfaces, dependencies, behavior, constraints, and lifecycle of an engineered product or system.

It connects intent to realizable engineering artifacts.

### 3. Systems of Record

**Where authoritative engineering truth lives.**

Open Engineering requires engineering knowledge to have explicit, addressable, versionable sources of truth.

These may include repositories, registries, catalogs, models, evidence stores, decision records, telemetry systems, and other authoritative records.

### 4. Runtime Architecture

**How the engineered system exists and behaves when running.**

The Runtime Architecture connects definitions and models with operational reality.

It covers deployed components, execution, events, messaging, state, observability, orchestration, infrastructure, and interaction with the physical world.

Together:

```text
Ontology
   │
   ▼
Product Model
   │
   ▼
Systems of Record
   │
   ▼
Runtime Architecture
   │
   ▼
Evidence
```

Open Engineering closes the loop between **meaning, design, implementation, operation, and evidence**.

---

## Core Principles

An Open Engineering system should strive to be:

### Open

The information required to understand, reproduce, modify, operate, and evolve the system is available under appropriate open terms.

### Explicit

Important engineering knowledge is represented explicitly rather than hidden inside tooling, undocumented conventions, or individual knowledge.

### Inspectable

A human or machine can inspect how the system is constructed, configured, and operated.

### Reproducible

A sufficiently equipped independent party can recreate the relevant engineering result from its declared sources.

### Modifiable

The preferred forms used to create the system are available so that the system can genuinely be changed.

### Composable

Engineering capabilities can be assembled into larger systems through explicit contracts and interfaces.

### Interoperable

Meaning and interfaces should not unnecessarily depend on a single vendor, application, runtime, or proprietary representation.

### Traceable

Engineering decisions and transformations can be followed from intent through implementation to operational evidence.

### Versioned

Definitions, artifacts, interfaces, decisions, and relevant state have identifiable versions.

### Evidence-Based

Claims about an engineering system should be capable of being supported by inspectable evidence.

### Automatable

Where practical, engineering definitions and rules should be machine-readable so humans and machines can participate in the same engineering process.

### Independently Operable

Openness should permit meaningful independence from the original creator or a single service provider.

---

## Preferred Source

Open Engineering distinguishes an engineering artifact from its **preferred source for modification**.

A rendered diagram is not necessarily its source.

A container image is not necessarily its source.

A compiled binary is not necessarily its source.

A generated configuration is not necessarily its source.

An API response is not necessarily its source.

Where modification requires an upstream representation, that representation forms part of the engineering source.

This principle applies beyond software—to models, diagrams, infrastructure, hardware, simulations, documentation, workflows, media, and other engineering artifacts.

---

## Engineering as a Graph

Open Engineering does not treat engineering as a collection of isolated files.

It treats engineering as an interconnected graph of identifiable things:

```text
Requirement
    │
    ▼
Definition
    │
    ▼
Model ───────► Decision
    │              │
    ▼              ▼
Artifact ◄──── Evidence
    │
    ▼
Deployment
    │
    ▼
Runtime
    │
    ▼
Observation
    │
    └──────────────► Investigation
                         │
                         ▼
                       Change
```

The graph should remain navigable across tools and lifecycle stages.

This enables both engineers and AI systems to answer questions such as:

- What is this?
- Why does it exist?
- Who or what owns it?
- Which definition governs it?
- What does it depend upon?
- How was it produced?
- Which decision introduced it?
- Where is its preferred source?
- What version is running?
- Does the implementation conform?
- What evidence supports that claim?
- What changed?

---

## Machine-Readable Engineering

Documentation for humans remains essential.

But Open Engineering also recognizes that engineering is increasingly performed by **humans and machines together**.

Definitions should therefore be machine-readable wherever doing so improves interoperability, validation, automation, composition, or reasoning.

```text
Human-readable
     +
Machine-readable
     +
Executable where appropriate
     =
Open Engineering
```

This allows definitions to become more than prose.

They can become inputs to:

- validators;
- parsers;
- rules engines;
- generators;
- builders;
- CI/CD systems;
- policy engines;
- digital twins;
- AI assistants and agents;
- runtime controllers;
- observability systems.

---

## Definitions and Conventions

Open Engineering distinguishes between **definitions** and **conventions**.

A **definition** establishes meaning and requirements.

A **convention** establishes an agreed way of representing or applying that meaning.

```text
Definition
    ↓
Convention
    ↓
Parser
    ↓
Rule
    ↓
Implementation
    ↓
Evidence
```

This separation allows conventions and technologies to evolve without casually changing the underlying engineering semantics.

---

## Conformance

Open Engineering should be capable of being assessed.

Conformance is therefore based on declared requirements and evidence rather than branding or self-identification alone.

A conforming implementation should be able to identify:

1. the Open Engineering Definition version it targets;
2. the applicable requirements;
3. its implementation of those requirements;
4. permitted exceptions or extensions;
5. evidence supporting its conformance claims.

The long-term goal is to make as much conformance verification as practical **automatable and reproducible**.

---

## Definitions Are Versioned

Engineering evolves.

So does Open Engineering.

Definitions are therefore versioned artifacts.

```text
definition
├── identity
├── version
├── semantics
├── requirements
├── rules
├── relationships
├── conformance
└── references
```

An implementation should be able to declare which version of a definition it implements.

This protects both stability and evolution.

---

## Open Engineering Ecosystem

The Definition is the foundation for a wider ecosystem.

```text
                 Open Engineering
                       │
                 ┌─────▼─────┐
                 │ Definition │
                 └─────┬─────┘
                       │
          ┌────────────┼────────────┐
          ▼            ▼            ▼
     Definitions   Conventions     Rules
          │            │            │
          └────────────┼────────────┘
                       ▼
                    Parsers
                       │
                       ▼
                   Capsules
                       │
                       ▼
                  Composers
                       │
                       ▼
                     Picos
                       │
                       ▼
               Runtime Systems
                       │
                       ▼
                    Evidence
```

The Definition answers **what Open Engineering means**.

The rest of the ecosystem turns that meaning into working engineering systems.

---

## Humans + AI

Open Engineering is designed for an era in which engineers increasingly collaborate with AI.

That makes explicit engineering semantics even more important.

An AI agent should not need to infer the architecture of a system exclusively from thousands of loosely related files. It should be able to discover definitions, identities, relationships, rules, decisions, interfaces, evidence, and preferred sources directly.

The same properties that make engineering understandable to AI also make it more understandable to humans.

Open Engineering therefore does not create a separate engineering world for AI.

It makes the existing engineering world **more explicit**.

---

## Technology Independence

The Definition intentionally avoids requiring a single technology stack.

An implementation might use technologies such as Git, containers, Kubernetes, Crossplane, databases, message brokers, digital twins, semantic models, or AI agents.

Those are implementation choices.

The Definition instead specifies the properties those implementations must provide.

```text
Definition → stable intent

Implementation → replaceable technology
```

This distinction is fundamental to preventing Open Engineering itself from becoming another form of technology lock-in.

---

## Relationship to Open Source

Open Engineering builds upon the achievements of open-source software, open hardware, open standards, open data, and open design.

It does not replace them.

Instead, it asks a broader systems question:

> **What must be open for an engineered system itself to remain understandable, reproducible, modifiable, interoperable, and independently operable throughout its lifecycle?**

Software licensing is part of that answer.

It is not the entire answer.

---

## What Belongs Here?

Repositories in the `open-engineering-definition` organization should concern the normative definition and its supporting materials, including:

- principles;
- terminology;
- semantic models;
- requirements;
- conformance criteria;
- schemas;
- definition lifecycle;
- governance;
- examples and reference material;
- validation specifications.

Technology-specific implementations should live elsewhere unless they serve directly as normative or reference material for the Definition.

---

## A Simple Test

A useful question for any Open Engineering system is:

> **Could another capable engineer—or engineering AI—discover what this is, understand why it exists, obtain its preferred source, reproduce it, modify it, operate it, verify it, and continue its evolution without depending on undocumented knowledge or a single proprietary environment?**

The closer the answer is to **yes**, the closer the system is to Open Engineering.

---

## The Goal

Open Engineering is not openness for its own sake.

The goal is engineering knowledge that can survive:

- organizations;
- individual engineers;
- applications;
- vendors;
- infrastructure generations;
- AI models;
- technology cycles;
- and time.

Engineering knowledge should be capable of becoming **shared, executable, inspectable infrastructure**.

That begins with defining what we mean.

# Define openly. Engineer openly.
