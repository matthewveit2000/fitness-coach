# Next Workout — Tailored Recommendation

_Generated: 2026-11-18 (Wed, Mountain Time) · accounts for every session logged through **2026-11-17** · plans against the week of **Mon 11/16 – Sun 11/22**_

> **What this file is.** From 2026-11-18 the fixed Day 1 → 5 rotation is retired: after **every** logged workout the agent regenerates this file with a recommended next session in **three options: 🏃 Cardio · 🏔️ Yellowstone Fitness · 🏢 Phillips 66**. The programming rules live in `ROUTINE.md` → *Adaptive Programming*; the step-by-step checklist is `AGENTS.md` §11. It is mirrored into `dashboard.html` → `NEXT_WORKOUT` (Today tab → 🎯 Next workout card; Train tab → full plan). Loads follow the 90%-training-max method in `ROUTINE.md` and the gym-comparability rule (`AGENTS.md` §4a): every gym option uses **that gym's** numbers only.

## Coach's call

**Lift: Legs & Arms, at whichever gym you're at (★).** Hamstrings and triceps are at **0 sets** this week and quads at 3. Chest, back and rear delts were trained Mon + Tue, so they sit this one out. Then get the Norwegian 4×4 in (no cardio in 10 days) and finish the week with an upper-body + hamstring session and a weekend Zone 2 run or hike.

## Inputs used

