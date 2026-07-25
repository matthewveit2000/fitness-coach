# Fitness Coach

Personal training log and coaching notes. Training mix: weightlifting, running/cardio, and bodyweight/calisthenics. Primary goals: hypertrophy, staying lean, general athleticism and health.

## Structure

- `GOALS.md` — current goals and target metrics, updated as they evolve
- `ROUTINE.md` — the current training plan/split
- `PROGRESS.md` — bodyweight, measurements, and lift/run PRs over time
- `workouts/` — one log file per month, individual workout entries go here

## Workflow

Workouts get logged by telling Claude what happened in a session; Claude records it in the appropriate `workouts/YYYY-MM.md` file and updates `PROGRESS.md` when a PR or notable measurement comes up.
