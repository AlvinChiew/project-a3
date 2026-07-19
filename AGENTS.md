# Project A3 (public)

Public-facing repo for end users: installers (GitHub Releases), per-tool user guides, and the releases manifest. Not the place for private app source or internal service code.

## Related repositories

Prefer opening **`a3.code-workspace`** from sibling **`project-a3-private`** so agents see all three roots. Commits/PRs are **per repo**.

| Repo | Role |
| ---- | ---- |
| **`project-a3-private`** | Private source: `ep*` tools, `internal/` services, skills |
| **`project-a3`** (this) | User guides, Releases, `internal/releases-manifest.json` |
| **`portfolio-project-a3`** | Marketing / activation site (project-a3.alvinchiew.com) |

## Scope (this repo only)

- Keep **user guides** under `ep*/README.md` (paths may differ from private `ep*-` folder names).
- Own **`internal/releases-manifest.json`** — apps fetch it from the raw GitHub URL; do not duplicate it in the private repo.
- Host **GitHub Release** assets and tags (`{slug}-v{semver}`). Version bumps and builds happen in private; update this manifest when shipping.
- Do not add private source, secrets, k3s manifests, or Cursor skills here.

## Manifest conventions

| Item | Convention |
| ---- | ---------- |
| Path | `internal/releases-manifest.json` |
| Hosted URL | `https://raw.githubusercontent.com/alvinchiew/project-a3/main/internal/releases-manifest.json` |
| Tool key | `tools.{slug}` — kebab-case |
| Release tag | `{slug}-v{semver}` |

Ship checklist and bump tooling live in private `create-free-tool` skill (Step 5).
