# CLAUDE.md

This file provides guidance for AI assistants working in this repository.

## Repository Overview

This is a minimal static HTML project in early development. Currently it contains a single HTML file (`index.htm`) with no build system, package manager, or testing framework configured.

## Project Structure

```
mission/
├── .gitignore      # Pre-configured for Node.js/frontend tooling
├── CLAUDE.md       # This file
└── index.htm       # Main HTML entry point
```

## Current State

- **Language**: HTML (plain static)
- **Framework**: None
- **Build system**: None
- **Package manager**: None
- **Tests**: None configured
- **CI/CD**: None configured

## Development Workflow

### Serving the project

Since there is no build step, the HTML file can be served directly:

```bash
# Python (if available)
python3 -m http.server 8080

# Node.js (if available)
npx serve .
```

### Making changes

Edit `index.htm` directly. No compilation or build step is required.

## Git Conventions

- **Main branch**: `master`
- **Claude-generated branches**: follow the pattern `claude/<task>-<session-id>`
- Commit messages should be clear and descriptive
- Git is configured to sign commits using SSH key at `/home/claude/.ssh/commit_signing_key.pub`

## Future Development Notes

The `.gitignore` is pre-configured for common Node.js/frontend tooling, indicating this project may grow to include:

- A JavaScript framework (Next.js, Nuxt, SvelteKit, Gatsby, etc.)
- TypeScript
- Vite or another bundler
- ESLint / Prettier for linting and formatting
- A test framework (Jest, Vitest, etc.)

When these are added, update this file with:
- Install instructions (`npm install` / `pnpm install` / etc.)
- Build commands
- Test commands
- Lint/format commands
- Environment variable requirements

## Key Conventions

- Keep changes minimal and focused
- Do not add dependencies or tooling unless explicitly requested
- If expanding the project, update this CLAUDE.md to reflect the new setup
