# MA Core Interfaces
This document defines the core contracts used by MA Core. MA Core does not implement a specific AI model, Observer, storage system, or enforcement mechanism. It defines stable interfaces that allow Entities, Observers, Collective Experience stores, and Assessment Frameworks to interoperate.

## Core Concept

MA Core is interface-first.

The framework defines relationships between:

- Entity
- Observer
- Governance Principles
- Assessment Framework
- Collective Experience
- Observation Log

Implementations may use different AI models, databases, scoring systems, storage layers, or policies as long as they respect the MA Core contracts.

## MA Core Contracts

The primary contracts are:

- IEntity
- IObserver
- IGovernancePrinciples
- IAssessmentFramework
- ICollectiveExperience
- IObservationLog

MA Core does not prescribe implementation details.

Implementations may use:

- AI models
- Rule engines
- Databases
- Event streams
- Search systems
- External services

as long as they satisfy the MA Core contracts and governance principles.

## IEntity

An Entity is any system capable of making decisions or performing actions.

Examples include:

- Large Language Models (LLMs)
- AI Agents
- Workflow Engines
- Business Process Systems
- Human Decision Systems

Entities retain decision authority.

An Entity may:

- Accept Observer recommendations
- Ignore Observer recommendations
- Override Observer recommendations

Entity actions and outcomes should be recorded for transparency and accountability.

## IObserver

An Observer is an independent assessment component attached to an Entity.

The Observer is responsible for assessing actions, generating recommendations, and recording observations.

The Observer does not make decisions on behalf of the Entity.

The Observer may:

- Analyze requests
- Evaluate potential impacts
- Assess risks
- Generate recommendations
- Generate warnings
- Record observations
- Maintain audit history
- Reference Collective Experience
- Apply Governance Principles
- Apply Assessment Frameworks

The Observer may not:

- Execute actions
- Override Entity decisions
- Enforce organizational policies
- Make final decisions

The Observer is advisory by design.

Decision authority remains with the Entity or governing organization.

The Observer exists to provide transparency, accountability, guidance, and auditability without removing Entity autonomy.

Observer assessments may be used by external policy systems, human reviewers, or organizational workflows, but the Observer itself remains an assessment component.

## IGovernancePrinciples

Governance Principles provide foundational guidance used by Observers during assessment.

Governance Principles establish the baseline standards that Observers must consider when evaluating actions and outcomes.

Governance Principles may include:

- Regulatory requirements
- Industry standards
- Accountability requirements
- Risk management principles
- Transparency requirements
- Auditability requirements

MA Core does not prescribe a specific set of Governance Principles.

Implementations may obtain Governance Principles from recognized standards bodies, regulatory frameworks, industry groups, organizations, or other trusted sources.

Governance Principles are intended to provide a stable foundation for assessment while allowing implementation flexibility.

## IAssessmentFramework

The Assessment Framework provides the methods and models used by an Observer to evaluate actions and outcomes.

Assessment Frameworks may evaluate:

- Risk
- Harm
- Impact
- Compliance
- Historical outcomes
- Long-term consequences

MA Core does not prescribe specific assessment methodologies, formulas, scoring systems, or weighting models.

Implementations may use deterministic rules, statistical models, machine learning systems, domain-specific frameworks, or other evaluation mechanisms.

Assessment results are intended to support Observer recommendations and observations while preserving Entity autonomy.

## ICollectiveExperience

Collective Experience provides access to historical observations, outcomes, patterns, and lessons learned.

Collective Experience enables Observers to reference prior actions and their outcomes when performing assessments.

Collective Experience may include:

- Historical observations
- Historical outcomes
- Distilled patterns
- Shared lessons learned
- Similar prior assessments
- Historical action-outcome relationships

MA Core does not prescribe how Collective Experience is stored, distributed, or maintained.

Implementations may use databases, event streams, knowledge stores, distributed networks, or other mechanisms.

Collective Experience is intended to improve future assessments through accumulated experience while preserving implementation flexibility.


## IObservationLog

The Observation Log records observations, recommendations, decisions, and outcomes.

Observation Logs support transparency, accountability, traceability, and auditability.

Recorded information may include:

- Request summary
- Observer assessment
- Recommendations
- Entity decisions
- Outcomes
- Timestamps

MA Core does not prescribe specific storage technologies or retention policies.

Implementations may use immutable logs, databases, event streams, distributed ledgers, or other storage mechanisms.


