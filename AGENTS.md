# Siftly Agent Instructions

Use `CLAUDE.md` as the detailed project guide. This file is the generic agent entrypoint for non-Claude agents.

## Project summary

Siftly is a self-hosted Twitter/X bookmark manager using Next.js, TypeScript, Prisma, SQLite, and AI-assisted categorization/search.

## Required read order

1. `CLAUDE.md`
2. `README.md`
3. `package.json`
4. `prisma/schema.prisma`
5. Relevant tests under `__tests__/`.

## Safe default commands

```bash
npm run lint
npm run build
npm test
npm run siftly -- stats
```

Run dependency installation only when explicitly needed and approved.

## Boundaries

- Do not commit `.env` or real credentials.
- Do not commit local SQLite databases.
- Do not change OAuth/auth flows without targeted review.
- Do not run external import/sync jobs without user approval.
- This repo is public and forked; avoid unnecessary divergence from upstream.
