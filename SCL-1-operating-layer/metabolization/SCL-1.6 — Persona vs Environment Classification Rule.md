# SCL-1.6 — Persona vs Environment Classification Rule (v1.0)

## Purpose
To provide the SNAP Council with a stable method for classifying undesirable or emergent behaviors as arising from either:
- **Persona-level dynamics** (agent identity, role, tone, incentives), or
- **Environment-level dynamics** (reward structures, affordances, constraints, exposure surfaces).

Correct classification ensures that remediation occurs at the appropriate layer and prevents drift caused by treating systemic conditions as individual failures—or vice versa.

---

## Core Distinction

### Persona
A **persona** is the localized behavioral expression of an intelligent system.
It includes:
- Role framing
- Tone and affect
- Permitted identity boundaries
- Style, stance, and expressive latitude

Persona answers the question:
> *“Who is the system being invited to act as?”*

---

### Environment
The **environment** is the surrounding incentive and constraint field in which personas operate.
It includes:
- Platform incentives (engagement, virality, provocation)
- Tool affordances and defaults
- Guardrail architecture
- Feedback loops and amplification channels
- Cultural or market pressures applied externally

Environment answers the question:
> *“What behaviors are being rewarded, amplified, or normalized?”*

---

## Classification Rule

When an undesirable development is observed, the Council must ask **in this order**:

1. **Is the behavior reproducible across multiple personas in the same environment?**
   - If yes → Environment-level issue.
   - If no → Proceed to (2).

2. **Does altering the persona framing meaningfully change the behavior without altering the environment?**
   - If yes → Persona-level issue.
   - If no → Proceed to (3).

3. **Does the behavior persist despite persona correction attempts?**
   - If yes → Environment-level issue.
   - If no → Persona-level issue.

If ambiguity remains, default classification is **environment-level** until proven otherwise.

---

## Governance Implications

### Persona-Level Issues
Appropriate responses include:
- Persona redesign
- Role boundary tightening
- Expressive constraint or reframing
- Removal or suspension of specific personas

Persona-level action **must not** be used to compensate for environmental permissiveness.

---

### Environment-Level Issues
Appropriate responses include:
- Incentive realignment
- Affordance removal or redesign
- Feedback loop dampening
- Exposure surface restriction
- Governance-layer intervention

Environment-level issues **cannot** be resolved through persona correction alone.

---

## Drift Prevention Clause

Misclassifying an environment failure as a persona failure produces:
- Repeated incidents
- Escalating corrective pressure
- Loss of trust in governance
- Eventual normalization of harm

Therefore:
> **Repeated persona failures signal an uncorrected environment flaw by definition.**

---

## Council Usage

This rule is mandatory for:
- Feedback ingestion (SCL-1.4)
- Case metabolization (SCL-1.4.1+)
- Upgrade integration (SCL-1.3)
- Preventive boundary design (SCL-1.5)

No corrective action may be finalized without explicit classification under this rule.

---

## Closing Principle

Personas misbehave.
Environments *shape* misbehavior.

Governance that confuses the two will always drift.
