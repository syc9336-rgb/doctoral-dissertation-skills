# Doctoral Dissertation Skills

A modular collection of Agent Skills for doctoral-dissertation planning, writing,
integration, restructuring, evidence auditing, language revision, and finalization.

[![skills.sh](https://skills.sh/b/syc9336-rgb/doctoral-dissertation-skills)](https://skills.sh/syc9336-rgb/doctoral-dissertation-skills)
[![Latest Release](https://img.shields.io/github/v/release/syc9336-rgb/doctoral-dissertation-skills?display_name=tag&sort=semver)](https://github.com/syc9336-rgb/doctoral-dissertation-skills/releases/latest)
[![Apache-2.0](https://img.shields.io/github/license/syc9336-rgb/doctoral-dissertation-skills)](LICENSE)

> This Skill does not invent dissertation content. It turns real research materials into an auditable, restructurable, and submission-ready dissertation workflow.

## Try it first

After installation, enter this prompt in Codex, Claude Code, or another agent that supports Agent Skills:

```text
Use the doctoral-dissertation skill.
Read the real project materials first and build a Frozen Facts Table,
Claim–Evidence Matrix, and RQ Closure Matrix.
Do not inherit cases, samples, variables, or research structures from a previous project.
Then rebuild the dissertation structure from the available evidence.
```

## Install in one command

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills \
  --skill doctoral-dissertation --yes --copy
```

Current skill:

- `doctoral-dissertation` — an end-to-end dissertation production and audit workflow.

This repository is released under the **Apache License 2.0**, which permits use,
copying, modification, redistribution, forking, integration, and commercial use
subject to the license terms.

## Repository layout

```text
doctoral-dissertation-skills/
├── LICENSE
├── NOTICE
├── README.md
├── README_EN.md
├── CONTRIBUTING.md
├── CHANGELOG.md
├── CITATION.cff
└── skills/
    └── doctoral-dissertation/
        ├── SKILL.md
        ├── README.md
        ├── README_EN.md
        ├── tasks/
        ├── references/
        └── examples/
```

Each top-level directory under `skills/` is intended to be an independently
installable Skill unit.

## Installation

List available skills:

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills --list
```

Install the dissertation skill:

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills \
  --skill doctoral-dissertation --yes --copy
```

Install globally for Codex:

```bash
npx skills add syc9336-rgb/doctoral-dissertation-skills \
  --global --agent codex --skill doctoral-dissertation --yes --copy
```

Manual Codex installation:

```bash
git clone https://github.com/syc9336-rgb/doctoral-dissertation-skills.git
mkdir -p ~/.codex/skills
cp -R doctoral-dissertation-skills/skills/doctoral-dissertation ~/.codex/skills/
```

Keep the full skill directory. `SKILL.md` depends on the accompanying
`tasks/`, `references/`, and `examples/` files.

## Good for

- Rebuilding dissertation structure from real research materials;
- Defining chapter, section, and paragraph boundaries;
- Closing the loop between research questions, evidence, and claims;
- Organizing literature review, theory, and research design;
- Separating and integrating methods, results, and discussion;
- Auditing figures, appendices, footnotes, citations, and multilingual versions;
- Running integrity and consistency checks before defense or submission.

## Feedback and contributions

Issues, [Discussions](https://github.com/syc9336-rgb/doctoral-dissertation-skills/discussions),
pull requests, sanitized case studies, and derivative development are welcome.
When reporting feedback, include the task, input-material type, expected result,
actual result, and whether the case can be reproduced publicly.

## Core design philosophy

- Evidence outranks the planned outline.
- Original research facts outrank later prose.
- Chapters solve major problems; sections solve sub-problems; subsections establish judgments.
- Final body prose presents the finished scholarly state, not author revision history.
- Methods investigate questions rather than preset desired results.
- Limitations are concentrated instead of scattered defensively.
- Rigor should not become habitual over-hedging.
- Every central conclusion must have an evidence anchor.
- Major revisions trigger a global consistency scan.

## Contributing

Issues, pull requests, forks, and derivative development are welcome.
See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Apache License 2.0. See [LICENSE](LICENSE) and [NOTICE](NOTICE).

