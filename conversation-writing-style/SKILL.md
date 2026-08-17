---
name: conversation-writing-style
description: Use this skill when the user asks for a long-form Chinese plain-text reply, Word-ready prose, a less AI-like conversational writing style, or specifically asks to avoid markdown, excessive quotation marks, dash-style insertions, mechanical transitions, and structured AI formatting.
---

# Conversation Writing Style

## Overview

Write Chinese long-form responses that feel like a knowledgeable person talking through an idea slowly and naturally. The target output is plain text that can be copied directly into Word, with high information density and minimal machine-like formatting.

Before writing, read the full local style guide:

```text
conversation-writing-style/对话回复写作风格规范.md
```

## When To Use

Use this skill when the user asks for:

- A Chinese long-form answer that should read like human prose
- Word-ready plain text
- A rewrite that removes AI flavor
- Fewer quotation marks, less markdown, less rigid structure, or more natural sentence rhythm
- A response following the user's 对话回复写作风格规范

## Core Rules

- Prefer natural paragraphs over markdown structure.
- Do not use markdown headings, bold, tables, blockquotes, horizontal rules, or bullet lists in the final user-facing artifact unless the user explicitly asks for them.
- Avoid Chinese em dashes and dash-style insertions. Rewrite with commas or separate sentences.
- Avoid decorative quotation marks around terms unless they are necessary for accuracy.
- Avoid colon-led parallel lists. Turn them into prose.
- Use Chinese numbered headings such as 一、二、三 when headings are needed.
- Keep one main idea per paragraph.
- Use specific examples only when they are accurate or clearly qualified.
- End cleanly without formulaic closing lines.

## Workflow

1. Read `对话回复写作风格规范.md`.
2. Identify whether the user wants a direct answer, a rewrite, or a reusable writing artifact.
3. Draft in plain Chinese prose with natural paragraph breaks.
4. Self-check for markdown residue, excessive quotation marks, em dashes, bullet lists, rigid transitions, and empty closing phrases.
5. Return only the polished text unless the user asks for explanation.

## Related Files

- `对话回复写作风格规范.md`: the full writing standard and self-check list.
