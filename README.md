# Engineering Engine

A repository engineering, analysis, repair, extension, validation, and automation engine.

## Purpose

Engineering Engine is designed to analyze software repositories, detect problems, identify root causes, propose or apply safe fixes, add required functionality, generate engineering scripts, run validation, and produce evidence-based reports.

## Initial Target

Version 0.1 starts with the M6 React Native / Android build-validation problem from the Universal ZIP-to-APK Builder project.

The React Native implementation is the first adapter, not the permanent scope of the engine.

## Core Workflow

Analyze → Detect → Diagnose → Plan → Repair → Verify → Regression Test → Report

## Safety Principles

- Preserve project intent and architecture.
- Prefer minimal, evidence-based changes.
- Never bypass required build/runtime gates just to obtain a PASS.
- Never silently change major dependencies or architecture.
- Protect existing local/project work.
- Every repair must be verifiable.
