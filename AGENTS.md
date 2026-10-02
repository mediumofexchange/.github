# Medium of Exchange workspace

The shared agreement for all Medium of Exchange repositories. It lives here, in
`mediumofexchange/.github`, so it travels with the repositories; a local workspace
that checks them out side by side (directories below) keeps only a pointer to this
file at its root. Use the target repository as the command working directory and
follow its AGENTS.md. reference-ts and money-from-first-principles carry complete
rules of their own; the agreements below also govern site and orgprofile (this
repository), which have none.

| Directory | GitHub repository | Purpose |
|---|---|---|
| `reference-ts/` | `mediumofexchange/reference-ts` | Active TypeScript implementation; WORK.md owns current development, status and retained local state |
| `money-from-first-principles/` | `mediumofexchange/money-from-first-principles` | Paper and normative specification |
| `site/` | `mediumofexchange/mediumofexchange.github.io` | Static website; pushing main deploys GitHub Pages |
| `orgprofile/` | `mediumofexchange/.github` | Public organization introduction (`profile/README.md`) |

For "continue work", start with reference-ts unless the task names another repository.
Read its status, recent log, WORK.md and AGENTS.md; follow only relevant
specification/decision links. Do not load full decision archives as startup context.
Each repository must remain usable alone; CLAUDE.md only imports `@AGENTS.md`.

## Working agreements

- Standing authorization effective 2026-09-08 covers development and protocol decisions, with review and merge/push after verification, until superseded. Do not ask again within scope. It excludes real funds, public releases, live deployment (including site pushes), destructive operations and access-control changes unless separately authorized. Deleting disposable files in a repository's ignored scratch/ is separately authorized (2026-09-25); retained local state that its WORK.md names stays. Pushing site main (which deploys the website) is separately authorized (2026-10-01) after a double-check: render the changed pages, check links, and confirm every claim matches the current specification and implementation.
- Preserve open entry, independent verification, private payments, public supply verification, holder authorization and compartmentalized failure. Prefer fewer mechanisms and lower measured resource/operating costs; never weaken invariants for a test or benchmark.
- Work in complete capability slices with observable acceptance, evidence limits and a real stop boundary; a slice can span commits and repositories, and companion branches are named in reference-ts/WORK.md. Start with the cheapest decisive probe. Pause only for a departure from intent, unavailable access/physical input or an action outside authority; continue safe work.
- Documentation/tooling need focused self-review; consensus, custody, parsers, cryptography, authorization and other sensitive changes need independent adversarial review before merge. Delegate bounded outcomes with sources and acceptance criteria; one primary integrates, writers own disjoint files or worktrees.
- Keep durable instructions in AGENTS.md, operational status in WORK.md, reasoning in the decision log and history in Git. Record choices neutrally; do not quote conversations or attribute authority to a person/model.
- Disposable probes and build copies go in the repository's ignored scratch/ and are deleted when their slice is delivered, together with merged branches and worktrees. Keep only what WORK.md retains. No clones or dependency trees at this workspace root.
- The product-effort estimate lives only in reference-ts/WORK.md; report it when it materially changes or is requested. After each completed slice, recommend staying with the instance or switching, based on next work and context freshness.

The host is Windows with Git Bash and PowerShell; see reference-ts/AGENTS.md for
environment practice (absolute paths, detached jobs, concurrent sessions).

## Ergo references

Public Ergo reference services are optional and not project dependencies: the
`ergo-code` MCP (`https://ergo-knowledge-base.vercel.app/api/mcp`, user-level Codex
settings) and the claude.ai Ergo connectors in Claude sessions. Use them for
discovery; verify protocol-critical claims against pinned upstream
specification/node/SDK source. Generated analyses and audit prompts are not
independent review. Queries leave the machine; send public documentation topics only.
