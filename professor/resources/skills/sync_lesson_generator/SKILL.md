---
name: sync_lesson_generator
description: Create or refine synchronous lesson notebooks with source-grounded concepts, distinct explanatory visuals, and substantial read-aloud teacher narratives beside each teaching scene. Use for lesson authoring and teacher-note expansion across subjects.
---

# Context

Create classroom-ready synchronous lessons in which the learner can see an idea unfold and the teacher has the complete words needed to explain it. A lesson is a sequence of distinct questions and discoveries, not a collection of demonstrations with interchangeable captions. Student explanations, illustrations, interactions and private spoken notes are authored together, including in the first delivery.

This skill is subject-independent. Identify the audience, language, prerequisites, duration, deliverable format, file organization and public/private surfaces from the user's request and local project instructions. An existing lesson is a quality reference, not a syllabus, fixed cell count, visual theme or technical stack to copy. Preserve the existing skill identifier.

# Rules

## Grounding, scope and sequence

- **Read before selecting.** Read the relevant source notes and existing lesson, including source files when available. Extract important concepts, assumptions and relationships. Distinguish theory from the sources, illustrative examples and invented model parameters. Identify missing sources explicitly.
- **Design for this audience.** Introduce only the prerequisites the audience needs. Use language the audience can understand and concrete situations. Do not treat the learner as a child or replace definitions with slogans. Explain technical terms when they become useful, not all at the beginning.
- **Map the contribution of each scene.** Before building, associate each teaching scene with its source section, central claim, prerequisite, question, visual representation, manipulation or observation, expected conclusion and time. A compact working table is enough. Use this map to find missing concepts and repeated coverage.
- **Count learning contributions honestly.** Count public teaching scenes separately from setup, separators, private notes and animation frames. Meet requested quantity through substantive concepts supported by the sources, not by splitting one mechanism into many cells. If source coverage conflicts with the requested duration or count, explain the tradeoff.
- **Merge procedural fragments.** Reading, choosing, changing, moving or returning can be stages of one mechanism within one explorer. Make them separate teaching scenes only when each has a genuinely different learning question and representation. Do not manufacture a new concept by changing an input, title, color or caption.
- **Build a causal story.** Establish a concrete question, expose the mechanism that answers it, and use the remaining uncertainty to motivate the next scene. A transition explains why the next question matters; it does not merely announce its title or repeat the previous conclusion.
- **Budget the actual lesson.** Include spoken explanation, prediction, playback, manipulation and discussion within the agreed duration. Estimate the complete script's reading time as well as interaction time, stating assumptions. Speech may accompany playback; do not budget it as both simultaneous and additional. Mark optional depth separately when necessary rather than silently extending the class.
- **Preserve existing work.** Inspect the canonical notebook and its builder before replacing anything. Integrate manual additions. A narrow request to expand teacher notes does not authorize changes to public theory, illustrations, outputs or unrelated files.

> **Authoring sequence**
>
> Extract -> Sequence -> Author -> Validate -> Publish when requested

In Extract, ground the concepts in the sources. In Sequence, establish distinct contributions, dependencies and time. In Author, develop the public scene and its complete private narration together. In Validate, inspect teaching quality as well as execution and presentation. In Publish when requested, derive the public edition by removing private material.

## Two coordinated teaching layers

- **Make the public layer teach.** Give each teaching scene a clear question, enough theory to understand the representation, the representation itself, a meaningful observation or experiment, and an interpretable result. Keep formulas selective: introduce what their quantities mean and the insight they express. Charts are appropriate when a relationship or comparison is the lesson.
- **Put the script beside its scene.** In a notebook, place an expanded private Markdown guide immediately after each public teaching scene, clearly associated by stable identifier and order. Include an appropriate guide for substantive theory-only scenes too; setup or separator cells need not invent a lesson. Do not collect several scenes' only explanations in a distant end-of-block guide.
- **Make the guide immediately readable.** Display the complete narrative openly, not as a hidden hint, collapsed solution or text requiring execution. Use comfortable paragraph spacing and clear scene identification.
- **Separate privacy structurally.** Keep public prose black on white and teacher speech or solutions red on white using `#b91c1c`. Private notebook cells carry `professor-only`; spoken guides also carry `teacher-guide`. Use an equivalent structural separation in other requested formats. Color is a reading aid, not the access boundary.
- **Keep private content out of public payloads.** Do not embed scripts, answers or teacher instructions in public code constants, hidden HTML, metadata or outputs. Preserve one canonical definition of the public content so teacher and student editions cannot drift.

