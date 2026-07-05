# Status Contract

## Platform / Account Matrix

Use this when mapping where content should go:

| Platform | Account | Required Version | Status | Notes |
| --- | --- | --- | --- | --- |

Definitions:

- `Platform`: Xiaohongshu, WeChat, Douyin, Bilibili, X, newsletter, podcast, etc.
- `Account`: specific account or channel name.
- `Required Version`: what format this platform needs.
- `Status`: current publishing state.
- `Notes`: blocker, link, caption note, or review detail.

## Content Rows

Use this when the user has a content package:

| Content Asset | Target Platforms | Current Status | Missing Item | Review Time |
| --- | --- | --- | --- | --- |

Examples of content assets:

- main article
- Xiaohongshu graphic note
- short video script
- podcast episode
- WeChat Moments short copy
- X thread
- newsletter intro
- Bilibili title and description

## Status Labels

Default labels:

- `idea`: topic exists, no draft yet
- `draft`: draft exists, not ready
- `ready`: publishable version exists
- `scheduled`: scheduled but not live
- `published`: already posted
- `skipped`: intentionally not used for this platform
- `blocked`: needs asset, link, approval, cover, caption, or rewrite
- `review-24h`: check first-day signal
- `review-48h`: check early trend
- `review-7d`: check stable performance and reuse value
- `repurpose-next`: should become another asset

Keep statuses simple. Do not create a complicated project-management system.

## Missing Item Rules

Common missing items:

- no title
- no cover
- no platform-specific opening
- no caption
- no link
- no video cut
- no image package
- no scheduled time
- no review reminder

## Review Reminder Rules

Use:

- `24h`: check first signal, comments, obvious mismatch
- `48h`: decide whether to adjust title, cover, distribution, or follow-up
- `7d`: decide whether the asset should become a series, article, episode, template, or archive

If the platform has no visible metrics, use qualitative review:

- comments
- replies
- saves
- shares
- direct messages
- whether the piece helped clarify the topic
