# Training Content AI Kit skill revisions

Prepared October 13, 2026 from the local `training-content-ai-kit-upstream` copy. These are replacement skill files, arranged by their path under the kit root:

- `skills/cdev-review/SKILL.md`
- `skills/cdev-write/SKILL.md`

The accompanying files are complete replacements for those two `SKILL.md` files. Their existing `role.md` files and the writer's evidence-status helper remain in the kit. No original kit file, AI-5 lesson file, online repository, or GitHub resource was changed.

## What changed

- Both roles now fetch the current [SimSpace Style Guide](https://docs.google.com/document/d/1non4MN0t4ZYXcc8jqJfhb5rXB4TdDgyLKdKCSG_LqhY/edit) on each run, check advice against it, and tell the user when a proposed exception or inaccessible live source limits confidence. The guide was read on October 13, 2026; its returned revision ID was `AHj4eMTthDan0ZE90SeP3OLAW5tFEjqL3wLfNGJNEBUjHUrLcFIQWvysb-1GRx0HPPtG5_UIhcJTwO_33W0BeXQ`.
- The writer maps lab reality to lesson prose before drafting; the reviewer checks that map across the whole module. OpenClaw is the project studied; Firefox and Forgejo are operated tools; ClawSweeper is an automated reviewer whose comments are read. Historical PR #82955 belongs to the lab's captured history, while the four added reports and their reviews are authored exercise material. The label `security: intake` is named as a label and its location is given, rather than being described as a separate queue.
- Toolkit guidance now includes only real tools learners operate. Names merely mentioned, simulated reviews, and projects under study are excluded. The first introduction explains a name once; later cards use it without repeating the definition.
- Both roles check for plain language, restrained second person and technical jargon, paragraph cohesion, and scope. One-sentence paragraphs are exceptional. A planned example must still justify its space in the timed learner path. The curl detour in AI-5 is the case that prompted this check.
- Lab checks distinguish background, actions, and interpretation. Actions belong in numbered steps; instructions and input constraints appear where learners need them. The `escalate` instruction belongs with the step where the comment is entered, not after the submission step. A complete lead-in precedes numbered lists, as the live guide requires. Interpretation may follow the observation it explains; moving every explanation before a lab is not a universal fix.
- Formatting checks cover list lead-ins, item capitalization, limited bold, Resources at the end of the relevant task card, and the final `Summary` task card name. Source URLs should not be embedded as links in learner prose. Resources use a bold page title and a full URL in inline code on the next line, with no live link or final period.
- Reviewers now test editor suggestions against the latest revised module and its governing authorities. If a concern has already been resolved, they report that instead of adding a duplicate explanation. They identify genuine style or format conflicts before recommending exceptions.

## Known format conflict

The editorial preference from this review is to omit manual A/B/C/D labels from Knowledge Check options and bold the correct answer in the authoring copy. The current `requirements/style-guide/structure.md` specifies A-D options with `(correct)` markers. The live SimSpace Style Guide does not resolve that source-format contract. Both revised skills flag the conflict and preserve the current parseable lesson format until the format specification and exporter are updated or an approved alternative is confirmed. This avoids accidentally exposing an answer in learner delivery.

The local kit copy of `requirements/style-guide/style-guide.md` also describes a Resources first line as a summary of purpose. The live guide specifies the page or website title instead. The revised skills explicitly follow the live guide and flag access limits. The local guide itself is not part of this replacement package.

## Scope

The local upstream copy contains `cdev-review` and `cdev-write` skills but no `cdev-style` or `cdev-quality` skill files. This package updates the two lesson-facing skills that exist in that copy. It does not attempt to rewrite the module, the lab, the plan, the style guide, or the exporter. Those are separate decisions, including any Knowledge Check format change.
