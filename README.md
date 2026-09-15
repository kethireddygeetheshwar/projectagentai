# Project Agent AI

An early-stage AI-assisted project workspace exploring how an agent can turn a software idea into a structured development plan.

## Current status

This repository is intentionally a small prototype. It is not presented as a production-ready autonomous coding agent.

## Goals

- Turn a product idea into explicit requirements and tasks.
- Break tasks into implementation steps and acceptance criteria.
- Keep generated plans reviewable by a human developer.
- Eventually connect planning with repository-aware development workflows.

## Planned architecture

```text
Idea
  ↓
Requirement extraction
  ↓
Task / acceptance-criteria generation
  ↓
Human review
  ↓
Implementation workflow
  ↓
Tests + validation
```

## Engineering principles

- Human approval before consequential changes.
- Generated output is treated as untrusted input.
- Secrets stay outside source control.
- Tests should accompany executable functionality.
- Small, observable steps are preferred over unrestricted autonomous changes.

## Roadmap

- [ ] Define a stable Python package structure
- [ ] Add typed request/response models
- [ ] Add deterministic planning tests
- [ ] Add an LLM provider abstraction
- [ ] Add prompt and output validation
- [ ] Add repository context ingestion
- [ ] Add a CLI for generating plans
- [ ] Add CI for tests and linting

## Contributing

Keep changes focused, document behavior, and add tests for executable functionality. Do not commit API keys, access tokens, or private project data.

## License

License will be added when the project's first reusable implementation is published.
