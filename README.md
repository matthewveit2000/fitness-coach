# Fitness Coach

Personal training log and coaching notes. Training mix: weightlifting, running/cardio, and bodyweight/calisthenics. Primary goals: hypertrophy, staying lean, general athleticism and health.

## Structure

- `GOALS.md` — current goals and target metrics, updated as they evolve
- `ROUTINE.md` — the current training plan/split
- `NUTRITION.md` — calorie/macro targets and the calibration protocol
- `PROGRESS.md` — bodyweight, measurements, and lift/run PRs over time
- `workouts/` — one log file per month, individual workout entries go here
- `meals/` — one log file per month, meals logged from a chat description or photo
- `dashboard.html` — tabbed HTML dashboard (Overview/Goals/Routine/Nutrition/Progress) summarizing everything above; published as a Claude artifact and regenerated whenever the source files change

## Workflow

Workouts get logged by telling Claude what happened in a session; Claude records it in the appropriate `workouts/YYYY-MM.md` file and updates `PROGRESS.md` when a PR or notable measurement comes up. Meals get logged the same way — describe what you ate or send a photo, and Claude estimates macros and records it in `meals/YYYY-MM.md`. Whenever any of `GOALS.md`, `ROUTINE.md`, `NUTRITION.md`, or `PROGRESS.md` change, `dashboard.html` gets regenerated to match and republished to the same artifact link.

**Date handling for logs:** every entry gets logged under the date the message describing it was received. **Determine that date by checking the actual current date/time in Mountain Time (the user's timezone) — e.g. `TZ=America/Denver date` — and log under that date automatically, without confirming with the user.** (This replaces an earlier version of this policy that required confirming every date; as of 2026-07-30 the user asked to stop being asked and have dates just looked up in Mountain Time instead.) Never infer a date from conversational phrasing ("last night," "this morning," "today") when it conflicts with the actual Mountain Time date. Log something under a different date only when the user explicitly asks for it (e.g. "log this for yesterday") — otherwise always use today's actual Mountain Time date.
