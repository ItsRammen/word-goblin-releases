# Word Goblin — releases

Signed Firefox builds of **Word Goblin**, an AI-assisted writing helper for Zendesk Agent Workspace
(rewrite, translate, summarize, snippets).

This repo is the distribution channel only — it holds the signed `.xpi` for each version and the
update manifest Firefox polls. The source lives elsewhere.

## Install

1. Download the latest `word-goblin-firefox-<version>.xpi` from
   [Releases](../../releases/latest).
2. In Firefox, open `about:addons` → the gear icon → **Install Add-on From File…**, and pick the
   file. (Dragging it onto that page works too.)

The build is signed by Mozilla, so it stays installed across restarts.

## Updates

Updates arrive on their own — no need to come back here. Firefox checks `updates.json` every few
hours; `about:addons` → gear → **Check for Updates** forces it immediately.

## Files

| File | What it is |
| --- | --- |
| `updates.json` | The update manifest Firefox polls. Must stay at the repo root on `main`. |
| Release assets | One signed `.xpi` per version, tagged `v<version>`. |
