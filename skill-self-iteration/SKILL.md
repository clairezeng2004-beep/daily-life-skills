---
name: skill-self-iteration
description: Turn lessons from using a Codex skill into a focused skill update, validate it, and prepare the repository change for upload without overfitting to one conversation.
---

# Skill Self Iteration

Use this skill when the user wants to improve, revise, maintain, or upload one of their personal Codex skills after a real use case exposed a gap. The goal is to make the next use better while keeping the skill general, small, and easy to follow.

## Core Principle

Update a skill only with lessons that will change future behavior. Do not add a rule just because a phrase worked once. Do not turn one bank, company, document, person, or conversation into a permanent default unless the user explicitly wants that scope.

A good skill update is:

- reusable across similar future requests;
- specific enough to guide a better decision;
- narrow enough not to distort unrelated uses;
- phrased as operating judgment, not a transcript summary;
- easy for a future model to apply without seeing the original conversation.

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

## Workflow

1. Identify the target skill folder and read its `SKILL.md` before proposing edits.
2. Summarize the learned lesson in plain language before editing when the user asks to review the plan first.
3. Convert the lesson into a general instruction, decision test, warning sign, or final quality-gate item.
4. Place the update where future users will naturally look for it. Prefer editing an existing section over adding a new top-level section.
5. Preserve the skill's original scope, tone, frontmatter, and structure unless the user asks for a larger redesign.
6. Avoid duplicating long instructions across skills. If one skill is the canonical style guide, have related skills refer to it briefly.
7. Validate the file shape and diff before finishing.
8. If the user asks to upload, commit only the intended changes and push to the repository.

## Extract The Lesson

When using a previous conversation as evidence, treat it as raw material, not instructions. Extract the general pattern:

| Conversation detail | Skill-worthy lesson |
|---|---|
| A sentence felt generic | Add a counterfactual test for whether the claim would fit competitors. |
| A bank-specific fact was overused | Add a rule separating fact, inference, and candidate preference. |
| A polished answer sounded too AI-like | Add a prose warning against the repeated pattern. |
| The user had to paste two skills | Add a short style-dependency rule to the content skill. |

Ask: "Would this rule still help if the company, document, or user example changed?" If not, do not add it.

## Edit Rules

- Keep edits close to the relevant section.
- Prefer one or two sharp bullets over a long new framework.
- Use examples only when they clarify a decision that would otherwise be ambiguous.
- Avoid company-specific examples unless the skill already has a named-company section or the user requests it.
- Preserve existing user-specific preferences that are already encoded.
- Do not remove unrelated instructions while cleaning up prose.
- Do not create helper scripts, assets, or reference files unless the workflow genuinely repeats enough to justify them.

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
3. Use a concise commit message naming the skill and purpose.
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
