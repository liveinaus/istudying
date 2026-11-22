# Changelog

## v0.1.0

First version, for family use.

- Kids sign in on the iPad by tapping their picture and typing a 4-digit PIN; the parent area has its own password
- Parent sets each kid's year level and difficulty for Maths and Reading
- Practice (answers straight away), test (answers at the end) and exam (strict timer) modes, 30 minute default
- Wrong answers go on a mistake list and come back in later tests until answered right twice
- "Fix my mistakes" practice kids can start themselves
- Step-by-step explanations; AI explanations (any OpenAI-compatible service, with presets for Vercel AI Gateway,
  Meta Muse, Anthropic and OpenRouter) saved as drafts for the parent to approve
- "I still don't get it" tries up to three different explanations before suggesting a parent helps
- AI answers are cleaned up for kids: plain maths (12 ÷ 3 = 4) instead of LaTeX, no filler
- Print any test as A4, with a separate answer sheet
- Question bank with JSON import, source filter and bulk "Make all live"
- About 1,900 questions, all in Australian English:
  - 49 starter questions (live)
  - 1,450 maths word problems from GSM8K (MIT), adapted for Australia, Years 3 to 6 (drafts)
  - 180 original NAPLAN-style maths questions for Years 3 and 5 (drafts)
  - 40 StoryWeaver reading texts (CC BY 4.0) with 240 NAPLAN-style questions (drafts)
- Works as a Home Screen app (PWA)
