# Diet & Training Audit — 2026-10-12

_Window audited: 2026-07-26 → 2026-10-11 · Performed by Claude Code at the user's request ("thorough analysis on my diet and workouts … what I'm doing well and my biggest levers … backed by science")._

## Scope and data coverage

| Source | What was used |
|---|---|
| `meals/2026-07…10.md` / `dashboard.html` `NUTRITION_LOG` | 57 **complete** days (510 logged items). Excluded per `README.md` → Logging coverage: 3 partial days (8/11, 8/28, 10/10) and 18 untracked days (8/12–8/17, 9/19–9/21, 9/26–10/4). 10/12 excluded (in progress). |
| `workouts/*.md` | ~40 logged sessions (gym + cardio) |
| `PROGRESS.md` | Weigh-ins (gym scale 7/27–9/4; home scale 10/5 →), e1RM history |
| `GOALS.md`, `ROUTINE.md`, `NUTRITION.md` | Goals, programming, targets, calibration protocol |

**Coverage caveat:** ~27% of calendar days in the window are partial or untracked, mostly social/alcohol and travel days. Every intake average below covers complete days only, so true average intake is higher than the logged average. That makes the main finding (no deficit) more certain, not less.

## Key numbers

| Metric | Value | Notes |
|---|---|---|
| Avg intake, complete days | **1,944 kcal** (N=57) | Target was ~1,840 |
| — Weekdays | 1,862 kcal (N=43) | On target |
| — Weekends | **2,197 kcal** (N=14) | +335/day vs weekdays → ~+670 kcal/week |
| Day-to-day SD | 358 kcal | 12 days >2,100; 5 days <1,600 |
| Avg protein | **150 g** (~2.1 g/kg @ 72 kg) | ≥130 g on 44/57 days; ≥120 g on 52/57 |
| Avg fat / carbs | 67 g / 192 g | |
| Items estimated (vs label/official) | 97 / 510 (19%) | High logging precision |
| Gym-scale weight 7/27–9/4 | 163.8–165.8 lb, flat | Logged intake ~1,990 kcal/day over that stretch → that's maintenance |
| Home-scale baseline 10/6–10/12 | 156.2–159.4 lb; 7-day avg ~157.4 | 10/11–10/12 inflated by the 10/10 untracked beer evening |

By month (complete days): Jul 2,045 kcal / 155 g P (N=6) · Aug 1,992 / 155 (N=23) · Sep 1,878 / 148 (N=22) · Oct 1,902 / 138 (N=6).

## What's going well

1. **Protein.** 150 g/day is at the top of the evidence range. Morton et al. 2018 (*Br J Sports Med*, meta-analysis of 49 RCTs) found gains in lean mass level off around 1.6 g/kg/day, with the upper 95% confidence bound at about 2.2 g/kg. Higher intakes are recommended during a deficit (Helms et al. 2014, *JISSN*).
2. **Volume and frequency.** In normal weeks: ~12–15 direct sets per muscle and each muscle trained twice a week in full-body sessions. Schoenfeld, Ogborn & Krieger 2017 (*J Sports Sci*) found a dose-response for weekly sets with clear benefits at 10 or more. Training a muscle at least twice a week matches or beats once a week (Schoenfeld et al. 2016).
3. **Effort.** Sets are routinely taken close to failure. Robinson et al. 2024 (*Sports Med*) found hypertrophy improves as sets get closer to failure.
4. **Conditioning quality.** Zone 2 runs stay 91–94% in zone. The 4x4s include 10–14 minutes in Zones 4–5. Helgerud et al. 2007 (*MSSE*): 4x4 intervals raised VO2max more than steady-state running. Schumann et al. 2022 (*Sports Med* meta-analysis): concurrent training doesn't reduce hypertrophy.
5. **Weekday nutrition discipline.** Weekdays averaged 1,862 kcal, essentially on target.
6. **Logging accuracy.** 81% of logged items come from labels or official nutrition info.
7. **Lifts still going up after 10 years of training and near-maintenance eating.** Low cable row 175×15 → 190×14. Lat pulldown 175×15 → 190×12. Weighted lunges 135×15 → 225×10. DB curl 30s → 40s. Lying leg curl e1RM 98 → 160 lb.
8. **Back-safe exercise selection.** No disc flare-ups in 11 weeks.

