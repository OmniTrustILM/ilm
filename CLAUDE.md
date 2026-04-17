# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is the **meta-repository** for the ILM (Identity Lifecycle Management) platform (`OmniTrustILM/ilm`). It contains no application source code — only project-level documentation, branding assets, and GitHub issue templates. The actual platform code lives in separate repositories under the [OmniTrustILM](https://github.com/OmniTrustILM) GitHub organization.

## What's Here

- `README.md` — Platform overview, feature list, and links to all component repositories
- `CONTRIBUTING.md` — Contribution guidelines, commit conventions, and development process
- `LICENSE.md` — MIT License
- `logo/` — OmniTrust ILM logo SVGs
- `icon/` — OmniTrust ILM icon SVGs

## Branching Model

Uses [GitHub flow](https://docs.github.com/en/get-started/using-github/github-flow). Feature branches are created from `main` and merged back via pull requests.

## Commit Convention

- Imperative mood, capitalized, max 50 chars for summary
- Blank second line, then optional detailed text wrapped at 72 chars
- Include a `Link:` line referencing the GitHub issue

## Platform Architecture (for context)

ILM is a microservices-based trust lifecycle management platform. Key component repos (all under `OmniTrustILM` org, lowercase with dashes):

- **core** — Central service managing certificate operations, secrets management, and connector orchestration
- **auth** — Access control and user identification (with OPA policies in `auth-opa-policies`)
- **scheduler** — Task automation
- **interfaces** — REST API definitions for building connectors
- **fe-administrator** — Admin web UI
- **cbom-lens / cbom-repository** — Cryptographic Bill of Materials scanning and storage
- **Connectors** — `ejbca-ng-connector`, `hashicorp-vault-connector`, `common-credential-provider`, discovery providers, cryptography providers, etc.
- **helm-charts** — Kubernetes deployment

The technology stack across the platform is primarily Java/Spring Boot (backend) and React (frontend).

## External Resources

- Website: https://www.omnitrust.com
- Documentation: https://docs.otilm.com
- Contact: ilm@omnitrust.com
