# Multi-platform Publishing Tracker Skill

Turn one content package into a clear publishing checklist across platforms,
accounts, statuses, and review reminders.

这个开源 Skill 解决的是创作者分发时最容易乱掉的一件事：

> 内容已经写好了，但不知道哪些平台发了，哪些账号漏了，哪些内容该复盘。

It is a lightweight workflow Skill for creators, indie teams, newsletters,
podcasters, and social media operators who repurpose one idea across many
channels.

It pairs naturally with the open-source web tracker:

<https://github.com/atian-create/multi-platform-publishing-tracker>

The web app gives you a local-first status grid. This Skill helps an Agent turn
raw content plans into that grid: platforms, account columns, publish status,
notes, and review reminders.

## Search Keywords

English keywords:

`multi platform publishing`, `content publishing tracker`,
`social media publishing checklist`, `creator content calendar`,
`content distribution workflow`, `publishing status tracker`,
`repurpose content across platforms`, `newsletter publishing checklist`,
`podcast content distribution`, `AI skill for creators`,
`local-first content tracker`.

中文关键词：

`多平台发布`, `内容发布追踪`, `发布状态表`, `创作者发布清单`,
`自媒体内容分发`, `多账号发布`, `小红书公众号播客分发`,
`内容复盘提醒`, `发布日历`, `内容运营工具`, `创作者工具`.

## Why This Exists

For many creators, the hard part is not writing one more post. The hard part is
remembering:

- which platform already received the content
- which account still needs a version
- which post needs a caption, cover, or link
- which content should be reviewed after 24h, 48h, or 7 days
- which ideas became assets and which disappeared in chat history

This Skill turns a messy content package into a visible operating checklist.

## What It Can Do

- build a publishing checklist from one content idea or content package
- map platforms and accounts into columns
- convert content assets into rows
- mark current status: draft, ready, published, skipped, review needed
- identify missing platform versions
- create a 24h / 48h / 7d review reminder plan
- prepare CSV-friendly rows for the tracker web app
- recommend what to publish next without turning into a full content strategy

## Who It Is For

This Skill is useful for:

- solo creators publishing across Xiaohongshu, WeChat, Douyin, Bilibili, X, or newsletters
- podcast creators turning one episode into clips, notes, articles, and posts
- small content teams that do not need a heavy project-management system
- indie builders doing Build in Public across many channels
- creators who need a local-first checklist instead of another SaaS dashboard

## Open-Source Boundary

This open version includes:

- publishing checklist workflow
- platform/account matrix rules
- status labels
- CSV-friendly output contract
- review reminder logic
- examples
- optional handoff to the open-source web tracker

This open version does not include:

- private platform credentials
- automatic publishing
- private analytics connectors
- scraping or monitoring
- guaranteed traffic or growth claims
- internal creator operations notes

## Relationship To The Web App

The existing open-source web app:

<https://github.com/atian-create/multi-platform-publishing-tracker>

is a local-first browser grid. It stores content in Local Storage and supports
CSV import/export.

This Skill sits before and after the grid:

1. Before publishing: turn a content package into rows, columns, and status labels.
2. During publishing: check what is missing or blocked.
3. After publishing: create review reminders and next-action notes.

You can use the Skill without the web app, but the best workflow is:

```text
content package -> Skill checklist -> tracker grid -> review reminders
```

## Best Inputs

You can give the Skill:

- one content idea
- a content package
- article draft
- podcast episode outline
- short-video script
- platform list
- account list
- existing CSV export
- screenshot of a publishing tracker
- notes about what has already been posted

## Output Contract

Default output:

1. Publishing scope
2. Platform/account matrix
3. Content rows
4. Status labels
5. Missing items
6. CSV-friendly table
7. Review reminder plan
8. Next publishing action

## Example Prompts

```text
把这个内容包拆成多平台发布清单：小红书、公众号、视频号、抖音、B站、X。
```

```text
我这篇文章已经发了公众号和朋友圈，帮我检查还漏了哪些平台，并做复盘提醒。
```

```text
把这期播客拆成发布追踪表：长文、短视频、图文、星球帖、X thread。
```

```text
根据这个发布状态，帮我输出 CSV-friendly 的 tracker 表格。
```

## Example Output Shape

```markdown
## Publishing Scope
...

## Platform / Account Matrix
| Platform | Account | Required Version | Status | Notes |
| --- | --- | --- | --- | --- |

## Content Rows
| Content Asset | Platforms | Current Status | Owner | Review Time |
| --- | --- | --- | --- | --- |

## Missing Items
- ...

## CSV-Friendly Tracker Rows
...

## Review Reminders
- 24h:
- 48h:
- 7d:

## Next Action
...
```

## Repository Map

- `SKILL.md`: Agent entrypoint and workflow rules
- `agents/openai.yaml`: OpenAI Agent display metadata
- `references/status-contract.md`: status labels and table rules
- `references/tracker-handoff.md`: how to hand off to the web tracker
- `examples/sample-publishing-checklist.md`: sample output

## Recommended GitHub Description

> Open Skill for turning one content package into a multi-platform publishing checklist, status table, and review reminder plan.

## Suggested GitHub Topics

`publishing-tracker`, `content-calendar`, `creator-tools`, `content-workflow`,
`social-media`, `newsletter`, `podcast`, `ai-skill`, `local-first`,
`build-in-public`, `open-source`

## License

MIT