## Biggest levers (ranked)

### 1. Create a real calorie deficit — **IMPLEMENTED 2026-10-12**
- Weight was flat for 6 weeks on the gym scale at ~1,990 kcal/day logged, before counting untracked days. True maintenance is about 2,000–2,100 kcal.
- The 1,840 target was only about 150 kcal under maintenance on paper. The actual average (1,944) left close to no deficit at all.
- `NUTRITION.md`'s calibration protocol says to cut 100–150 kcal when weight isn't moving after 2–3 weeks. That step was never applied after 7/27.
- **Change:** **1,700 kcal weekdays / 1,900 kcal weekends**. Weekly average ≈1,757/day, about 300–350 kcal below maintenance. Expected pace: ~0.6–0.7 lb/week (~0.4–0.5% BW/week).
  - Garthe et al. 2011 (*IJSNEM*): athletes losing ~0.7% BW/week kept or gained lean mass. Those losing 1.4%/week didn't.
  - Helms et al. 2014: 0.5–1%/week recommended for lean, trained people.
- **Endpoint:** Lean mass is about 127–129 lb, so 15% body fat ≈ 149–151 lb on the home scale. That's 6–8 lb from the ~157 baseline, or roughly 8–12 weeks.
- **Why weekends get a separate budget:** Weekend over-eating is a well-documented pattern (Racette et al. 2008, *Obesity*). Budgeting for it is more sustainable than expecting weekends to look like weekdays.

### 2. Bring alcohol nights under control and log them — _recommendation, not yet implemented_
- Untracked beer evenings (8/11, 8/28, 10/10, plus travel) are the largest unmeasured calorie source.
- Alcohol after exercise cut muscle protein synthesis by 24–37% even when protein was eaten with it (Parr et al. 2014, *PLoS One*).
- The 10/10 night produced a +2.4 lb water-weight spike that hid the real trend for 2–3 days.
- **Recommendation:** At most one night a week. Log a rough estimate instead of marking the day untracked. Don't drink on lifting-day evenings.

### 3. Progressive overload — add load when you hit the top of the range — _recommendation, not yet implemented_
| Lift | Prescribed reps | Current performance | Since |
|---|---|---|---|
| DB lateral raise | 12–15 | 25 lb × 15 | 7/28 (tied 6+ times) |
| Weighted dips | 8–12 | +45 × 15 | 8/5 (above the top of the range for 2 months) |
| Weighted pull-ups | 6–10 | +45 × 10 | 7/27 (tied 4×, then dropped from rotation after 8/24) |
| Incline DB press | 8–12 | 65 × 12 | 8/22 (one 70×11 on 9/1) |

- `ROUTINE.md`'s own rule ("once the top of a rep range is hit … add weight") isn't being applied to these lifts. Progressive overload is the core driver of continued gains in trained lifters (ACSM 2009 position stand; Plotkin et al. 2022).
- **Recommendation:**
  - Dips: +55–60 lb.
  - Incline press: 70s as the first set.
  - Lateral raise: 27.5–30 lb strict, or progress on a cable or machine.
  - Bring weighted pull-ups back on Day 1.

### 4. A minimum plan for travel and disrupted weeks — _recommendation, not yet implemented_
- 9/6–10/4: one lifting session logged in four weeks, a mix of Hyrox taper and travel. 9/22–9/25 had complete food logs but no lifting logged.
- Strength and size can be maintained with as little as one session a week at about a third of normal volume, as long as the weights stay heavy (Spiering et al. 2021, *JSCR*).
- **Recommendation:** "Travel minimum" = 2 × 30-minute full-body sessions a week, with 2 hard sets each of a press, a pull, a squat pattern and lateral raises.

