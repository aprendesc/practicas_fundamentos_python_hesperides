# Project organization

This repository prepares classes and exercises for Fundamentos de Python at Universidad de las Hespérides. It preserves the teaching format and organization of the Deep Learning exercises project, excluding its content and planning. Chapter 1 has a confirmed duration of 90 minutes and uses the Programación I notes. The number and duration of other sessions, and their prerequisite knowledge, remain unconfirmed.

## Public and private surfaces


- `workshop/` is the versioned student distribution and contains only `clases_sincronas/` and `tareas/`. The new visual proposal resides in `professor/clases_sincronas/capitulo_1.ipynb`; the student copy and exercises remain pending. Preparing the local file does not imply uploading it to GitHub.

- `professor/` is ignored in Git and mirrors `clases_sincronas/` and `tareas/` with solved and enriched versions. It adds `resources/` for private preparation materials.

- Deliver each class in one `capitulo_N.ipynb` directly in `clases_sincronas/`. When preparing only the structure, do not create notebooks or course content.

- Student notebooks must not contain solutions, private hints, or instructions to lead the class. Put teacher solutions in the teacher notebook itself.

- Separate every private script or solution into cells tagged `professor-only`. Add `teacher-guide` to scripts. Use black for public text and red for teacher text. Do not use color alone to separate the content.

## Private resources

Within `professor/resources/`, the reserved folders are `notas/`, `medios/`, `scripts/`, `documentacion/`, `cache_datos/`, and `skills/`. `notas/` contains a copy of Programación I chapter 1 and its six referenced images. The source and content selection are documented in `documentacion/capitulo_1.md`. Do not create data, laboratory, or script folders at the root. Do not add dependencies on files from the previous project.

## Editing and publication


- Before rebuilding a notebook, preserve manual additions.

- Work on unpublished proposals in `professor/`. To review published material, identify the canonical version. Do not edit the same public cells in parallel.

- Publish only when requested. Derive the student edition without changing its public cells. Exclude private cells, metadata, and outputs.

- No generation or validation scripts were copied from the other course. Before running newly created scripts, inspect them. Do not assume that a build pipeline exists.

- Validate the format, execution from the final location, and operation of browser controls. Do not claim to have tested notebooks that do not yet exist.

- `AGENTS.md` and `professor/` are ignored local context. Do not force them into Git. Commit and push require a request.

## Teaching criteria


- Before designing a class, read the available notes and sources. Cover programming fundamentals at the agreed level. Unlike a neural network class, Python syntax and semantics may be the main subject.

- Use one central concept per block and one relevant visualization per insight. Do not repeat cosmetic variants. Use the sequence: explanation, prediction, execution, modification, and comparison.

- Provide clear academic theory for students. Highlight key questions. Use executable examples. Give the teacher script one bullet per topic. Include a short explanation in bold and a natural spoken paragraph in the first person plural. Connect sentences. Keep unnecessary punctuation to a minimum.

- When controls and Play help explain the mechanism, use them. Instruction execution and branches are discrete. Do not interpolate fictitious Python states to make playback appear smooth.

- Make notebooks self-contained and executable on CPU with the environment in `pyproject.toml` and `uv.lock`. They must not require the original repository. Add libraries for actual needs. Do not carry over neural network dependencies.

## Chapter 1 construction

The class was rebuilt from scratch at the user’s explicit request. `professor/resources/scripts/construir_aula_visual.py` generates and executes only the teacher proposal `professor/clases_sincronas/capitulo_1.ipynb`. `aula_visual.html` contains the new scenes, and `validar_aula_visual.cjs` checks their models. It does not import previous generators. Before using `--replace`, integrate manual additions. Previous notebooks, generators, evidence, and checkpoints were removed from the project at the user’s express request.

Do not restore or reuse them.

The confirmed criterion is a simple, graphical, animated class with distinct concepts. It has 30 visual cells and 30 private literal scripts, one immediately after each scene (60 cells total). Six 15-minute blocks include 12 minutes of exploration and 3 minutes of practice in pairs. `conceptos_clase.py` defines questions, sources, representations, and the core oral content. `guiones_ampliados.py` develops each explanation to 313–349 words in four paragraphs. The paragraphs are red and have the tags `professor-only` and `teacher-guide`.

To edit only scripts without changing or executing public cells, use `construir_aula_visual.py --guides-only`.
Validate with `validar_guiones_profesor.py`. `conceptos_visuales.js` adds the specific illustrations. The map resides in `professor/resources/documentacion/mapa_conceptos_clase.md`. Each representation appears once, except terminals and the board, which appear twice. Do not split a mechanism into one cell per step.

Group the phases of Turing, the CPU cycle, and the cache in one cell each. When charts and occasional formulas explain a concept from the notes, use them. Identify synthetic models and samples as such. They are not real measurements. Derive the student edition only when requested.

## Local skill

When creating or refining synchronous classes, read and use `professor/resources/skills/sync_lesson_generator/SKILL.md`. It preserves the teaching format and tone and is adapted to Fundamentos de Python. It contains no paths to demos or chapters from the previous course. It is a local resource, not a global installation.

## Downstream continuous integration

Read `$downstream-ci` for the integration policy. Integrate numbered contribution branches through validated pull requests into `downstream/develop`, without mandatory GitHub approvals or status checks. After merge, return the clean worktree to setup to develop. For a distinct personal or Pantagruel upstream, prepare a clean numbered branch and use a PR into upstream develop. Validate publication changes before the release PR into main. This policy supersedes earlier integration instructions where they conflict. Keep corporate upstream procedures unchanged.
