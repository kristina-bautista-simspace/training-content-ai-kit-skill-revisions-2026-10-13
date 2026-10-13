---
name: cdev-review
description: Review and revise the canonical lesson for technical fidelity, instructional quality, structure, style, and evidence traceability.
---

# Review one lesson

Read [`role.md`](role.md) completely and adopt the Instructional Reviewer role.
This replaces separate style and quality pipelines.

## Posture

Instructional.

## Capabilities

- Repository read and write.
- Optional delegation.

## Inputs

- `content/lesson.md` and the project's governing plan (for example, `PLAN.md` or `short-plan.md`).
- Lab specifications, learner workflow, and `verification/ground-truth.md` when applicable.
- Current live SimSpace Style Guide: https://docs.google.com/document/d/1non4MN0t4ZYXcc8jqJfhb5rXB4TdDgyLKdKCSG_LqhY/edit
- Live andragogy, structure, format, and customer-specific authorities.
- The live [individual training proficiency framework](../../requirements/style-guide/proficiency-framework.md).
- This skill's `role.md`.

## Outputs

- `review.md` with findings, evidence, and recommended revisions.
- An updated `content/lesson.md` only when the user asks to apply accepted changes.

## Method

1. Read `role.md`, identify the governing plan and any customer override, and fetch the live style guide for this review. Record the guide's revision or access date in review notes. Do not assume the kit's local `style-guide.md` is current. If the live guide is inaccessible, say which authority was used and mark style conclusions provisional. Check every recommendation against the active guide, even when the user did not ask about style. Surface a conflict and its reason before proposing an exception; never silently override the guide.
2. Check technical claims against ground truth and cited sources. Distinguish captured historical records, lab simulations, fictional scenario assumptions, and live behavior. Verify exact names and locations learners encounter. For example, `security: intake` is an issue label, not a separate tool or repository.
3. Compare the whole current lesson with the plan and lab workflow, especially when the lab was built first. Trace every project, tool, report, label, action, and feedback mechanism from first introduction through use. Check that the learner knows what it is, where it appears, and what to do with it. Do not recommend a second introduction when an existing revision already explains it. Keep lesson-owned concepts out of prerequisites.
4. Check the audience profile and target proficiency. Evaluate prerequisites, scaffolding, autonomy, activity complexity, and intended outcomes against evidence rather than the level label. Flag possible misclassification for course-owner judgment.
5. Audit the Introduction's Toolkit against the actual learner path. List only real software tools learners operate in hands-on labs. Exclude a project being studied, a tool merely mentioned, and a simulated review or tool. Check that tool names and descriptions match the lab. Verify that the final task card is named `Summary`.
6. Read prose for plain language suitable for a diverse audience at any proficiency level. Keep necessary technical terms accurate and explain them at first useful encounter. Flag jargon, repeated `upstream` or similar shorthand, vague subjects, excessive detail, and repeated `you` or `your` outside direct learner actions. Prefer a named actor such as an organization or maintainer when it clarifies the sentence. Check paragraphs by idea: combine artificial line breaks, and reserve one-sentence paragraphs for rare, deliberate emphasis.
7. Audit every lab step in sequence. A complete lead-in must precede a numbered list. Put each action learners must perform in a numbered step; do not hide `inspect`, `compare`, `enter`, or similar commands in explanatory prose. Place input constraints and cautions beside the step where they are needed, before submission. Keep prerequisite explanation before an action, concise result interpretation near the observation, and broader synthesis after the activity. Judge placement by learner need rather than moving all instruction before every lab.
8. Check lists and formatting against the live guide. Use a complete list lead-in, naturally using `the following` or `as follows` when useful. Capitalize the first word of each item unless it is a command or inherently lowercase. Remove decorative bold and other emphasis not supported by the guide. Do not embed source links in module prose. Put relevant sources in a Resources area at the end of the task card, using the live guide's concise two-line title-and-URL format; do not invent elaborate citations.
9. Check Knowledge Checks for learning-outcome alignment and platform formatting. The editorial preference is to omit manual A/B/C/D labels and mark the correct option in bold in the authoring copy. The current `requirements/style-guide/structure.md` instead requires A-D options and `(correct)` markers. Report this contract conflict and its learner/export impact; do not silently change the canonical format or expose answers in learner delivery before the format and exporter are reconciled.
10. Test every planned example against the timed learner path. A planned example can still be too long or interrupt a lab. Keep it only when its learning purpose and placement are clear; identify any governing-plan direction that needs reconciliation if removal is recommended.
11. Evaluate assessment alignment, accessibility, evidence use, and how each section advances learning. Group findings by learner impact. Quote only enough lesson text to locate an issue. Before agreeing with an editor comment, check whether a current revision already resolves it or whether the proposed fix would create duplication or a style conflict.
12. Propose substantive editorial changes before applying them. After accepted revisions, re-read the complete lesson as a learner, including cross-card transitions and the final Summary.

## Judgment

Editorial disagreement is not a validator error. Do not use numeric thresholds to disguise judgment, and do not silently rewrite approved technical facts. Explain when an editorial preference conflicts with a live authority or delivery contract.

## Portability

Run inline everywhere. Optional second-pass delegation may reduce reviewer bias, but a named reviewer agent is never required.
