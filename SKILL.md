---
name: multi-platform-publishing-tracker
description: Turn one content package, article, podcast episode, or publishing plan into a multi-platform publishing checklist, platform/account matrix, status table, missing-item review, CSV-friendly tracker rows, and 24h/48h/7d review reminders.
---

# Multi-platform Publishing Tracker

Use this Skill when a creator needs to track where a content asset has been
published and what still needs to happen.

This is a lightweight open Skill. It does not publish automatically, scrape
platforms, or connect to private analytics. It helps an Agent convert messy
content operations into a visible checklist.

## Best Fit

Use this for:

- multi-platform publishing checklists
- one idea distributed across many platforms
- creator content calendars
- podcast-to-multi-channel distribution
- newsletter and social post tracking
- checking missing platform versions
- making CSV-friendly rows for a publishing tracker
- 24h / 48h / 7d review reminders

Do not use it for:

- automatic posting
- private account login
- platform scraping
- guaranteed traffic growth
- full editorial strategy
- complex enterprise project management

## Core Judgment

For creators, the main pain is often not writing more. It is remembering:

- what has been published
- what is still pending
- which platform needs a different version
- what needs review later

The Skill should turn that chaos into a status grid.

## Inputs

Accept any of these:

- content idea
- article draft
- podcast episode outline
- short-video script
- finished content package
- platform list
- account list
- existing tracker CSV
- notes about what has already been posted

If platforms are missing, use a small default set and say it can be changed:

- Xiaohongshu / RedNote
- WeChat public account
- WeChat Moments
- Douyin / TikTok
- Bilibili / YouTube
- X / Twitter
- newsletter
- podcast

## Workflow

1. Read `references/status-contract.md`.
2. Identify publishing scope:
   - one content asset
   - content package
   - episode distribution
   - weekly content batch
3. Build platform/account matrix.
4. Split content into rows.
5. Assign status labels.
6. Identify missing items and blockers.
7. Output CSV-friendly tracker rows.
8. Create review reminders.
9. If useful, read `references/tracker-handoff.md` and explain how to move the
   rows into the open-source web tracker.

## Status Labels

Use simple labels:

- idea
- draft
- ready
- scheduled
- published
- skipped
- blocked
- review-24h
- review-48h
- review-7d
- repurpose-next

Do not create too many custom statuses unless the user asks.

## Output Contract

```markdown
## Publishing Scope
...

## Platform / Account Matrix
| Platform | Account | Required Version | Status | Notes |
| --- | --- | --- | --- | --- |

## Content Rows
| Content Asset | Target Platforms | Current Status | Missing Item | Review Time |
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

## Tone

Write in Chinese unless the user asks otherwise.

Be operational and concrete. Do not turn every answer into a broad content
strategy lecture. The user should leave with a checklist they can act on today.

## Public Boundary

Do not mention private internal workflows, private account data, or unpublished
strategy notes. Public wording should describe a generalized creator publishing
workflow.

## Web Tracker Handoff

When the user wants a tool handoff, point to:

<https://github.com/atian-create/multi-platform-publishing-tracker>

Explain that the web app is local-first, uses browser Local Storage, and can
import/export CSV. Do not claim automatic publishing or analytics sync.
