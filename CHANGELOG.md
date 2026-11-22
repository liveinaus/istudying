# Changelog

## v0.1.1

Points and rewards, a daily test, hints, and support for more than one family.

Points, rewards and tests

- Points for every test: 100 for full marks plus a 20 point bonus, scaled by score; practice earns half
- Practice is scored question by question: full points first try, fix points (50%) on a later try, none if the
  answer is shown. "Fix my mistakes" pays fix points once per question, so it can't be repeated for points
- Rewards kids can ask for (screen time, staying up, toy credit) with weekend discounts; points are only taken
  when a parent approves. Kids see how to earn points on their points page
- Daily test kids start themselves, on chosen days, with an adjustable expiry
- Change the time limit of a test that's already going; test defaults (type, time limit, number of questions)
  in Settings
- The iPad screen stays on during a test

Hints and practice

- In practice the answer stays hidden until the kid gets it right, runs out of tries or asks to see it
- A 💡 hint appears after a wrong first try: a nudge, never the answer or the steps
- Parents can see, edit or rewrite any hint; hints travel with question Export and Import

Question bank

- Search by text, and by kid: done or not, first answer wrong, always right first time, last answer right or
  wrong, answer shown. Shows what the kid first answered, and whether they fixed it later
- "Answers from kids" shows each kid's first and final answer for a question
- Export (everything matching the filters) and Import that merges: questions already in the bank aren't
  added again, only their missing hint or explanation is filled in
- Retire (red) instead of Delete, and Bring back for retired questions
- Question sources have plain names and link to the original story or problem, with the reference on hover

Families

- More than one family: each family has its own link (/<12 characters>), parents, kids, tests, points, rewards and
  settings. The question bank and AI service are shared and managed only by the admin.
- Admin "Families" page: add a family and copy its link, rename, switch off, delete, set a parent's password
- Settings shows the family link, for setting up another iPad
- Upgrading moves the existing install into the first family; its first parent becomes the admin
- AI limit per family: 100 requests a month by default (Hobart time), changed by the admin; the admin's
  family has no limit. Once used up, kids get general tips instead. Parents see their usage in Settings.

Fixes

- The database works on bind-mounted data folders owned by another user
- Practice answers picked but not checked are marked when the practice is finished
- Copy link works on plain HTTP and iPad, checkboxes are normal size, the Delete button text shows

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
