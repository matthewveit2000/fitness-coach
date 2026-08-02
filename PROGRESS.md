# Progress

_Last updated: 2026-07-26_

## Bodyweight / Measurements
| Date | Weight | Notes |
|------|--------|-------|
| 2026-07-26 | 163 lb | Estimated body fat high teens-low 20s %, 5'6" |
| 2026-07-27 | 164.3 lb | Gym scale, after work, with shoes, on a padded floor — not directly comparable to the 7/26 reading (different conditions/time of day). Use same-conditions weigh-ins for the real trend once a pattern is established. |
| 2026-07-28 | 164 lb | Same conditions as 7/27 (gym scale, after work, shoes, padded floor) — comparable to that reading, down 0.3lb. Still not comparable to the 7/26 baseline (different conditions). |

## Lift PRs
| Lift | Weight x Reps | Date |
|------|---------------|------|
|      |               |      |

## Run PRs
| Distance | Time | Date |
|----------|------|------|
|          |      |      |

## Estimated 1RMs
Inferred from logged working sets via the Epley formula (see `ROUTINE.md` → Suggested Weights from Estimated 1RM), not from actual 1RM testing. Updates only when a set implies a higher number than what's on file, like a PR. Empty until a set is logged for that exercise.

**RIR default corrected again 2026-07-28** — history: 2 RIR (original) → 1 RIR (corrected 7/27, after a "struggling" session got estimated with the old +2 default anyway) → **0 RIR (corrected 7/28)**, after the 7/28 session was logged with no RIR mentioned, defaulted to 1 per the previous fix, and still produced suggested weights the user reported as unrealistic given how the session actually felt. Direct quote: *"I was struggling with all my workouts... I normally fail a rep at least once during one of my sets per workout."* That means near-failure effort is this athlete's baseline, not a noteworthy exception — so unstated RIR is now read as 0, not 1. The 6 entries below logged 7/28 are recomputed at RIR=0. `ROUTINE.md` also now applies a 90% training-max haircut when converting e1RM into a *suggested working weight*, to separately account for fatigue across multiple consecutive working sets in a session (a gap the per-set Epley formula doesn't cover) — the e1RM numbers below are the undiscounted estimate, not the training max.

**Gym-comparability caveat, added 2026-08-01** — 7/30, 7/31, and 8/1's sessions were all at Yellowstone Fitness rather than the usual gym; the user flagged that machines aren't perfectly comparable across facilities even at the same stated weight (resistance-curve/calibration differences are common on machines, less so on free weights). The three Yellowstone sessions are internally consistent with each other, but any exercise with **both** an older non-Yellowstone number and a newer Yellowstone one should be read as two data points from different equipment, not a clean before/after strength comparison — flagged inline below wherever that applies. "Laying Leg Curl" (8/1) is additionally likely a different machine variant (lying/prone) than whatever "Leg Curl" was measured on previously, so it's tracked as its own line rather than overwriting the existing one.

