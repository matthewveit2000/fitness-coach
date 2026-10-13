# Nutrition

_Last updated: 2026-10-12_

## Why this exists
Training determines the stimulus; body composition change (leaner + hypertrophy) is driven at least as much by intake. This was the single biggest gap found in the last routine audit — there was a body-fat target in `GOALS.md` but nothing about food.

## Targets (current — see Calibration below)
**Revised 2026-10-12 — weekday/weekend split, real deficit.** The 10/12 audit (`audits/2026-10-12-diet-training-audit.md`) found ~11 weeks at maintenance: gym-scale weight sat flat at 163.8–165.8 lb from 7/27–9/4 while logged intake averaged ~1,990 kcal/day, and across all 57 complete days intake averaged 1,944 kcal (weekdays 1,862, N=43; weekends 2,197, N=14). That puts true maintenance at ~2,000–2,100 kcal once untracked social/travel days are counted, so the old 1,840 target was only a ~150 kcal deficit on paper and ~0 in practice. This applies the calibration protocol's "not moving → cut" step below, which hadn't been run since 7/27, and budgets weekends explicitly instead of pretending they look like weekdays.

| | **Weekdays (Mon–Fri)** | **Weekends (Sat–Sun)** | Basis |
|---|---|---|---|
| Calories | **~1,700/day** (range 1,650–1,750) | **~1,900/day** (range 1,850–1,950) | Weekly avg ~1,757/day ≈ 300–350 kcal below estimated true maintenance → ~0.6–0.7 lb/week (~0.4–0.5% BW/week). Within the 0.5–1%/week range that preserves lean mass in trained lifters (Helms 2014; Garthe 2011) |
| Protein | **~130g/day** (floor; 140–150g preferred) | **~130g/day** | Unchanged. You've averaged 150g (~2.1 g/kg) — keep that; it's the top of the evidence range (Morton 2018) and matters more in a deficit |
| Fat | **~60g/day** | **~65g/day** | Trimmed 5g on weekdays to make room; still well above the ~0.5 g/kg hormonal-health floor |
| Carbs | **~160g/day** | **~200g/day** | Fills the remainder; extra weekend carbs land on the days that usually carry the bigger social meals |

Weekday vs. weekend = the calendar day (Mountain Time). Past days are always judged against the target that was in effect that day — `dashboard.html`'s `TARGET_SCHEDULE` encodes both the old flat 1,840 target (7/27–10/11) and this split (10/12 →).

**Weigh-in reading for this phase:** judge progress on the dashboard's 7-day moving average of home-scale weigh-ins, not single days. Expected pace: −0.8 to −1.1 lb/week at most; if the 7-day average falls faster than ~1.5 lb/week for 2+ weeks, add ~100 kcal back. Endpoint: ~149–151 lb on the home scale ≈ 15% body fat at current lean mass, ~8–12 weeks out.

### Previous target (2026-07-27 → 2026-10-11, superseded)
**Revised again 7/27**: maintenance bumped to ~2,000 kcal/day per your own judgment that WHOOP underestimates — consistent with the known bias (wearables tend to underestimate resting energy for higher-lean-mass/muscular individuals), just a larger correction than the ~1,850 estimate first applied. Your read on your own body's response is a legitimate input here, on top of the device data.

| | Target | Basis |
|---|---|---|
| Calories | **~1,840/day** (range 1,750–1,950) | Maintenance ~2,000 (WHOOP + your correction) · same mild ~8% deficit as before |
| Protein | **~130g/day** (range 120–140g) | **Revised 7/30 per your request** — ~0.8g/lb bodyweight (~159–164lb baseline), down from 1.0–1.2g/lb. Still comfortably above the ~0.7g/lb floor most muscle-retention-in-a-deficit research converges on, just less padding above it than before |
| Fat | **~65g/day** minimum | Restored to the original level now that there's more calorie room — was only trimmed to 55g because the lower ~1,700 ceiling needed the space for carbs |
| Carbs | **~185g/day** | Fills the remainder — the lower protein target freed up ~45g of the calorie budget, which rolls into carbs (helps with the training-fuel issue from the 7/27 under-fueling incident); flex this around training days if performance/recovery suffers |

**Calories are still the main lever for the leaning-out goal.** _(The table above under "Previous target" is kept for history — current numbers are the weekday/weekend table at the top of this section.)_ Protein's no longer being held as a hard floor above what's needed for muscle retention — hit ~130g most days, but it's not worth stressing over on a day it comes up short the way it was at 175g.

**History:** 2,200 (initial formula) → 1,700 (WHOOP-anchored) → 1,840 (WHOOP + your correction that it underestimates) → **1,700 weekdays / 1,900 weekends** (10/12 audit — weight trend showed 1,840 was effectively maintenance). If strength, recovery, or energy noticeably suffer before the next scheduled check-in below, that's itself a signal to nudge calories up further — don't wait for the 2–3 week mark if training is clearly degrading.

