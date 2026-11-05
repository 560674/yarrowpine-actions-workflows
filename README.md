# Actions Starter Workflows (Free)

Three small, copy-paste-ready GitHub Actions workflows, linted with `actionlint` and `yamllint`.

| File | What it does |
|---|---|
| `ci.yml` | Node.js and Python test jobs; each skips itself if `package.json` / `requirements.txt` is missing |
| `pr-labeler.yml` | Labels PRs (`documentation`, `ci`, `tests`, `code`) by changed paths, using only the `gh` CLI |
| `release.yml` | Pushing a `v*` tag creates a GitHub Release with auto-generated notes |

## Usage

1. Copy the files you want into `.github/workflows/` in your repo.
2. For `pr-labeler.yml`, create the labels once (or let it fail softly).
3. Push. That's it — no secrets required (uses the built-in `GITHUB_TOKEN`).

```bash
mkdir -p .github/workflows
cp path/to/this/repo/.github/workflows/*.yml .github/workflows/
```

## Want more?

**Pro pack — 16 workflows + docs ($9):** multi-OS/multi-version CI matrix, dependency caching,
multi-arch Docker build & push to GHCR, Dependabot auto-merge, stale bot, Conventional-Commit
semantic releases, scheduled jobs, GitHub Pages deploy, CodeQL, workflow linting, PR-title checks,
npm and PyPI publishing.
(CodeQL is governed by the GitHub CodeQL Terms: free for public repositories; private repositories require GitHub Advanced Security.)

## Notes

- Not affiliated with or endorsed by GitHub. "GitHub" is used only to describe compatibility.
- This project is maintained with AI assistance; every workflow is linted before release.
- License: MIT © 2026 Yarrowpine Studio
