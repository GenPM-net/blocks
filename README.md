# @core/blocks

[![genpm](https://api.genpm.net/v1/badge/@core/blocks.svg)](https://genpm.net/p/@core/blocks) ![license](https://img.shields.io/badge/license-MIT-blue)

> Page builder blocks: 15 accessible sections (hero, pricing, FAQ with JSON-LD…), admin editor and registry for more

A [GenPM](https://genpm.net) module: **source code + AI rules + MCP config**, injected into your project instead of hidden in `node_modules`. The code lands in `src/lib/blocks`, pinned to a verified commit, and you own it.

## Install

```bash
genpm add @core/blocks
```

No genpm yet? `curl -fsSL https://genpm.net/install.sh | sh` (macOS/Linux), `irm https://genpm.net/install.ps1 | iex` (Windows), or one-off with `npx @genpm-net/cli add @core/blocks`.

Or let your AI agent do it: run `genpm mcp setup` once, then ask *"add @core/blocks with genpm"* in Claude Code, Cursor, VS Code, Windsurf, Codex or Gemini CLI. It shows you a dry-run plan before writing anything.

## What it does

Page sections that editors combine from the admin: hero, features, benefits, testimonials, logos, pricing, FAQ (with
FAQPage JSON-LD), call to action, gallery, video, stats, comparison, guarantee, rich text and form. Each block is a
zod schema + editor fields + a React component. Other packages and kits add their own blocks (product grid, latest
posts…) to the same registry. Blocks are stored as JSON inside @core/content entries; no tables of its own.

## At a glance

- **GenPM dependencies** (installed with it): [@core/db](https://genpm.net/p/@core/db), [@core/contracts](https://genpm.net/p/@core/contracts), [@core/rich-text](https://genpm.net/p/@core/rich-text), [@core/media](https://genpm.net/p/@core/media), [@core/ui](https://genpm.net/p/@core/ui), [@core/admin](https://genpm.net/p/@core/admin)
- **npm dependencies** (proposed, never installed without asking): `react`, `zod`
- **AI rules**: [`AGENTS.md`](AGENTS.md), loaded by your agent only when it works in `src/lib/blocks`

## Security

GenPM installs a 40-character commit SHA (never a branch), verifies an Ed25519-signed manifest, never runs install scripts and scans AI rules for prompt injection. Details: [genpm.net/docs/security](https://genpm.net/docs/security).

## License

MIT — see [LICENSE](LICENSE). Browse the full catalog at [genpm.net](https://genpm.net).