**Week so far (Mon 11/16 →, direct sets, counted the same way as the dashboard's Weekly Review):** 11/16 Yellowstone (Day 1 variant, 19 sets) + 11/17 P66 (mixed, partial, 10 sets).

| Muscle | Done | MEV floor | After either gym option | Status after |
|---|---|---|---|---|
| Chest | 6 | 8 | 6 | Next lift (+3–4) |
| Back | 8 | 10 | 8 | Next lift (+3–4) |
| Quads | 3 | 8 | **9** | ✅ ≥ MEV |
| Hamstrings | 0 | 6 | **4** | Next lift (+3) |
| Side delt | 3 | 6 | **6** | ✅ ≥ MEV |
| Rear delt | 3 | 6 | 3 | Next lift (+3) |
| Biceps | 3 | 6 | **6** | ✅ ≥ MEV |
| Triceps | 0 | 4 | **4** | ✅ ≥ MEV |
| Abs | 3 | 0 | 3 (+2–3 optional) | ✅ |

- **Last trained:** hamstrings & triceps 11/12 (6 days ago) · quads, side delts, biceps, abs 11/16 · chest, back, rear delts 11/17.
- **Cardio:** 0 sessions this week; last session 11/8 (hike), last Norwegian 4×4 11/4, last Zone 2 run 11/7.
- **Constraints:** lower-back disc (no loaded spinal flexion, no heavy axial loading) · right knee (quad work pain-guided) · ⚠️ flags carried from `PROGRESS.md` (Yellowstone leg extension 400 lb, hammer curl 45×20).
- **Preference signals applied** (see `ROUTINE.md` → Preference signals): since mid-September cardio gets its own day rather than being tacked onto a lift · the Day 2 superset flow you repeat most (knee-machine pair → lateral raise ↔ curl → triceps finisher) · each gym's staples (Yellowstone: BSS, lateral raise machine, 2:1 pushdown station; P66: leg press ↔ crunches, DB laterals) · you push sets past the top of the range, so each lift gets a rep-based cue.

## Option 1 — 🏃 Cardio: Norwegian 4×4 (treadmill) · ~40 min

_Pick this if today is a non-lifting day. Keep it at least 24 h away from the legs session._

| Block | Time | Target |
|---|---|---|
| Warm-up | 10 min | Easy jog, building into Zone 2 (138–151 bpm) |
| 4 × hard interval | 4 min each | ~7.7–8.5 mph (your 10/11 speeds) · HR ~167–182 bpm (WHOOP Z4–Z5; 11/4 plateaus were 175–182) |
| Recovery between | 3 min each (×3) | Walk / easy jog until HR is back to ~115–130 bpm |
| Optional 5th round | 4 + 3 min | Only if recovery HR still drops under ~130 (you added one on 11/4) |
| Cool-down | 5 min | Easy walk |

**Alternative:** if your legs are heavy or energy is low, do a Zone 2 run instead: 45–60 min at 138–151 bpm. You held 90%+ in-zone on 10/7 and 10/14.

## Option 2 — 🏔️ Yellowstone Fitness: Legs & Arms · ~55–60 min · 20 sets (+2 optional)

| Block | Exercise | Sets × Reps | Load | Last time at Yellowstone | Cue |
|---|---|---|---|---|---|
| Superset 1: Hamstrings ↔ Quads (leg machines) | Lying Leg Curl | 4 × 10–15 | ~101–114 lb | 120×15, 11, 10 (11/12) | 4 sets today: start at 120 and drop to ~110 if set 3 falls under 10. |
| | Leg Extension ⚠️ | 3 × 12–15 | ~288–309 lb | 400×10, 10, 8 (11/10, ⚠️ unverified) | Pain-guided (right knee). 400 × 10 stays flagged until repeated, so the suggestion stays ~288–309. |
| Superset 2: Quads ↔ Abs (DB area / mat) | Bulgarian Split Squat (DB) | 3 × 10–12/leg | ~48–50.5 lb/hand | 55×10, 10, 10 (11/12) | 55s for 10 on all 3 sets: chase 55 × 12 before going heavier. Stop on sharp pain at the knee bump. |
| | Crunches ⚠️ _(optional)_ | 2 × 20–30 | bodyweight | 30, 25, 15 (11/16) | Optional; swap to plank / Pallof press if the back feels tight. |
| Superset 3: Side delts ↔ Biceps | Lateral Raise Machine | 3 × 12–15 | ~88–94 lb | 110×10, 9, 100×10 (11/16) | You've done 110 × 10 for five sessions straight. Build reps in range at ~100 (12–15) instead of grinding 110 × 10. |
| | Hammer Curl (DB) | 3 × 10–12 | ~43.4–45.6 lb | 45×20, 20, 20 (11/10, ⚠️ Low confidence) | Try 50 × 10–12 on set 1. That gives a clean in-range read on the 45 × 20 sets. |
| Finisher: Triceps (cable) | Triceps Pushdown (2:1 station) | 4 × 10–12 | ~60–63 lb (2:1) · ~128.6–135 lb on the 1:1 stack | 60×10, 8, 7 (11/10, 2:1) | Keep every set at 8 reps or more. Drop 10 lb for the last set if needed. |

_2:1-station load derived from that station's own best (70 lb × 10 on 10/6 & 10/8 → e1RM 93.3 → 90% TM 84.0 → 60–63 lb for 10–12). It is not comparable to the 1:1-stack PR._

## Option 3 — 🏢 Phillips 66: Legs & Arms · ~55–60 min · 20 sets (+3 optional)

| Block | Exercise | Sets × Reps | Load | Last time at P66 | Cue |
|---|---|---|---|---|---|
| Superset 1: Hamstrings ↔ Quads (leg machines) | Leg Curl | 4 × 12–15 | ~194–207 lb | 215×15, 12, 12 (11/3) | 215 held 12+ reps on every set: stay at 215 and push for 15s. |
| | Leg Extension | 3 × 15–20 | 215 lb (P66 stack max) | 215×15, 18, 20 (11/3) | The stack is maxed, so progress with a 3-second lowering and a 1-second squeeze at the top. Pain-guided (right knee). |
| Superset 2: Quads ↔ Abs (leg press / mat) | Leg Press | 3 × 10–12 | ~445.5–501 lb → ~510 | 490×15, 15, 15 (11/9) | 490 × 15 on all 3 sets is the top of the range, so add load (~510) and work 10–12 (ROUTINE progression rule). |
| | Crunches ⚠️ _(optional)_ | 3 × 20–30 | bodyweight | 30, 25, 25 (11/9) | Optional; your usual P66 pairing. |
| Superset 3: Side delts ↔ Biceps (DB rack) | DB Lateral Raise | 3 × 12–15 | ~24–25.7 lb | 30×10, 25×10, 25×10 (11/9) | Use 25s in the 12–15 range; the 25 × 10 sets leave room to build reps. |
| | Hammer Curl (DB) | 3 × 10–12 | ~43.4–45.6 lb | 45×10, 10, 10 (11/3) | Try 50 × 10–12 on set 1 for a clean in-range read. |
| Finisher: Triceps (cable) | Triceps Pushdown | 4 × 10–12 | ~103–108 lb | 120×10, 9, 110×9 (11/3) | 4 sets this time: start near 105–110 so set 4 still reaches 10. |

_P66 pushdown load derived from P66's own data (120 lb × 10 on 11/3 → e1RM 160.0 → 90% TM 144.0 → ~103–108 lb for 10–12). The ~128.6–135 lb ROUTINE number comes from Yellowstone's 1:1 stack and overshoots at P66, as the 11/3 note in `PROGRESS.md` anticipated. The leg-press ~510 comes from the progression rule (top of range hit on every set), not from a new e1RM._

## Rest-of-week outlook

- **Next lift (Thu/Fri): upper body + hamstring top-off.** Chest 3–4, back 3–4, rear delts 3, leg curl 3, side delts 2–3. That puts every muscle at or above MEV by Sunday.
- **Cardio:** Norwegian 4×4 at least 24 h after the legs session, plus a long Zone 2 run or hike on the weekend (your 11/7–11/8 pattern). Target ≥2 cardio sessions per week.

## Recommendation history

_Fill in "What was done" at the next workout log (which option, swaps, skipped blocks). This is the feedback loop that tunes the preference signals in `ROUTINE.md`._

| Generated (MT) | Accounts for | Options offered | What was done | Notes |
|---|---|---|---|---|
| 2026-11-18 | through 11/17 (P66 mixed, partial) | 🏃 Norwegian 4×4 · 🏔️ YS Legs & Arms ★ · 🏢 P66 Legs & Arms ★ | _pending (fill in at next workout log)_ | First tailored recommendation; replaces the fixed Day 1→5 rotation. |
