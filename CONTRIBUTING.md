# Contributing

Engineering Engine is built around evidence, minimal changes, and verifiable results.

## Engineering Rules

### Keep the Core Framework-Agnostic
Framework-specific logic belongs in adapters and rules.

### Prefer Small Changes
Each change should have a clear purpose and a reviewable scope.

### Do Not Weaken Validation
Never remove or bypass a required validation gate simply to obtain a PASS.

### Provide Evidence
Behavior-changing contributions should include appropriate tests or reproducible validation.

### Classify Uncertain Repairs

- `AUTO_REPAIR`
- `REVIEW_REQUIRED`
- `BLOCKED`

## Pull Requests

A useful pull request should describe:

- problem
- evidence
- diagnosis
- proposed change
- validation
- regression result
- known limitations
