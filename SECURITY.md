# Security

Engineering Engine operates on software repositories and may eventually automate repository modifications.

## Security Principles

- Never expose secrets in logs.
- Never commit credentials or tokens.
- Treat repository contents as untrusted input.
- Avoid unnecessary command execution.
- Keep automated repairs bounded and deterministic.
- Require review for high-risk changes.
- Preserve evidence needed to audit repairs.

## Untrusted Repositories

A repository may contain malicious scripts, unexpected build hooks, arbitrary dependency code, misleading configuration, or sensitive information.

Automation must not assume repository code is trusted.

## Reporting

Reports should avoid exposing tokens, passwords, private keys, authentication cookies, or unrelated personal data.

Sensitive values should be redacted before persistence or reporting.
