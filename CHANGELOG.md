# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.1.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.1.0] - 2026-08-13

### Added

- `pre_tool_call` hook: transparently activates mise for every `terminal()` command when a mise config file is present.
- `on_session_start` hook: trusts the nearest mise config on startup for frictionless activation.
- `pre_llm_call` hook: injects bundled `context.md` as additional context into every LLM turn.
- Bundled `mise` skill covering manual activation, `mise exec`, tasks, installs, and trust.
- CI workflow (lint via ruff + ty, test via pytest) with SHA-pinned actions.
- Release workflow: tag-on-merge pipeline with PyPI trusted publishing (OIDC, no tokens).
- CHANGELOG.md.
