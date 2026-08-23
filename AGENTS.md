# AGENTS.md — instructions for any AI agent working in this repo

This is a personal training/nutrition log, maintained by talking to an AI agent
(Claude, Google Jules, or others) instead of a dedicated app. Multiple different
agents may work on this repo at different times — **always assume you are not
the only one.** The rules below exist because specific mistakes have already
happened; each one names the failure it prevents.

`README.md`, `NUTRITION.md`, `ROUTINE.md`, and `PROGRESS.md` explain *why* the
project works the way it does. This file is the procedural checklist for *how*
to make an edit without breaking something — read it before touching any file,
every session, even if you've edited this repo before.

## 0. Before you write anything

- **Fetch/pull `main` first.** Another agent may have committed since your
  context was built. Never assume the files you have in context are current —
  re-read a file if there's any chance it changed underneath you.
- **Read the exact section you're about to edit, fresh**, not from memory of
  an earlier turn.

## 1. Repeated items are normal — don't "fix" them

If the same food or product appears on two different days in `meals/`, that is
the user eating the same thing twice, not a duplicate log entry. **Never merge,
delete, or re-date an entry because it matches an earlier day** — only remove
or change a log entry if the user explicitly says it was logged wrong. When in
doubt whether something is a real repeat vs. an actual mistake, ask; don't decide
silently either way.

## 2. Dates: Mountain Time, no exceptions

Log every entry under the actual current date **in Mountain Time**
(`TZ=America/Denver date`), never the date/timezone of your own runtime, and
never inferred from phrasing like "last night" or "this morning." Only use a
different date if the user explicitly asks for one (e.g. "log this for
yesterday"). See `README.md` → Workflow for the full policy.

## 3. Meal entries — required format

Every food line needs: description, kcal, protein, fat, carbs, and a source
tag in parentheses:
- `(exact, from label)` / `(official <brand> nutrition info, exact)` — read
  directly off a label or official source
- `(estimate — <one-line reasoning>)` — no label available; say what the
  estimate is based on

After every new item, recompute and append `**Daily total so far: ...**`;
switch to `**Daily total: ...**` (no "so far") only once you're sure the day
is over — check the current Mountain Time before closing a day out, since a
later entry can still land on that same date.

See `NUTRITION.md` for targets, staple-product defaults, and portion
conventions (e.g. banana peel discounted at USDA's 36% refuse figure).

## 4. Workout entries — required format

- Heading format: `## YYYY-MM-DD — <Session Type>` — always include the
  session type/day label (e.g. `Gym (Day 2)`, `Zone 2 Run (Cardio)`), never a
  bare date. If a gym session's exercise pairing matches one of the Day 1–5
  templates in `ROUTINE.md`, name it (e.g. `Day 4 — Extra Volume`); if it's a
  genuine mix, say so explicitly rather than leaving the type blank.
- RIR default is **0** (near-failure) unless the message says otherwise — see
  `PROGRESS.md`'s RIR history for why. A "failed Nth rep" set uses the reps
  *actually completed* (N−1) in the Epley formula, not N.
- e1RM formula: `weight × (1 + reps/30)` (Epley). Reliable to ~12 reps; past
  that, treat the result as directional and downgrade confidence accordingly
  (see existing entries in `PROGRESS.md` for the tone/format to match).

### 4a. The gym-comparability rule — mandatory, no exceptions

This user regularly switches between gyms/machines, and a pin-loaded machine
at 300lb can mean something completely different from one gym to the next.
**Before recording any new e1RM as validating or replacing an existing PR:**

1. Compare it to the *most recently confirmed* number for that exact
   exercise in `PROGRESS.md` (not just the single highest number on file —
   read the full history in that row).
2. If the new number is dramatically higher or lower (as a rule of thumb,
   more than ~15–20%) than a baseline that's been **confirmed more than
   once**, and the session didn't note a gym/machine change, **do not**
   assert the new number invalidates the old one. Instead:
   - Record the new data point as logged (never discard real performance
     data).
   - Add a flag, matching the tone of existing flagged entries in
     `PROGRESS.md` (search for "⚠️" in that file for examples) — name the
     specific prior baseline being contradicted and by how much, and say
     what would confirm or contradict it (typically: a follow-up session at
     a known gym).
   - Carry the same flag into the matching `ROUTINE.md` suggested-weight
     line(s) — **every** occurrence of that exercise (an exercise can appear
     on more than one day, see §5).
3. **Never delete, soften, or silently overwrite an existing caveat** written
   by a previous session — if new evidence changes the picture, add to the
   history, don't erase it.

This exists because `ROUTINE.md`'s suggested weights are numbers the user
actually loads onto a machine at the gym next session — an unverified inflated
number is a real injury/frustration risk, not just a data-quality nit.

## 5. Every markdown edit requires a *complete* dashboard sync

`dashboard.html` mirrors `GOALS.md` / `ROUTINE.md` / `NUTRITION.md` /
`PROGRESS.md` / `meals/*.md` / `workouts/*.md`. A **partial** sync is worse
than no sync — it makes the dashboard internally contradict itself, which is
harder to spot than a stale-but-consistent dashboard. On every commit that
touches any source file, update **all** of the following in `dashboard.html`:

- [ ] `NUTRITION_LOG` JS object — add/edit the day's item array
- [ ] `TODAY` — the current Mountain Time date
- [ ] Workout Log section — one new HTML block per session, in the same
      `<div class="callout info">...</div>` format as every existing entry
      (do not introduce a different structure like a bare `<ul><li>` list —
      grep the file for `class="callout info"` and match it exactly)
- [ ] Estimated 1RMs table — every exercise row whose `PROGRESS.md` line
      changed, including confidence label and any ⚠️ flag
- [ ] **Every** Routine-tab card that mentions the changed exercise — some
      exercises appear on more than one day (e.g. Leg Extension is on both
      Day 2 and Day 4). Grep the exercise name in `dashboard.html` after
      editing and confirm every occurrence changed, not just the first one
      you found.
- [ ] "What's Logged So Far" stat tiles — Workout Entries and Meal Entries
      counts (count real `## ` session headings in `workouts/*.md`,
      excluding the format-template header and untracked/vacation
      placeholders; count `NUTRITION_LOG` array items for meals)
- [ ] Header `sync-note` "last updated" date

**Before ending your turn**, grep the file(s) you just edited for the
exercise/date/value you changed and confirm every match was updated — not
just the first one you found.

## 6. Repo hygiene

- Never commit tool/runtime artifacts: `server.log`, `*.pyc`,
  `__pycache__/`, `node_modules/`, editor swap files, etc. `.gitignore`
  covers the common cases — extend it rather than committing around it. If
  you ran a local server or script to preview `dashboard.html`, clean up
  before committing.
- A commit should only touch files that are actually part of the logged
  change.

## 7. Coverage / gaps

See `README.md` → "Logging coverage and gaps" for the partial/untracked-day
rules (a day can be `partial`, `untracked`, or default `complete`) — get this
right before computing any average, total, or trend across multiple days.

## 8. Commit messages

Describe what was logged/changed in the first line (e.g. `Log 8/22 dinner:
pasta, chicken bites, sauce`), not a generic message. If you touched
`PROGRESS.md`/`ROUTINE.md` because of a PR or a flagged anomaly, say so.
