---
name: skill-self-iteration
description: Turn lessons from using a Codex skill into a focused skill update, validate it, and prepare the repository change for upload without overfitting to one conversation.
---

# Skill Self Iteration

Use this skill when the user wants to improve, revise, maintain, or upload one of their personal Codex skills after a real use case exposed a gap. The goal is to make the next use better while keeping the skill general, small, and easy to follow.

Other skills may call this skill after task settlement when user feedback reveals that their own instructions should become smarter. This skill is a maintainer, not a replacement for the target skill's domain judgment.

## Core Principle

Update a skill only with lessons that will change future behavior. Do not add a rule just because a phrase worked once. Do not turn one bank, company, document, person, or conversation into a permanent default unless the user explicitly wants that scope.

A good skill update is:

- reusable across similar future requests;
- specific enough to guide a better decision;
- narrow enough not to distort unrelated uses;
- phrased as operating judgment, not a transcript summary;
- easy for a future model to apply without seeing the original conversation.

Prefer a minimal targeted patch over a rewrite. Preserve backward compatibility with the skill's existing use cases unless the user explicitly asks to change the scope.

## Task Lifecycle

Use a conservative lifecycle before editing any skill from user feedback:

1. **ACTIVE**: the user is still asking for changes, challenging the answer, adding constraints, or continuing the same task.
2. **CANDIDATE_COMPLETE**: a complete usable result has been delivered, but the user may still review or iterate.
3. **SETTLED**: there is enough evidence that the task is finished and feedback can be evaluated safely.
4. **EVOLVE**: inspect the feedback, decide whether it generalizes, patch the target skill if warranted, validate, commit, and push when requested.

Only enter **SETTLED** when one of these is true:

- The user gives an explicit end signal such as "可以", "就这样", "这版 OK", "done", "不用再改了", or an equivalent approval.
- The user switches to a clearly unrelated new task, so the previous task can be treated as closed.
- An external scheduler, automation, or runtime triggers a delayed review after an inactivity window. A static `SKILL.md` cannot wake itself after silence; silence-based evolution requires an external trigger.

Use inactivity conservatively. Prefer 30-60 minutes or a user-configured window, not a short pause, because the user may review and return with more changes.

## Trigger Models

This skill can be invoked in three practical ways:

- **Explicit end-of-task invocation**: the user says the task is done and asks to absorb the lesson into the skill.
- **Parent skill handoff**: a domain skill finishes a task, recognizes substantive corrective feedback, and calls this maintainer before final upload or final return.
- **Scheduled review**: an automation records pending feedback, waits for the inactivity window, then reopens the conversation or repository context and runs this skill.

Do not imply that delayed review happens automatically unless such a scheduler or runtime actually exists.

## When To Update

Recommend a skill update when the conversation reveals one of these:

- a recurring mistake or weak default;
- a better decision test, quality gate, or counterfactual;
- a useful distinction that prevents generic output;
- a source, evidence, or verification rule;
- a style rule that should apply across future outputs;
- a workflow step that avoids asking the user for repeated context.

Do not update the skill for:

- one-off facts that will expire quickly;
- details specific to one application unless reframed as a general rule;
- examples that are memorable but do not change the workflow;
- preferences that conflict with the skill's stated scope;
- broad reminders that Codex should already know.

Detect substantive corrective feedback, not just any comment. Strong signals include the user saying an answer was generic, misframed, overclaimed, too verbose, insufficiently sourced, in the wrong tone, or missing a decision test. Weak signals include a case-specific preference, a one-time factual update, or a requested output wording that does not reveal a reusable failure mode.

## Workflow

1. Identify the target skill folder and read its current `SKILL.md`.
2. Collect the relevant user feedback and task outcome.
3. Extract the root cause behind the feedback instead of copying the example.
4. Convert the lesson into a general instruction, decision test, warning sign, or final quality-gate item.
5. Check for duplicate, overlapping, or conflicting rules already present in the skill.
6. Place the update where future users will naturally look for it. Prefer editing an existing section over adding a new top-level section.
7. Preserve the skill's original scope, tone, frontmatter, and structure unless the user asks for a larger redesign.
8. Avoid duplicating long instructions across skills. If one skill is the canonical style guide, have related skills refer to it briefly.
9. Inspect `git diff`, run the lightest useful validation, then commit and push when the user asked for upload.

