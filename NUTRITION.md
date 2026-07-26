# Nutrition

_Last updated: 2026-07-26_

## Why this exists
Training determines the stimulus; body composition change (leaner + hypertrophy) is driven at least as much by intake. This was the single biggest gap found in the last routine audit — there was a body-fat target in `GOALS.md` but nothing about food.

## Targets (starting point — see Calibration below)
Revised using WHOOP's measured burn (~1,800 kcal/day average across all days, including training) as the primary signal, in place of the initial Mifflin-St Jeor formula estimate (~2,600) — real tracked data beats a population-average formula. Nudged slightly above the raw WHOOP number because wearables tend to underestimate resting energy for higher-lean-mass/muscular individuals, so 1,800 is likely a slight floor rather than the true number.

| | Target | Basis |
|---|---|---|
| Calories | **~1,700/day** (range 1,600–1,800) | Revised maintenance estimate ~1,850 (WHOOP-anchored) · ~8% deficit — kept mild since the maintenance estimate itself already carries uncertainty |
| Protein | **~175g/day** (range 160–195g) | 1.0–1.2g/lb bodyweight — unchanged even though calories dropped; protein needs stay high (or go up) in a deficit specifically to protect muscle, they don't scale down with calories |
| Fat | **~55g/day** minimum | Trimmed from the original 65g to leave more room for carbs at this lower calorie ceiling; still comfortably above the ~50g hormonal-health floor |
| Carbs | **~125g/day** | Fills the remainder — flex this around training days if performance/recovery suffers |

**Protein is the hard target — hit it consistently even on days calories drift.** Calories are the main lever for the leaning-out goal; carbs/fat are flexible around whatever's left after protein and the calorie target.

**This is a meaningful downward revision (2,200→1,700) and worth watching closely.** 1,700 kcal is low relative to your training volume (lifting 3–5x/week + running). If strength, recovery, or energy noticeably suffer before the next scheduled check-in below, that's itself a signal to nudge calories up ~100–150 — don't wait for the 2–3 week mark if training is clearly degrading.

## Why a moderate deficit, not aggressive
At 10 years of training experience, simultaneous muscle gain + fat loss ("recomposition") is still achievable — research confirms it isn't just a beginner phenomenon — but it's slower and more dependent on execution than it would be for a newer lifter, and requires high protein + a genuine training stimulus + only a mild deficit. An aggressive cut risks losing the muscle you're training hard for. This is set up for **modest, steady change, not a fast cut.**

## Calibration protocol (this is the part that actually matters)
The numbers above are still a *starting estimate* — WHOOP's burn number is better information than a population formula, but it's still an estimate with its own error margin, not ground truth. Actual weight-trend data is what actually settles it:
1. Weigh in regularly (already tracked in `PROGRESS.md`).
2. After 2–3 weeks, check the trend:
   - Losing ~0.5–1% of bodyweight/week → on track, keep going.
   - Not moving → drop calories ~100–150/day.
   - Losing faster than ~1%/week → that's muscle-loss risk territory, add ~100–150/day back.
3. Re-adjust every 2–3 weeks rather than reacting to single days — bodyweight fluctuates daily from water/sodium/glycogen.
4. Don't wait for the scheduled check-in if training performance (strength, recovery, energy) drops off noticeably — see the note above.

## Logging — flexible, conversational
No app, no manual macro lookup required. Just tell me what you ate, in whatever form is easiest:
- **Describe it in chat** ("had 2 eggs, toast, and a protein shake for breakfast") — I'll estimate calories/protein/fat/carbs and log it.
- **Send a photo** of the meal or the nutrition label — I'll estimate from that.
- Entries go in `meals/YYYY-MM.md`, one file per month like the workout logs, with a running daily total against the targets above.
- Estimates are approximate, not lab-precision — that's fine, consistency over weeks matters more than precision on any single meal, and the calibration protocol above corrects for estimation error using real weight-trend data anyway.

## Notes
- Update the targets table above if the calibration protocol calls for a calorie adjustment, or if your actual activity level turns out meaningfully different from "moderate."
- Alcohol, sauces/oils, and cooking fats are easy to undercount — mention them when describing a meal rather than assuming they're negligible.