## Why a moderate deficit, not aggressive
At 10 years of training experience, simultaneous muscle gain + fat loss ("recomposition") is still achievable — research confirms it isn't just a beginner phenomenon — but it's slower and more dependent on execution than it would be for a newer lifter, and requires high protein + a genuine training stimulus + only a mild deficit. An aggressive cut risks losing the muscle you're training hard for. This is set up for **modest, steady change, not a fast cut.**

## Calibration protocol (this is the part that actually matters)
The numbers above are still a *starting estimate* — WHOOP's burn number is better information than a population formula, but it's still an estimate with its own error margin, not ground truth. Actual weight-trend data is what actually settles it:
1. Weigh in regularly (already tracked in `PROGRESS.md`) — home scale, morning, minimal clothing; read the 7-day average, not single days.
2. After 2–3 weeks, check the trend:
   - Losing ~0.5–1% of bodyweight/week → on track, keep going.
   - Not moving → drop calories ~100–150/day.
   - Losing faster than ~1%/week → that's muscle-loss risk territory, add ~100–150/day back.
3. **Actually run this check every 2–3 weeks** — next one due ~2026-10-26 (2 weeks into the new targets). The 10/12 audit found it had gone unrun for ~11 weeks while weight sat flat. Re-adjust every 2–3 weeks rather than reacting to single days — bodyweight fluctuates daily from water/sodium/glycogen.
4. Don't wait for the scheduled check-in if training performance (strength, recovery, energy) drops off noticeably — see the note above.

## Logging — flexible, conversational
No app, no manual macro lookup required. Just tell me what you ate, in whatever form is easiest:
- **Describe it in chat** ("had 2 eggs, toast, and a protein shake for breakfast") — I'll estimate calories/protein/fat/carbs and log it.
- **Send a photo** of the meal or the nutrition label — I'll read the label directly if there is one (exact, not estimated), or estimate from the photo if not.
- **Whenever a restaurant or store/brand name is mentioned, search online for official nutrition info first** (their site, a published nutrition PDF, etc.) before falling back to an estimate. Large chains usually publish full nutrition breakdowns; smaller regional chains often don't — note in the log entry whether the number came from an official source or an estimate either way, so confidence level is always visible at a glance.
- Entries go in `meals/YYYY-MM.md`, one file per month like the workout logs, with a running daily total against the targets above.
- **When a message describes multiple food items for one meal, log each item as its own line with its own calories/macros — never blended into a single combined line.** They still count toward the same meal (e.g. "Lunch") and the same daily total, but each item's numbers stay visible individually so you can see what any one thing actually cost you.
- Estimates are approximate, not lab-precision — that's fine, consistency over weeks matters more than precision on any single meal, and the calibration protocol above corrects for estimation error using real weight-trend data anyway.
- **Dates: logged under the date the message was received, not inferred from phrasing like "last night" — see `README.md` Workflow for the full policy.**
- **Context from past history & staples:** When an item is mentioned without specific brand or variant details (e.g. "milk", "fairlife shake", "burrito"), check recent history in `meals/` and Preferred Staples below to determine the established product/portion before falling back to generic estimates or picking a random brand variant.
- **Explicitly state all assumptions in responses:** Every logging response must clearly state any assumptions made (e.g. which product variant was assumed from history, estimated portion or gram weights, cooking fats) so that catching and correcting any differences is frictionless.

## Preferred Staples
Default items to assume when logging, unless a photo or description says otherwise:
- **Protein shake:** Premier Protein Vanilla, 11 fl oz — 160 kcal, 30g protein, 3g fat, 4g carbs _(replaced the fairlife Nutrition Plan shake as of 2026-07-28)_; **Pumpkin Spice variant:** 11.5 fl oz — 160 kcal, 30g protein, 3g fat, 2g carbs, 230mg sodium _(label confirmed from bottle photo 2026-10-05)_
- **Granola bar:** Kirkland Signature 100 Calorie granola bar — 100 kcal, 1g protein, 3g fat, 18g carbs _(exact, from label — established staple)_

## Notes
- Update the targets table above if the calibration protocol calls for a calorie adjustment, or if your actual activity level turns out meaningfully different from "moderate."
- Alcohol, sauces/oils, and cooking fats are easy to undercount — mention them when describing a meal rather than assuming they're negligible.
- **Standing habit, not logged:** Metamucil (sugar-free orange, 2 heaping tbsp) every morning — added 2026-08-11. Calories are negligible so it's not added to the daily meal log or totals, but it's a real daily fiber source (~6g soluble fiber/dose) and should factor into any fiber/nutrition-quality assessment — the diet isn't as fiber-deficient as the raw food log alone would suggest.
