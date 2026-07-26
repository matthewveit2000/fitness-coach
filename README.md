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
