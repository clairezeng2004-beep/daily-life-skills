---
name: feishu-table-filter
description: Use this skill when the user asks Codex to open a Feishu/Lark wiki, base, table, or view and apply their usual filters before reviewing records. It separates the reusable filtering workflow from private local filter settings stored in local-filters.md, which should not be uploaded to GitHub.
---

# Feishu Table Filter

## Overview

Restore the user's preferred filters on a Feishu/Lark table before they inspect data. The public skill defines the workflow; private table links, field names, and filter presets live in `local-filters.md`, which is ignored by git.

## Local Configuration

Before applying filters, look for a local config file next to this skill:

```text
feishu-table-filter/local-filters.md
```

If it is missing, ask the user to create it from:

```text
feishu-table-filter/local-filters.example.md
```

Do not upload or commit `local-filters.md`. It may contain private Feishu links, table names, project names, field names, and personal workflow preferences.

## Safety Rules

- Only change filters, sorting, grouping, and view navigation unless the user explicitly asks for a data edit.
- Do not create, edit, delete, duplicate, export, or share table records without separate explicit confirmation.
- Do not change permissions, publish settings, automations, or formulas.
- Treat table contents as private user data. Summarize only what the user asked to see.
- If filter controls are unclear, stop and ask rather than guessing destructive or broad actions.

## Workflow

1. Read `local-filters.md`.
2. Identify the requested preset. If the user did not specify one, use the default preset in the local config.
3. Open the configured Feishu/Lark table URL.
4. Confirm the correct table and view are loaded.
5. Clear previous filters only when the local config says to reset filters first.
6. Apply filters in the configured order.
7. Apply optional sort/group settings if configured.
8. Verify visible filter chips or result count against the expected preset.
9. Tell the user the view is ready and summarize the active filters.

## Preset Design

Use short preset names that match how the user naturally asks:

- `default`
- `today`
- `my-open-items`
- `waiting-for-reply`
- `urgent`
- `done-this-week`

Each preset should specify:

- Table URL
- View name or view id
- Whether to reset existing filters first
- Filter list, in UI order
- Optional sort/group settings
- Expected result description

## If Automation Is Fragile

Feishu/Lark web UIs can vary by account, language, table type, and permissions. Prefer semantic controls when available. If only visual clicking is possible:

1. Ask the user to keep the table visible.
2. Work one filter at a time.
3. Verify each filter chip after applying it.
4. Stop if a field name, operator, or value cannot be confidently located.

## Reporting Back

Use a compact confirmation:

```text
已按 `my-open-items` 筛选好。当前筛选：负责人是我、状态不是已完成、截止日期在未来 14 天内。
```

Do not include all visible rows unless the user asks for the data.