## Literal teacher narrative

- **Write the words to say.** The script must work when read aloud by a teacher who has not authored the lesson. Replace reminders such as “explain the mechanism,” “ask what happens” or “discuss the result” with the actual explanation, the spoken question and its answer. Put navigation instructions, timing notes and source references outside the read-aloud prose.
- **Develop an explanation, not an outline.** Start a topic with a bold micro-explanation that states its main insight, followed by a colon and connected prose. Keep one teacher bullet per topic; a substantial narrative may contain several paragraphs inside it. A heading, one-sentence summary or short caption is not a complete guide.
- **Use the accepted depth without enforcing a quota.** For an expanded guide like the requested reference, roughly 300–350 words across several connected paragraphs is a useful depth reference, not a universal cell size. Let conceptual difficulty, audience and timing determine length. Never reach a word count through repeated definitions, generic teaching advice or paraphrases of the same conclusion.
- **Ground the explanation in theory.** Explain what the source concept means, why the relationship holds, which assumptions matter and how the current example shows it. Do not merely describe objects on the screen. Keep source anchors available to the teacher without turning the speech into a bibliography.
- **Take the audience through the scene.** Supply the concrete context, define unfamiliar elements, establish the initial state, invite a prediction, follow the meaningful changes, explain the outcome and address the likely misunderstanding. Combine these functions in a natural narrative. Do not copy an identical paragraph template into every guide.
- **Narrate what actually happens.** Name the controls, states, values, paths and results used by this scene. Explain what changes, what stays the same and why. Distinguish an initial state from a completed action; do not describe a predicted or pending outcome as already observed. Give the teacher the expected answers for the proposed comparisons.
- **Use natural spoken language.** Match the classroom language and register. Favor inclusive first-person plural, connected sentences and varied openings. In Spanish, “nos fijamos,” “si cambiamos” or “aquí vemos” can help, but are not stock phrases to repeat mechanically. Use punctuation and paragraph breaks for breathing and logical grouping; avoid both clipped fragments and an unreadable sentence without pauses.
- **Keep narrative causal.** Storytelling means following a question through evidence and explanation, not adding fictional characters, theatrical filler or an unrelated anecdote. An analogy earns its place by explaining a relationship, and its limits must be clear.
- **Finish with transfer.** Explain what the observation lets us conclude, what it does not establish, and the unresolved question that leads onward. Do not end every guide with the same generic request to “reflect” or recap the entire class.
- **Pass the cold-reading test.** Read each guide as literal speech. Could another teacher explain the scene, its results and its limits without improvising missing theory or translating author instructions? If not, complete the narrative before delivery.

A brief example of the distinction, not a complete guide or fixed wording:

> **Reminder:** “Explain the delay and ask why the output has not changed.”
>
> **Literal explanation:** “We have changed the input, but the output still shows the previous value because the change has not reached it yet. Let us follow the marked path before advancing: the middle stage still holds the old state. Once the change reaches the destination, the output updates. The delay does not mean that the input was ignored; it tells us where we are in the process.”

## Visual specificity and variety