### 5. Leave 1–2 reps in reserve on early compound sets — _recommendation, not yet implemented_
- Incline press goes 12 → 7 → 6 when set 1 is taken to failure.
- In trained lifters, failure vs. stopping 1–2 reps short gives similar hypertrophy, but failure costs more fatigue (Refalo et al. 2023 and 2024, *Sports Med*).
- **Recommendation:** Stop 1–2 reps short on early compound sets. Keep failure for last sets and machine isolation work.
- This doesn't change `ROUTINE.md`'s 0-RIR *logging* default. That default is about estimating e1RM from how sets actually went, not about how hard to train.

### 6. Measure body fat change beyond the scale — _partly implemented_
- Lifts going up while weight holds steady could be recomposition, but scale weight alone can't show it.
- **Implemented:** The dashboard's bodyweight chart now plots a trailing 7-day average of home-scale weigh-ins.
- **Recommendation:** Weekly waist measurement at the navel (morning) and progress photos every 2 weeks.

## Smaller items (recommendations only)
- **Creatine gummies:** Creatine itself is well supported (Kreider et al. 2017, ISSN position stand). Independent lab tests in 2024–25 found many gummy brands contain much less creatine than labeled. Plain monohydrate powder at 3–5 g/day is cheaper and reliable, and drops ~50 kcal/day of gummy sugar.
- **Satiety while dieting:** The Idahoan pouch = 440 kcal / 12 g protein / ~1,960 mg sodium. Ultra-processed diets drove ~500 kcal/day higher intake when people ate freely (Hall et al. 2019, *Cell Metab*). Rice or potatoes plus more vegetables will make 1,700 easier to stick to.
- **Fiber:** Covered adequately by Metamucil, vegetables and berries.
- **Calves:** Excluding direct calf work was justified for Hyrox. The race is over, so 2–3 sets twice a week is cheap if aesthetics matter.
- **Gym switching:** Different machines at the two gyms make progress hard to read. Progress each exercise at one gym, or keep separate per-gym baselines (already partly done).
- **Sleep:** Not logged, though WHOOP tracks it. One night of sleep deprivation cut muscle protein synthesis ~18% (Lamon et al. 2021).
- **Stale goal:** `GOALS.md` still lists Hyrox (9/20) as upcoming.

## Changes made on 2026-10-12 as a result of this audit
1. **Calorie targets:** 1,700 kcal weekdays / 1,900 kcal weekends. Protein stays at a 130 g floor. Fat 60/65 g, carbs 160/200 g. Files: `NUTRITION.md`, `GOALS.md`, `PROGRESS.md` (Nutrition Calibration Log), `meals/2026-10.md` header.
2. **Dashboard target logic:** `dashboard.html` now uses a date-aware `TARGET_SCHEDULE`, so each day is judged against the target in effect that day. Days 7/27–10/11 keep the flat 1,840; days from 10/12 use weekday/weekend targets.
   - Today tab: macro bars and runway use the day's own target and show a Weekday/Weekend badge.
   - 14-day trend: per-day target marks and shaded weekend columns.
   - Weekly Review: the 7-day target is the sum of each day's target, and there's a per-day "Kcal Target" column with ± vs target.
   - Nutrition Target History card: new 10/12 row.
3. **Bodyweight data:** At the user's request, all pre-home-scale weigh-ins were removed from the dashboard. That covers `WEIGH_INS`, the weigh-in table, the chart and the Weigh-ins tile (21 → 8). They stay in `PROGRESS.md` as raw history.
   - The chart was rebuilt around the home scale and adds the 7-day moving average.
   - The 10/5 bedtime setup reading is plotted but left out of the average.

## Next check-in
**~2026-10-26** (2 weeks on new targets), per the `NUTRITION.md` calibration protocol:
- Compare the home-scale 7-day average with today's ~157.4 lb.
- Expect about −1.2 to −2 lb.
- If it's flat, cut another ~100 kcal.
- If it's falling faster than 1.5 lb/week, add ~100 kcal back.
