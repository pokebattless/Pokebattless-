# Security Policy

## Supported Versions

This project is a single-page front-end application. Security fixes are applied to the `main` branch only.

| Version | Supported |
| ------- | --------- |
| `main`  | ✅ |

## Reporting a Vulnerability

If you discover a security vulnerability (e.g. XSS, exposed secrets, unsafe API key handling), please **do not open a public issue**.

Instead:

1. Open a [private security advisory](../../security/advisories/new) on GitHub, **or**
2. Contact the maintainer directly with details of the issue.

Please include:

- A description of the vulnerability
- Steps to reproduce
- Potential impact

We'll do our best to respond and patch within a reasonable timeframe.

## Notes on This Project

- This app calls the Anthropic Claude API directly from the browser for AI narration. No API keys are hard-coded in the client — do not commit real API keys to this repository.
- As a static, client-only app, there is no backend/database attack surface.