- **Choose the representation after the insight.** Use a physical illustration for component roles, an evolving trace for state changes, a chart for quantitative relationships, a map for location, or another form appropriate to the subject. This is a set of possibilities, not a checklist to fill. Do not make a universal box-and-arrow cartoon the default answer to every concept.
- **Give each scene its own explanatory illustration.** For the requested varied lesson style, reuse the same main illustration at most twice unless the user asks to follow one shared explorer. Each reuse must answer a different question. Shared typography, controls or chart primitives are fine; relabeling the same diagram is not a new illustration. Two charts may share axes while explaining genuinely different relationships.
- **Show the mechanism, not just its caption.** Represent where an action occurs, which element acts, what changes and what remains. When a process is central, make its relevant movement, transformation, accumulation, transfer or structural change visible. Buttons and colored rectangles alone do not establish visual quality.
- **Make frames explanatory.** Associate meaningful stages with readable explanations of the event, its cause and its consequence. Highlight the relevant element and make direction, destination and current state legible. A sequence that only cycles labels or changes decorative colors does not explain a process.
- **Preserve useful comparisons.** Keep inputs, initial conditions, scale and assumptions controlled when comparing variants. Label axes, units, reference values and normalization where relevant. Explain what a qualitative illustration's size or distance means instead of inviting false numerical inferences.
- **Use decoration selectively.** Physical detail, texture, realism or 3D should help identify elements or understand relationships. Do not make every scene realistic when an abstract chart is clearer, and do not replace accurate structure with attractive decoration.

## Interaction and technical truthfulness

- **Make controls meaningful.** Let the learner change quantities or conditions central to the question without editing code. Link the visible control value, illustration, result and explanation to the same state.
- **Provide a prepared route.** Interactive scenes need a ready-to-run demonstration and manual control, with Play, pause and reset or an appropriate equivalent; include stepping or reversal when it helps inspect a process. Verify that playback changes the represented mechanism, not only a progress label.
- **Respect the type of change.** Animate continuous quantities smoothly when interpolation has meaning. Keep discrete decisions and evaluated states discrete, even if their physical depiction moves continuously. Label playback or crossfades as such rather than inventing intermediate logical states.
- **Calculate and label honestly.** Compute displayed values consistently with the underlying example. Distinguish conceptual diagrams, simulations, actual execution traces and measurements. Identify synthetic data, illustrative parameters and simplifying assumptions; a model comparison is not a measured speedup or an exact physical law.
- **Support the intended classroom environment.** Follow the agreed runtime and resource constraints. Make the notebook self-contained where requested, including necessary visual assets. Reuse existing working infrastructure when appropriate without importing unrelated course dependencies.

## First-delivery quality gate

- **Review distinctness.** Compare the concept map with the actual cells. If removing a scene loses no explanation, comparison or learning outcome, merge or remove it. If two visuals differ only by labels, decide whether one explorer should contain both. Audit illustration reuse against the intended limit.
- **Review completeness per scene.** Check that every substantive scene has its own readable, source-grounded guide, actual expected results, relevant assumptions and a non-redundant transition. Inspect all guides, not just the opening examples. Length alone does not demonstrate quality.
- **Review pacing and voice.** Read the sequence as a class, checking prerequisite order, repetitive openings, repeated explanations, total spoken volume and space for learner participation. A complete private script supports interaction; it must not turn every exercise into a passive demonstration.
- **Validate the artifact proportionally.** Validate notebook structure and execute changed code from its final location in the project environment. For teacher-text-only revisions, verify unchanged public cells, code and saved outputs instead of rebuilding or rerunning demonstrations unnecessarily.
- **Check UI independently.** Successful kernel execution does not prove that embedded visuals work. In the target browser inspect actual rendered scenes and long teacher notes, legibility, clipping, color and adjacency. Exercise meaningful parameter changes, progression, pause/reset and relevant result checks on representative interactions; distinguish those checks from all-scene render or numerical tests.
- **Inspect the final saved version.** Confirm the canonical artifact, public/private counts and what the browser is actually showing. Do not mistake a stale open notebook for the new file. Report any validation not performed and any remaining limitation rather than describing an attempted check as completed.
- **Publish only when requested.** Derive the student edition by subtracting private cells, metadata and outputs without changing public content. Inspect the derived file for leaks. Lesson creation or revision does not authorize publication, commit or push; honor the project's locations and workflow.
