# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Status

This repository has no code yet (no commits, no source files). There are no build, lint, or test commands, and no architecture to describe.

Once the project is scaffolded, re-run `/init` (or update this file by hand) to add:
- Commands for build, lint, test, and running a single test
- A high-level overview of the architecture

## Agent skills

### Issue tracker

Issues are tracked in GitHub Issues for ElvinKukuhN/Brainmatics-edukids, using the `gh` CLI. See `docs/agents/issue-tracker.md`.

### Triage labels

Uses the five default triage labels (`needs-triage`, `needs-info`, `ready-for-agent`, `ready-for-human`, `wontfix`). See `docs/agents/triage-labels.md`.

### Domain docs

Single-context: one `GLOSSARY.md` and `docs/adr/` at the repo root. See `docs/agents/domain.md`.
