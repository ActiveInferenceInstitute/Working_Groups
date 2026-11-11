# Agent guide — Working_Groups

Public home of the Active Inference Institute Working Groups initiative: draft founding documents and the reviewed position paper Coordinating the Field (doi:10.5281/zenodo.23066904).

## Working notes

- Repository: `ActiveInferenceInstitute/Working_Groups` (default branch `main`).
- InstituteOS classification: category `governance`, maturity `wip`, status `active`.
- License: `CC-BY-4.0`.
- Keep private content in private repositories; never commit credentials,
  personal data, or unverified claims.
- Read [`README.md`](README.md) first, then the nearest nested `AGENTS.md`.
- Prefer small, verified changes; run the declared tasks before handing work back.

## Tasks

| Task | Command | Working directory |
| --- | --- | --- |
| `docs` | `ls docs` | `.` |
| `inventory` | `git ls-files` | `.` |

There is no build or test suite: the repository contains Markdown documents
(`docs/`), the published paper artifacts (`paper/`), and `CITATION.cff`.

## InstituteOS sidecar

This repository carries a committed [`.aii/`](.aii/README.md) sidecar with curated
InstituteOS metadata (`aii-sidecar/v1`): category, maturity, ecosystem relations,
key artifacts, provenance, and portable tasks. It is read by
[InstituteOS](https://github.com/ActiveInferenceInstitute/InstituteOS) tooling and
does not affect the project's build or runtime. Regenerating the sidecar docs
rewrites only `.aii/README.md`, `.aii/AGENTS.md`, `.aii/docs/README.md`,
`.aii/docs/AGENTS.md`, and `.aii/docs/INTEGRATION.md`.
