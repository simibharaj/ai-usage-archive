# AI Usage Archive and Dashboard

A system for collecting my own AI work across ChatGPT, Claude, Gemini, Perplexity and Polar into one organized archive, then turning it into a usage dashboard ("AI odometer") and raw material for writing.

I use it to write [AI I.M.O.](https://aiimo.substack.com), a Substack about what AI can actually do when used well. Every post has to answer one question: **what capability does this prove?** The archive exists to keep the evidence, not to write for me.

## What is here
| Path | What it is |
|---|---|
| `docs/PIPELINE.md` | How the daily collection workflow works (collect, merge, count, log) |
| `docs/PRIVACY.md` | What is deliberately never collected or published |
| `templates/` | CSV headers for the archive tabs (Sessions, Her Words, Media, Lanes, Dashboard, Run Log) |
| `dashboard/index.html` | A small static dashboard that renders the metrics table, shown with **sample data** |
| `dashboard/sample_dashboard.csv` | Example metrics in the Metric / Number / Status / Explanation format |

## Design rules (the interesting part)
- **Collect and organize only.** The system never drafts or rewrites my writing. My own lines are kept verbatim.
- **One work episode, logged once**, even when a problem moves across several models, with a note on why I switched.
- **State changes, not every prompt:** decisions, rejected approaches, artifacts, failures, discoveries.
- **Honest status per platform.** "No new activity" is a normal result. "Failed" is only for platforms that could not be read, and a failed platform keeps its old timestamp so the next run retries.
- **Personal chats are skipped entirely.** Mixed chats log only the project parts.
- **Nothing is published or sent automatically.**

## Status
Working daily for personal use. This repository contains the design, templates and a sample dashboard. It does **not** contain any of my conversations, images, account identifiers or real usage numbers.
