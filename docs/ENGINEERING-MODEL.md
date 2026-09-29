# Engineering Model

Engineering Engine treats software repair as an evidence-driven process.

## Finding

A finding identifies an observed problem.

A finding should contain:

- identifier
- location
- observed evidence
- severity
- affected component
- reproducibility

## Diagnosis

Diagnosis explains the likely root cause based on evidence.

A diagnosis must distinguish:

- Observed
- Inferred
- Unknown

Unknown information must never be silently converted into assumptions.

## Repair Plan

A repair plan describes:

- intended change
- affected files
- expected effect
- risk
- repair classification
- verification method
- regression requirements

## Repair Classes

### AUTO_REPAIR

Deterministic and evidence-backed changes that can be safely automated.

### REVIEW_REQUIRED

Changes that require human review because they may affect dependencies, architecture, behavior, or project intent.

### BLOCKED

Cases where safe progress is impossible without guessing, weakening validation, or bypassing requirements.

## Verification

Verification must test the requirement that originally failed.

A repair is not complete merely because a command exits successfully.

## Regression

Regression testing protects previously working behavior.

The engine should record:

```text
Before
  ↓
Change
  ↓
After
  ↓
Regression Result

## Report

Reports should provide enough evidence for another engineer to understand and reproduce the conclusion.
```
