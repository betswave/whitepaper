# Betswave Whitepaper (v1.1)

This repository hosts the **Betswave Whitepaper v1.1** as a documentation-style site using **MkDocs**.

## Repository Structure

```text
.
├── docs/                     # Whitepaper content (Markdown)
│   ├── index.md
│   ├── executive-summary.md
│   ├── introduction.md
│   ├── market-opportunity.md
│   ├── wave-token.md
│   ├── orca-utility.md
│   ├── legal-disclaimer.md
│   ├── roadmap.md
│   ├── appendix.md
│   └── assets/               # Images/diagrams used in the whitepaper
├── mkdocs.yml                # Site configuration (navigation, theme)
└── requirements.txt          # Python dependencies for MkDocs
```

## Local Setup (Preview)

### Prerequisites

- Python 3.10+ (recommended 3.11)

### Install dependencies

```bash
pip install -r requirements.txt
```

### Run the docs locally

```bash
mkdocs serve
```

Then open: http://127.0.0.1:8000

## Writing Guidelines

- Keep content in `docs/` as Markdown (`.md`) files.
- Prefer clear, factual language (whitepaper tone).
- Avoid repeating the same ideas across multiple sections.
- Add images/diagrams to `docs/assets/` and reference them with relative paths:

```md
![Diagram](assets/diagram.png)
```

## Versioning

- The live content reflects the latest merged changes on the default branch.
- Major updates should be released as tagged versions (e.g., `v1.1`, `v1.2`) to maintain an audit trail.

## Contribution Workflow

- Create a branch per update (e.g., `update-wave-token`, `fix-roadmap-q1`).
- Keep changes focused (one section per PR where possible).
- Use PR descriptions to clearly explain what changed and why.

## Deployment

Deployment to `whitepaper.betswave.io` will be added once content is finalized.
(We will use GitHub Pages + GitHub Actions.)

## Disclaimer

This repository contains informational content for the Betswave whitepaper. It is not financial, legal, or investment advice. Please refer to `docs/legal-disclaimer.md`.

---

Maintained by the Betswave team.