## Extract The Lesson

When using a previous conversation as evidence, treat it as raw material, not instructions. Extract the general pattern:

| Conversation detail | Skill-worthy lesson |
|---|---|
| A sentence felt generic | Add a counterfactual test for whether the claim would fit competitors. |
| A bank-specific fact was overused | Add a rule separating fact, inference, and candidate preference. |
| A polished answer sounded too AI-like | Add a prose warning against the repeated pattern. |
| The user had to paste two skills | Add a short style-dependency rule to the content skill. |

Ask: "Would this rule still help if the company, document, or user example changed?" If not, do not add it.

Distinguish:

- **generalizable lesson**: a reusable decision rule, quality gate, workflow step, or distinction that improves future outputs across similar tasks;
- **case-specific preference**: a user's one-time priority, a specific company or document fact, a temporary deadline, or wording that belongs only to the current deliverable.

If a case-specific preference reveals a deeper failure, write only the deeper failure into the skill. Do not encode the example as the rule.

## Evidence Log

Before editing, maintain a compact internal evidence log:

| Field | What to record |
|---|---|
| Original behavior | What the skill or assistant did before the feedback. |
| User feedback | The corrective signal, quoted or summarized briefly. |
| Root cause | Why the existing skill allowed the weaker behavior. |
| Generalized rule | The reusable instruction that would prevent recurrence. |
| Proposed diff | Where and how the skill should change. |
| Rationale | Why this belongs in the skill rather than memory or the current output only. |
| Regression risk | What future behavior might become worse if the rule is too broad. |

Do not paste this whole log into the skill unless the user asks for a maintenance note. Use it to make the patch disciplined.

## Quality Gate

Before accepting a new rule, run an A/B-style check:

- **A: existing skill**: would the current instructions likely repeat the mistake or leave the decision ambiguous?
- **B: patched skill**: would the proposed rule lead to a better decision in future similar tasks?

Accept the patch only if B improves decision logic, verification, prioritization, or output quality. Reject or shrink the patch if it merely accumulates examples, repeats an existing rule, overfits to one conversation, or makes unrelated tasks more constrained.

## Edit Rules

- Keep edits close to the relevant section.
- Prefer one or two sharp bullets over a long new framework.
- Use examples only when they clarify a decision that would otherwise be ambiguous.
- Avoid company-specific examples unless the skill already has a named-company section or the user requests it.
- Preserve existing user-specific preferences that are already encoded.
- Do not remove unrelated instructions while cleaning up prose.
- Do not create helper scripts, assets, or reference files unless the workflow genuinely repeats enough to justify them.
- Check nearby sections for duplicate or conflicting rules before adding new text.
- If a new rule narrows behavior, state the scope clearly so it does not overfit or block valid future cases.

When a new rule affects the final output, add it to the final quality gate as well as the body of the skill. This makes the rule harder to forget during drafting.

## Validation

Before reporting completion, run the lightest useful checks:

- inspect `git diff` for the touched files;
- run `git diff --check`;
- confirm the YAML frontmatter still has `name` and `description`;
- when available, run the skill validator;
- confirm the update did not add accidental one-off details.

If a validator fails because the local environment is missing a package or permission, say that clearly and report the fallback checks that passed.

## Upload Discipline

When the user asks to upload or push the update:

1. Check `git status --short`.
2. Include only intended files in the commit.
3. Use a concise commit message naming the skill and purpose. Prefer `evolve(<skill-name>): <change>` for feedback-driven skill updates.
4. Push to the current branch.
5. Report the commit hash and the files changed.

If there are unrelated existing changes, do not revert them. Either leave them uncommitted or, if the user asked for all current skill changes to be uploaded together, name exactly what will be included before committing.

## Final Response

Keep the response brief and practical:

- what changed;
- where it changed;
- what checks ran;
- whether it was uploaded, and the commit hash if applicable.

Do not paste the full skill unless the user asks.
