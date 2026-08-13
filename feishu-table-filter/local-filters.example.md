# Feishu Table Filter Local Config Example

Copy this file to `local-filters.md` and fill in your own private table links, field names, and presets.

`local-filters.md` is ignored by git and should not be uploaded.

## Tables

### daily-projects

- URL: `https://example.feishu.cn/wiki/...?...`
- Table: `Projects`
- Default view: `Main`
- Reset filters first: `yes`

## Presets

### default

- Table: `daily-projects`
- View: `Main`
- Reset filters first: `yes`
- Filters:
  - Field: `Owner`
    Operator: `is`
    Value: `me`
  - Field: `Status`
    Operator: `is not`
    Value: `Done`
- Sort:
  - Field: `Due date`
    Direction: `ascending`
- Expected result: `Open records owned by me, sorted by due date.`

### waiting-for-reply

- Table: `daily-projects`
- View: `Main`
- Reset filters first: `yes`
- Filters:
  - Field: `Status`
    Operator: `is`
    Value: `Waiting`
  - Field: `Owner`
    Operator: `is`
    Value: `me`
- Expected result: `Items where I am waiting for someone else.`

