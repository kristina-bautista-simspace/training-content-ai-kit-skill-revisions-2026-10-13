---
name: cdev-write
description: Author or revise the canonical lesson from the plan, live editorial authorities, and visible lab-evidence status.
---

# Write from evidence

Read [`role.md`](role.md) completely and adopt the Instructional Writer role
before producing learner-facing prose.

## Posture

Instructional.

## Capabilities

- Repository read and write.
- Optional image generation.
- Optional delegation.

## Inputs

- The project's governing plan (for example, `PLAN.md` or `short-plan.md`).
- Current live SimSpace Style Guide: https://docs.google.com/document/d/1non4MN0t4ZYXcc8jqJfhb5rXB4TdDgyLKdKCSG_LqhY/edit
- Live andragogy, structure, research, format, and customer-specific authorities.
- The live [individual training proficiency framework](../../requirements/style-guide/proficiency-framework.md).
- `verification/ground-truth.md` and lab specifications when the plan is hands-on.
- Existing `content/lesson.md` when revising.
- This skill's `role.md`.

## Outputs

- Canonical `content/lesson.md`.
- Images under `content/images/` when requested and supported.
- Visible provisional markers for any unverified technical assumption.

## Method

1. Read `role.md` and the complete project authorities. Fetch the live SimSpace Style Guide for each writing or revision run; note its revision or access date. Do not treat the kit's local `style-guide.md` as proof of the current rule. Customer overrides take precedence within their stated scope. If the live guide cannot be read, disclose that limit and treat style judgments as provisional. Do not quietly depart from an active rule; identify any proposed exception to the user with its reason.
2. Use the governing plan's audience profile and target proficiency to calibrate guidance and scenario complexity, but write in plain language accessible to readers with diverse backgrounds. Use accurate technical terms and explain unfamiliar ones when needed. Avoid jargon, inflated explanations, repeated `upstream` or similar shorthand, and needless `you` or `your` in general prose. Use second person mainly for direct learner actions. Keep related sentences in one paragraph; one-sentence paragraphs should be rare and serve a clear point.
3. Inspect the plan's hands-on declaration and available ground truth. The optional [`scripts/evidence-status.mjs`](scripts/evidence-status.mjs) helper reports this boundary without turning missing evidence into a gate. For verified hands-on work, write from observed behavior and cite evidence in author notes where traceability matters. For absent or provisional evidence, recommend verification first and offer evidence-independent concepts or an explicitly provisional draft. For `Hands-on: no`, write without a lab dependency.
4. Before drafting the learner path, map lab artifacts and interactions to the lesson. Distinguish real historical records from authored simulations and fictional scenario context. Record where learners find each report, label, source view, action, and feedback reply. Introduce each named project, tool, and reviewer before first use, then avoid reintroducing it on later cards. Verify visible terms against the range: for example, `security: intake` names an issue label. Do not push concepts the lesson teaches into `Key Skills Needed`.
5. Build the Introduction's Toolkit from tools learners actually operate in hands-on labs. Do not add a project merely studied, a tool only mentioned, or a simulation. Check that descriptions match actual use. Name the final task card `Summary`.
6. Keep one lesson source. Recover one unambiguous Git-aware move when safe; ask when multiple candidate lessons exist. Develop each explanation under the live andragogy authority, but keep only what advances a learning outcome or the learner's next action. Test planned examples against scope and time. When an example no longer earns its place, identify the plan change needed instead of retaining a detour solely because the plan listed it.
7. For each lab, give the numbered steps a complete lead-in that states their goal. Put actions in numbered steps rather than hiding them inside notes or explanatory paragraphs. Place constraints beside the step that needs them, before submission; for example, specify the exact `escalate` input where the learner enters it. Use brief point-of-use explanation for an unfamiliar concept, and put result interpretation after the observation. Do not move all explanation before the lab by default. Keep step numbers and cross-card transitions coherent after edits.
8. Before finalizing, audit lists, emphasis, links, and resources against the live guide. Use complete list lead-ins; `the following` or `as follows` can make a lead-in clear without becoming a stock phrase. Capitalize the first item word unless it is a command or inherently lowercase. Use bold only where the guide calls for it. Do not embed source links in module prose. Place sources at the end of the relevant task card in a Resources area: bold page title on the bulleted first line, full URL in inline code on the next line, no live link or final period. Keep citations short and factual.
9. For Knowledge Checks, preserve the active source and delivery contract. The editorial preference is no manual A/B/C/D labels and a bold correct answer in the authoring copy, but current `requirements/style-guide/structure.md` requires A-D options with `(correct)` markers. Do not silently replace that parseable format or reveal correct answers to learners. Flag the conflict for a format/export decision before applying the preference.
10. Re-read the full module after writing, especially if labs preceded prose. Confirm introductions, provenance, exact interface labels, step placement, feedback locations, resource formatting, assessments, and Summary all fit together without repetition.

## Judgment

Never convert a proposed command, output, timing, machine identity, or success condition into verified fact. Use `<!-- TODO: verify ... -->` for unresolved learner-facing details. If a requested revision conflicts with the live guide or a format contract, explain the conflict and a workable option to the user.

## Portability

Run inline on any host that can load the role and authorities. Delegation and image generation are optional.
