# Contributing to TinkeringDao

Contributions to the `TinkeringDao` organization profile and project index must comply with [`LEGAL.md`](LEGAL.md), [`CODE_OF_CONDUCT.md`](CODE_OF_CONDUCT.md), and the 6-stage autonomous workflow defined in [`docs/agents/autonomous-pipeline.md`](docs/agents/autonomous-pipeline.md).

## Pull Request Standards

1. **Branch Isolation**: Create a topic branch from `main` (`feat/*`, `fix/*`, `docs/*`, `chore/*`).
2. **Cryptographic Commit Signing**: Author all commits as `TinkeringDao <203040288+TinkeringDao@users.noreply.github.com>` with `ED25519` SSH signing enabled.
3. **Structured PR Body**: Include `## Summary`, `## Evidence`, and `## Merge Danger` (`Door: two-way | one-way`, `Blast Radius: local | module | system`).

### Verification Checklist & Pre-Merge Gate Commands

Every Pull Request is automatically audited by [`.github/workflows/autonomous-pr-review.yml`](.github/workflows/autonomous-pr-review.yml). Run these commands locally before opening or updating a PR:

| Gate | Requirement | Local Pre-Merge Command |
| :--- | :--- | :--- |
| **Gate 1: OPSEC & Zero-PII** | Zero personal identifiers, local usernames, postal codes, or coordinates in repo tree | `grep -rnI -iE "<FORBIDDEN_PII_PATTERN>" . --exclude-dir=.git --exclude="*autonomous-pr-review.yml"` (see workflow) |
| **Gate 2: Cryptographic Signatures** | Every commit signed with `ED25519` SSH key (`verified == true`) | `git log -1 --show-signature` |
| **Gate 3: Legal & Autonomous Spec** | `LEGAL.md` (with German Statutory Addendum), `LICENSE`, `SECURITY.md`, `CODE_OF_CONDUCT.md`, `CODEOWNERS`, `AGENTS.md`, `CLAUDE.md`, `docs/agents/autonomous-pipeline.md` present | `grep -q "Addendum: German Statutory References" LEGAL.md && test -s docs/agents/autonomous-pipeline.md` |
| **Gate 4: Workflow & Syntax** | All GitHub Actions workflows and markdown indices validate cleanly | `python3 -c 'import yaml, glob; [yaml.safe_load(open(f)) for f in glob.glob(".github/workflows/*.yml")]'` |
