# github-actions-templates

Reusable GitHub Actions composite actions. Each action lives in its own
subdirectory and is referenced as
`uses: chimeranext/github-actions-templates/<action>@main`. Starter workflows
for each action are in `.github/workflows/`.

## Actions

- `prds-check` — validates PR descriptions per PRDS audit checks (Summary /
  Tracker / Test plan / Scope boundaries). Starter: `.github/workflows/prds.yml`.
- `codeowners-replicate` — replicates the canonical CODEOWNERS SSOT from the
  governance repo to target repos (MPH point 8). Starter:
  `.github/workflows/codeowners-replicate.yml`.
- `security-scan` — standardized CodeQL (SAST) + Trivy (config/fs/secret)
  scan. Used by the assurance `security.yml` workflow (CIS standard).

Make this repo a template so clients can "Use this template".
