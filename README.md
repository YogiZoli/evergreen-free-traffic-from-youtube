# Evergreen Free Traffic from YouTube

> **Superseded on 2026-10-23. Not built.** The method now lives in the YouTube Evergreen Flywheel mini course (lead-magnet slot lm3) and in the Playlist Planner inside IdeaToVideo. Kept for reference only. See Drive doc 26_Course_Creator_Universe_Map_and_Build_Order.

Working name: **YT Flywheel Creator**. Lead magnet #4 of the Template 1 (Course Creator) set.

Status: **PARKED (concept only, not built).** Saved here on 2026-10-10 so the thinking is not lost. Build starts only after Lead Magnet #3 (Brand Channel Wizard) ships and its Evergreen Traffic Card format is final.

Source of truth for the wider strategy: Drive doc `23_Strategy_Session_2026-10-09_Decisions_v2` (ID `186ItPPhgGbKyS1H0XKNd6qxiebeDHs3hTgwoG8AmBas`).

## What it is

The core of the Ownership Method: turn a course creator's niche into an evergreen YouTube flywheel. It tells the creator which videos to make, in which playlist, in which order, and gives a ready brief for each video. The value grows over time: the user comes back, sees which videos are done and which one is next.

## Decisions so far

| Topic | Decision |
|---|---|
| Product type | Standalone SaaS, not a static page. It must remember state (channels, playlists, video progress) over weeks. |
| Hosting | Railway (same as C2C and PDT), plus a database. Not GitHub Pages. |
| Distribution | First as a GoHighLevel affiliate bonus (free access for users who sign up through the affiliate link), next to vidrev.app and PDT. Same code can later become a paid SaaS; only the access gate changes. Long term it is the base the "1000 small businesses" template runs on. |
| Relation to Lead Magnet #3 | Fully independent app. No code shared. The only link is a file: the **Evergreen Traffic Card .md** exported by the Brand Channel Wizard. |
| Keyword research | Same pattern as #3, no API on our side. Door A: the app gives a Research Prompt Packet the user runs in their own Claude or ChatGPT with their own vidIQ connector, then pastes results back. Door B: the user uploads an existing Evergreen Traffic Card .md and skips research. Gemini is out (no vidIQ connector). |
| Requirements shown at the start | vidIQ account (free plan works) plus Claude or ChatGPT with the vidIQ connector. Blocks until confirmed (Door A only). |
| Output per video | A **Video Brief** export (.md): title, target keyword, hook, structure, CTA to a lead magnet. Works with any video tool (HeyGen etc.). |
| IdeaToVideo | Stays internal (doc 23: not for sale, zero support). It reads the same Video Brief file, so on Zoltan's own channels a Flywheel plan becomes a video in one step. Making it a public bonus would need a separate decision in doc 23. |

## Open questions (resolve in the design session)

1. Exact output model: pillars, playlists, video order, video types (pillar, supporting, short).
2. What is stored per user, and the minimum login method.
3. Final Evergreen Traffic Card .md schema (shared contract with #3).
4. Final Video Brief .md schema (shared contract with IdeaToVideo).
5. How the affiliate bonus access is verified.

## Files

- `docs/BUILD_PROMPT_DRAFT.md`: draft prompt for the implementation chat. Not final; update it after the design session.