| Exercise | Est. 1RM | Confidence | Based on (weight x reps, date) |
|---|---|---|---|
| Incline DB Press | 82 lb | High (≤12-rep range) | 70lb x 5, failed 6th rep, 7/30 — a failed rep is direct/true failure data, not a RIR assumption |
| Weighted Dips | 60 lb added | High (≤12-rep range) | 45lb x 10 (x2 sets), 7/27 — RIR corrected to 0 (was 2); "struggling" + light-headed/nauseous partway through the session are direct evidence of near-failure effort, not 2 in reserve |
| Pec Deck | 240 lb | High (10-rep set) | 180lb x 10 (x2 sets), 7/30 — RIR=0 default; actual reps performed (8-10) are within the reliable ≤12 range even though the exercise is normally programmed at 12-15, so confidence is High for this entry specifically |
| Low Cable Row | 262.5 lb | High (12-15 rep range) | 175lb x 15, 7/31 — RIR=0 default; new PR, up from 253lb (7/28). ⚠️ 7/28 was a different gym than 7/31/8/1 (Yellowstone Fitness) — the jump may partly reflect equipment, not just strength. The 8/1 session (also Yellowstone) reproduced the same 175lb x 15 → 262.5lb exactly, which is a good internal-consistency check for Yellowstone's numbers at least. |
| Weighted Pull-Ups | 60 lb added | High (≤12-rep range) | 45lb x 10 (x2 sets), 7/27 — RIR corrected to 0 (was 2); same reasoning as Weighted Dips above |
| Lat Pulldown | 233 lb | High (10-rep set) | 175lb x 10, 7/30 — RIR=0 default |
| Arnold Press | — | High (≤12-rep range) | |
| Lateral Raise | 37.5 lb | Low — trend only (12–15 rep range) | 25lb x 15 (x2 sets), 7/28 — RIR corrected to 0 (was 1); 15-rep sets are past the formula's reliable range so treat as directional only. (8/1 session at Yellowstone Fitness best was 25lb x13, e1RM ~35.8 — didn't beat this, no change; also a different gym so not directly comparable anyway.) This is dumbbell lateral raise specifically — see the separate machine entry below for 8/2. |
| Lateral Raise (machine, Yellowstone Fitness — explicitly flagged by user) | 135 lb | High (10 & 15-rep sets agree closely) | 90lb x 15, 8/2 (100lb x10 gave a very close 133lb estimate — good cross-check). 90-100lb on a machine vs. 25lb dumbbells confirms this is a completely different exercise implementation, not a calibration quirk — tracked separately, not merged with the DB entry above. Suggested weight (if using this exact machine again): ~81–87lb for 3x12–15 |
| Reverse Pec Deck | 190 lb | High (8-rep set) | 150lb x 8, failed 9th rep, 7/30 — a failed rep is direct/true failure data; the 8-rep set beat the 15-rep set (120lb) that would otherwise have been the low-confidence entry. (8/2 session, same machine (Yellowstone) — best was 130lb x12, e1RM ~182lb, didn't beat this, no change.) |
| Leg Press | 735 lb | Medium (10–15 rep range) | 490lb x 15, 7/27 — RIR corrected to 0 (was 2); reported "struggling with the weight," which is direct evidence the set was near failure, not 2 reps shy |
| Weighted Lunges | 202.5 lb | Low — trend only (15-rep set) | 135lb x 15 (x3 sets), 7/31 — RIR=0 default; reps assumed per-leg to match the routine's prescription, flag if that's wrong |
| Leg Extension | 392 lb | High (12-rep set) | 280lb x 12, 8/1 (Yellowstone Fitness) — RIR=0 default; up from 322.5lb (7/28, different gym). ⚠️ This is a big jump (215→280lb) after only 4 days — likely reflects Yellowstone's machine being calibrated differently, not a genuine 20%+ strength gain. The 12-rep set is more reliable than the old 15-rep trend-only number, so it's recorded as the new estimate, but treat the suggested-weight jump with real skepticism until confirmed back at the usual gym. |
| Leg Curl | 322.5 lb | Low — trend only (12–15 rep range) | 215lb x 15, 7/28 — unchanged; see "Leg Curl (lying, Yellowstone)" below for the 8/1 session, which used a different machine variant and isn't merged into this entry |
| Leg Curl (lying variant, Yellowstone Fitness) | 98 lb | High (12-rep set, failed 13th) | 70lb x 12, failed 13th, 8/1 — a failed rep is true failure data. Not comparable to the "Leg Curl" entry above (different machine/variant and different gym); tracked separately |
| Leg Curl (seated?, Yellowstone Fitness — explicitly flagged by user) | 177 lb | High (8-10 rep range) | 140lb x 8, failed 9th, 8/2 — roughly double the "lying variant" weights (70lb) for a similar rep range, confirming this is a third distinct machine, not the same one. Suggested weight (if using this exact machine again): ~106–114lb for 3x12–15 |
| DB Curl | 49 lb | High (≤12-rep range) | 35lb x 12, 7/31 — RIR=0 default |
| Bench Press _(not in current routine — see Notes)_ | 233 lb | High (≤12-rep range) | 175lb x 10 (x2 sets), 7/31 — 2nd set explicitly "couldn't have done another," true failure |
| Hammer Curl | 60 lb | Medium (mix of ≤12 and 13–15 rep sets) | 40lb x 15 (best set), 7/28 — RIR corrected to 0 (was 1, though the math barely moves at 15 reps); the top set was at 15 reps (past the ≤12 reliable zone) even though the prescribed range is 10–12, so confidence is downgraded from the usual "High" for this exercise |
| Triceps Pushdown | 176 lb | High (≤12-rep range) | 135lb x 9, 7/28 — RIR corrected to 0 (was 1); user reported struggling with the whole session. (7/30 session best was 135lb x7 failed 8th, e1RM ~166.5 — didn't beat the recorded PR, so no change; a single lower day doesn't lower an e1RM. 8/2 session was notably lower still — 70lb x10, e1RM ~93 — likely fatigue from being the 14th exercise in a long session rather than a new machine, but flagging the pattern in case it recurs.) |
| Bodyweight Dips (max reps, no added weight) | 22 reps | Reference only — not an e1RM | 8/2, bodyweight only. Tracked as a separate capacity marker, not converted into the "Weighted Dips" e1RM above since it's a different loading context (0 added weight vs. a tested added-weight max). |
| Overhead Triceps Ext. | — | High (≤12-rep range) | |
| Crunches | n/a | Bodyweight core exercise — no meaningful 1RM | |

## Nutrition Calibration Log
Track calorie target changes here alongside the reasoning, so adjustments over time are traceable.

| Date | Calorie Target | Reasoning |
|------|----------------|-----------|
| 2026-07-26 | ~2,200 | Initial estimate — Mifflin-St Jeor formula, moderate-activity assumption |
| 2026-07-26 | ~1,700 | Revised same day — WHOOP measured ~1,800 kcal/day average burn (all days), notably lower than the formula estimate; real tracked data takes priority |
| 2026-07-27 | ~1,840 | Revised again — user's own judgment that WHOOP underestimates burn; maintenance bumped 1,800→2,000, same ~8% deficit reapplied |
