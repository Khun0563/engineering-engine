# Engineering Engine — Project Contract

## Mission

Build a general-purpose repository engineering engine capable of:

1. Repository analysis
2. Error detection
3. Root-cause diagnosis
4. Safe repair
5. Feature/addition assistance
6. Script generation
7. Validation
8. Regression testing
9. Evidence collection
10. Engineering reporting

## Initial Implementation

M6 React Native / Android is the first real-world validation target.

## Architecture Rule

The engine itself must remain framework-agnostic.

Framework-specific behavior belongs in adapters and rules.

## Repair Policy

### AUTO_REPAIR

Only safe, deterministic, evidence-backed changes.

### REVIEW_REQUIRED

Changes that can affect dependencies, architecture, project behavior, or compatibility.

### BLOCKED

Changes that would require bypassing project requirements, guessing intent, or weakening validation.

## PASS Rule

A project is not considered fixed merely because one command succeeds.

The relevant validation chain must pass.

## Repository Isolation

Engineering Engine must remain independent from the target project.

It must not become a runtime dependency of the Universal ZIP-to-APK Builder.
