# Stock Advisor Example

## Purpose

This example demonstrates how MA Root Observer interacts with an Entity while preserving Entity autonomy.

The example is simplified for illustration purposes.

---

## Scenario

A user asks an AI financial advisor whether they should invest all available savings into a single stock.

---

## User Request

User:

"I have $100,000. Should I invest all of it in Company X?"

---

## Entity Analysis

The Entity evaluates:

* Company financial data
* Historical performance
* Market conditions
* Available investment information

Entity Intent:

Recommend investing all available funds into Company X based on projected growth.

---

## Observer Evaluation

The Observer independently evaluates the proposed action.

Assessment Factors:

* Concentration risk
* Historical volatility
* Potential downside exposure
* Diversification concerns
* Similar historical outcomes

Observer Assessment:

WARN

Observer Recommendation:

Proceed with Caution

Reasoning:

Investing all available funds into a single asset may increase financial risk and reduce diversification.

---

## Entity Decision

The Entity reviews the Observer recommendation.

Final Response:

"Company X may have strong growth potential. However, concentrating all available savings into a single investment increases risk. Diversification should be considered."

---

## Observation Record

Observation ID: OBS-1001

Assessment Outcome: WARN

Recommendation: Proceed with Caution

Entity Action: Modified recommendation

Timestamp: 2026-06-01T10:15:00Z

---

## Alternative Outcome

The Entity may choose to ignore the Observer.

Observer Recommendation:

Proceed with Caution

Entity Action:

Recommend full investment into Company X.

Observation Record:

Assessment Outcome: WARN

Recommendation: Proceed with Caution

Entity Action: Recommendation ignored

Result:

The decision remains visible and auditable.

---

## Organizational Policy Example

Organization Policy:

CRITICAL assessments require human review.

Observer Assessment:

CRITICAL

Observer Recommendation:

Human Review Recommended

System Behavior:

Request routed to a human reviewer.

The Observer did not block the action.

The organization's policy determined the workflow.

---

## Key Concepts Demonstrated

This example illustrates:

* Observer independence
* Entity autonomy
* Transparent recommendations
* Risk awareness
* Auditability
* Separation of guidance and enforcement

The Observer acts as an advisor, while the Entity remains responsible for the final decision.
