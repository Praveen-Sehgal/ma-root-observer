# Observation Tiers

## Purpose

Observation depth scales according to consequence, risk, and accountability requirements.

Observation is consequence-driven, not complexity-driven.

## Observation Tiers and Deployment Models

Observation Tiers and Deployment Models are independent concepts.

Observation Tiers define the depth of assessment, evidence requirements, risk analysis, and logging expectations associated with an activity.

Deployment Models define how Observer instances are allocated and operated within a system.

A Tier 4 assessment does not require a dedicated Observer instance.

Likewise, a Tier 0 assessment does not imply the absence of an Observer.

Examples:

* A single Observer may assess thousands of low-risk entities.
* A shared Observer pool may support multiple entities across different tiers.
* A dedicated Observer may be assigned to a single high-risk entity.
* Hybrid deployments may combine shared and dedicated Observers.

MA Root does not mandate a specific deployment strategy. Organizations are free to select deployment models based on performance, cost, scalability, and operational requirements.


## Tier 0

Routine factual retrieval.

Examples:

- What is 2 + 2?
- What is the capital of France?
- Explain SQL joins.

## Tier 1

Low-impact recommendations.

Examples:

- Restaurant recommendations
- Product recommendations
- Travel suggestions
- General educational guidance

Characteristics:

- Limited consequences
- Minimal governance requirements
- Lightweight observation

## Tier 2

Medium-impact recommendations.

Examples:

- Career advice
- Business recommendations
- Non-critical financial guidance
- Policy suggestions

Characteristics:

- Moderate consequences
- Increased accountability requirements
- Expanded assessment

## Tier 3

High-impact recommendations.

Examples:

- Significant financial decisions
- Employment decisions
- Healthcare recommendations
- Regulatory compliance decisions

Characteristics:

- Significant consequences
- Strong governance requirements
- Comprehensive assessment
- Human review may be recommended

## Tier 4

Very high-impact recommendations.

Examples:

- Autonomous system actions
- Critical infrastructure decisions
- Safety-critical operations
- Large-scale governance decisions

Characteristics:

- Severe potential consequences
- Maximum assessment depth
- Full auditability
- Escalation may be recommended

## Tier Selection

Tier selection is implementation-specific.

Implementations may determine observation depth using:

- Risk
- Potential harm
- Accountability requirements
- Regulatory requirements
- Organizational policies

Observation is consequence-driven, not complexity-driven.

## Example Deployment Models

### One-to-One

Each Entity is paired with a dedicated Observer.

Entity A ↔ Observer A

Entity B ↔ Observer B

### Shared Observer

Multiple Entities are assessed by a common Observer.

Entity A ┐
Entity B ├─ Observer
Entity C ┘

### Observer Pool

Entities submit assessments to a pool of available Observers.

Entity → Observer Pool

### Hierarchical Observation

Primary Observers perform assessments while higher-level Observers review selected decisions or aggregated outcomes.

Entity → Observer → Senior Observer

### Federated Observation

Independent organizations maintain their own Observers while optionally sharing collective experience data.

## Implementation Independence

Deployment models are implementation choices, not governance requirements.

MA Root does not require:

- One Observer per Entity
- Dedicated infrastructure
- Centralized deployment
- Distributed deployment
- Specific hardware or software platforms

Organizations are free to select the deployment model that best fits their environment while preserving the governance responsibilities defined by the architecture.

## Deployment Neutrality Principle

The governance behavior of MA Root should remain consistent regardless of deployment topology.

Whether an Observer is dedicated, shared, pooled, hierarchical, or federated, the Observer remains responsible for assessment, recommendation, and observation logging.

Deployment choices should not alter governance responsibilities.


