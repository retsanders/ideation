# CLAUDE.md

This file provides guidance for AI assistants working in this repository.

## Repository Purpose

This repository serves two purposes:
1. **Exploring Claude Code capabilities** — specifically when used from the mobile app
2. **Tracking vibe-coded app ideas** — a place to log ideas and develop POC implementations

The repository is in an early stage. Expect it to evolve as new projects and experiments are added.

## Current State

- Minimal structure: only a `README.md` exists
- No build system, test framework, or CI/CD pipeline has been established yet
- Each new project or POC may introduce its own tech stack

## Development Conventions

Since this repository is expected to host multiple independent POCs and experiments, follow these conventions:

### Directory Structure
- Place each POC or app idea in its own subdirectory (e.g., `projects/app-name/` or `ideas/app-name/`)
- Keep a brief description of each idea in the directory's own `README.md`
- Avoid putting unrelated files at the root level

### Adding New Projects
When starting a new POC:
1. Create a subdirectory with a descriptive name (kebab-case)
2. Add a `README.md` describing the idea, goal, and tech choices
3. Initialize the project's own tooling (e.g., `package.json`, `pyproject.toml`) inside that subdirectory
4. Do not mix dependencies from different projects at the repo root

### Commits
- Use clear, imperative commit messages (e.g., `Add ideation notes for chat app POC`)
- Keep commits focused — one logical change per commit
- Branch off `main` for new features or experiments; use descriptive branch names

## Working with Claude Code (Mobile)

This repo is used to test Claude Code from the mobile app. Keep the following in mind:
- Prefer self-contained tasks that don't require multi-step human intervention
- Document assumptions clearly so context can be rebuilt across sessions
- Prefer simple, readable implementations over clever ones — mobile sessions may be shorter

## Notes for AI Assistants

- There is no linter, formatter, or test runner configured yet — don't assume they exist
- If adding code, choose a language/framework appropriate to the specific POC, not a one-size-fits-all default
- When in doubt about structure, ask before creating new top-level files or directories
- Do not generate placeholder or stub files unless asked
