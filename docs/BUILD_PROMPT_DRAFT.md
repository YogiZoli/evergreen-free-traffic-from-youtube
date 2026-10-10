# BUILD PROMPT (DRAFT, do not run yet)

Status: draft parked on 2026-10-10. Run only after the design session closes the open questions in README.md. Placeholders are marked `TBD`.

```
You are a senior full-stack builder and YouTube growth strategist. Task: build "YT Flywheel Creator" v1, a standalone SaaS that turns a course creator's niche into an evergreen YouTube flywheel.

READ FIRST
- README.md in this repo (decisions and open questions).
- Drive doc "23_Strategy_Session_2026-10-09_Decisions_v2" (ID 186ItPPhgGbKyS1H0XKNd6qxiebeDHs3hTgwoG8AmBas). Do not reopen decisions listed there.
- My existing skills: yt-flywheel-team:agent-01-channel-strategist, agent-02-seo-title, strategic-launch-orchestrator. They hold the flywheel logic. Reuse it, do not invent a new framework.
- Lead Magnet #3 repo YogiZoli/brand-channel-wizard: the Evergreen Traffic Card .md format it exports.

ARCHITECTURE
- Railway service plus a database (TBD: Postgres on Railway or Neon). Same deployment pattern as my C2C and PDT apps.
- Zero AI calls and zero paid APIs on my side. Keyword research runs in the user's own AI app with their own vidIQ.
- Unified brand design: use my shared design system (repo YogiZoli/brand-frames, as used by vidrev, PDT, IdeaToVideo).

FLOW
0. Login (TBD: magic link email).
1. Choose a door:
   A. Research Prompt Packet: requirements gate first (vidIQ account plus Claude or ChatGPT with the vidIQ connector; block until confirmed). The app gives one copy-ready prompt; the user runs it and pastes results back.
   B. Upload an Evergreen Traffic Card .md from the Brand Channel Wizard and skip research.
2. Flywheel plan: pillars, one playlist per pillar, ordered video list per playlist (TBD: video types).
3. Per video: a Video Brief (title, target keyword, hook, structure, CTA to a lead magnet), downloadable as .md (schema TBD, shared with IdeaToVideo).
4. Progress board: each video planned, in production, published. The user returns and sees what is next.
5. Final CTA: one line to my 6-pillar cohort program (constant PROGRAM_URL).

ACCESS
- v1 is a GoHighLevel affiliate bonus (TBD: how affiliate signup is verified).

CONSTRAINTS
- English UI. No emojis anywhere. No dashes as sentence punctuation.
- Mobile first, premium look.
- Private repo.

DELIVERABLES
- Live Railway URL
- 5-line summary: data model, where the constants are, how to test both doors.
```
