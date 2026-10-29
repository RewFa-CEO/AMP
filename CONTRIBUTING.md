# Contributing to AMP

Thanks for helping improve AMP. This file covers what you need to know to make a good first PR.

## Dev setup

```bash
git clone https://github.com/RewFa-CEO/AMP.git
cd AMP
npm install
npm run build
npm test
```

The TypeScript core lives in `src/`, the MCP + REST server in `mcp/`, the Python implementation in `python/`, and the browser extension in `extension/`.

## Tests

- TypeScript: `npm test` (Jest, `tests/`)
- Python: `cd python && python -m pytest tests/`

Please add or update a test for any behavior change. PRs that break the suite will not be merged.

## Good first contributions

- Docs fixes (typos, unclear wording, missing steps) — always welcome
- New storage backends or provider options behind the existing `StorageProvider` interface
- MCP tool surface improvements (keeping the tools consistent across TS and Python)

## Honesty policy

The README's Roadmap separates "implemented" from "planned" (vector retrieval, graph tier). Please keep docs and implementation aligned in both directions: don't advertise what isn't shipped, and don't undersell what is.

## Reporting issues

Open an issue with: what you ran, what you expected, what happened, and the storage backend you used (File / SQLite / Redis). Reproduction steps beat stack traces.
