# Documentation Structure

This folder contains the project documentation used during delivery.
Keep content concise, versioned with the codebase, and aligned with `.github/copilot-instructions.md`.

## Core Files

- `business-process-hierarchy.md`: project-local copy of the process hierarchy used by documentation workflows.
- `product_requirements_document.md`: business goals, scope, stakeholders, and high-level requirements.
- `technical_specifications.md`: implementation choices, integration details, technical constraints, and non-functional requirements.

## Subfolders

- `adr/`: Architecture Decision Records. Use it to capture significant technical or solution decisions with rationale and consequences.
- `design/`: solution design material such as architecture notes, diagrams, sequence flows, and component decomposition.
- `specs/`: detailed functional or technical specifications that guide implementation.
- `user/`: user-facing guides, operating instructions, and support material.
- `minutes/`: meeting minutes. Create one file per meeting when the documentation scaffold is enabled.
- `minutes/recap/`: short recap documents distilled from detailed meeting minutes.
- `bbp/`: business blueprint outputs and structured analysis deliverables.

## Usage Guidelines

1. Put stable reference documentation in the most specific folder available.
2. Keep architecture decisions in `adr/`; avoid burying them inside generic design notes.
3. Store working session notes in `minutes/`, then promote confirmed outcomes into PRD, technical specs, ADRs, or BBP artifacts.
4. Keep diagrams, assumptions, and interface details in `design/` or `specs/` instead of scattering them across multiple files.
5. Keep `business-process-hierarchy.md` aligned with the project scope discussed in workshops.
6. Update this folder when project scope, architecture, or delivery decisions materially change.

## Notes

- Some folders are optional and are created only when the corresponding scaffold pack is enabled.
- Pandoc defaults, templates, and Avanade assets remain bundled in the plugin skills; they are no longer copied into the target repository.
- Use US English unless the project explicitly requires a different documentation language.
