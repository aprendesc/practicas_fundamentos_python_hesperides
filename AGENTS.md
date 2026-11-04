# Hespérides — Fundamentos de Python practice

## Purpose and context

This repository provides Fundamentos de Python classes and practice notebooks for Hespérides. It reuses the teaching organization of the Deep Learning practice project, not its subject content. The [Hespérides corpus](/Users/alejandroprendes/Desktop/projects/hesperides/AGENTS.md) holds teaching assignments and source notes.

## Key definitions

- **Student edition:** executable public class material and unsolved practice.
- **Teacher edition:** private solutions, narration and preparation.
- Programming syntax and semantics are subject matter; visual models must reflect actual discrete execution.

## Repository map

- [practicas](practicas/): student `clases_sincronas/` and `tareas/`.
- [profesor](profesor/): private class and exercise editions.
- [profesor/resources/documentacion](profesor/resources/documentacion/): class sources, concept map and design records.
- `profesor/resources/notas/`, `medios/`, `scripts/` and `cache_datos/`: local teaching resources.
- [pyproject.toml](pyproject.toml) and [uv.lock](uv.lock): independent execution environment.

## Planning and stakeholders

[Planning panel](https://github.com/users/aprendesc/projects/6)

- `aprendesc`: lecturer, author and repository maintainer.
- Paola Serracchiani: academic coordination and operational support.
- Students: users of the teaching materials.

## Methodologies and references

Choose contracts by the issue's main purpose, not by supporting scripts. Use [coding-contract-guidelines](/Users/alejandroprendes/.codex/skills/coding-contract-guidelines/SKILL.md) for software implementation, [documental-contract-guidelines](/Users/alejandroprendes/.codex/skills/documental-contract-guidelines/SKILL.md) for authored documents, and [general-contract-guidelines](/Users/alejandroprendes/.codex/skills/general-contract-guidelines/SKILL.md) for organization, administration and class preparation, recording, delivery or review without a principal manuscript. Each contract lives in `context/issues/<issue>/`; documentary prose and figures belong inside that issue. Preserve requirements, decisions, pauses and historical evidence. Real supporting validators may stay beside any task without turning it into a software feature. Global functional scenarios remain in `context/tests/`.

[`development-methodology`](/Users/alejandroprendes/.codex/skills/development-methodology/SKILL.md).
Use the local [sync_lesson_generator](profesor/resources/skills/sync_lesson_generator/SKILL.md) for the teaching format and class construction.

Keep teacher solutions and guidance private. Preserve manual edits when rebuilding. Existing student notebooks do not prove institutional publication. Chapter-specific timing, cell counts and builder details belong to the class documentation.

Local clone safeguards and configuration: [.githooks/CLONE.md](.githooks/CLONE.md).
