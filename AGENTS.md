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

## Layout

| Path | Contents |
| --- | --- |
| [`docs/`](docs/README.md) | Living draft documents: Charter, Operating Procedures, Predecessor Documents |
| [`paper/`](paper/README.md) | Unchanged published paper artifacts (PDF, DOCX, EPUB); do not edit |
| [`README.md`](README.md) | Repository overview, candidate domains, timeline |
| [`CONTRIBUTING.md`](CONTRIBUTING.md) | Comment and change-proposal process |
| [`TODO.md`](TODO.md) | Owner-facing open items |
| [`CITATION.cff`](CITATION.cff) | Citation metadata |
| [`.aii/`](.aii/README.md) | InstituteOS metadata sidecar |

## Documentation conventions

- Documentation lives in Markdown: repository overview in `README.md`, living
  governance documents in [`docs/`](docs/README.md), published snapshots in
  [`paper/`](paper/README.md). There is no separate site generator.
- When you edit a governance document, update its version line and any
  cross-reference in the other `docs/` files that names it.
- Do not edit the files in `paper/`; they mirror the Zenodo publication record.
- Keep relative links valid: check that every path you add resolves from the
  file that contains it.
- The two referenced documents that do not exist yet (Domain Working Group
  Charter Template and AII-POL-IP-001) are described as forthcoming in the
  README and Charter; do not create placeholder files for them.

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
