# Terroir Whitepaper

This repository contains the **published whitepaper document package** for Terroir.

## Contents

- `content/whitepaper/document.en.json` - canonical English whitepaper content
- `content/whitepaper/summary.ka.json` - Georgian summary metadata and labels
- `content/whitepaper/supporting.json` - citations, figures, tables, and equations metadata
- `public/downloads/terroir-trace-shield-whitepaper.pdf` - release PDF
- `public/whitepaper/figures/*.svg` - whitepaper figure assets

## Layout Contract

The directory layout is intentionally website-compatible:

- `content/whitepaper/...`
- `public/downloads/...`
- `public/whitepaper/figures/...`

This allows direct reuse by the Terroir website and related tooling without path rewrites.

## Update Workflow

1. Update source whitepaper content/assets in the main Terroir website repository.
2. Run whitepaper validation there:

```bash
node scripts/check-whitepaper.mjs
```

3. Copy release artifacts into this repository preserving paths.
4. Commit and push to `main`.

## Scope

This repo is **documents/artifacts only**. It does not contain website runtime code.
