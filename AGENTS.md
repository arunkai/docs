# docs

Arun Kai's Notes: a public Mintlify site with posts (`2025/`), about pages and the Mintlify
starter's `essentials/` pages. Navigation and theme live in `docs.json`.

- Shared defaults live in `~/Dev/studio` ([arunkai/studio](https://github.com/arunkai/studio)): start with `agent/defaults.md`. This file overrides them where they differ.
- Read [`LEARNINGS.md`](LEARNINGS.md) before changing build or deploy setup.

## Stack

- Mintlify (`docs.json`, `.mdx` pages, `snippets/`).

## Run, build, deploy

```sh
npm i -g mint
mint dev           # http://localhost:3000
```

Publishing goes through Mintlify's GitHub integration (pushes to the default branch); there's
no deploy script in the repo.

## Rules

- This repo is **public**. Nothing private (accounts, IDs, unreleased work) goes here.
- Every new page needs an entry in `docs.json` navigation.
- No spaces in paths or names (kebab-case). Never commit `.env`, `.dev.vars` or keys; secrets go in `wrangler secret` / Workers Builds variables.
