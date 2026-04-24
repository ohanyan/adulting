---
name: training-plan
description: Weekly training plan built around Peter Attia's "Centenarian Decathlon" framework. Zone 2, strength, stability, VO2max. Usage is /training-plan. Asks about the week, produces a specific schedule.
---

# /training-plan

Peter Attia's core frame: you are training now for the physical tasks you want to be able to do at 85. Not to look good at 45. The muscle, aerobic capacity, and stability you build in your 30s, 40s, and 50s is the tax you pay to have a good marginal decade.

The modern protocol has four components. Most people neglect at least two.

## The four components, weekly

### 1. Zone 2 aerobic (3+ hours/week)

- Conversational pace. You can talk, but barely sing.
- Measured by heart rate (~60-70% max) or feel.
- Protects mitochondrial function, metabolic health, cardiovascular health.
- Options: walking inclined (incline treadmill, rucking), cycling, rowing, swimming, easy jogging.
- Split across 3-4 sessions of 45-60 min, OR one long session + shorter ones.

### 2. Strength (3x/week)

- Compound movements. Squat, deadlift (or trap-bar), bench, row, pull-up, overhead press, carry.
- Progressive overload. Track weight or reps, nudge up.
- Floor targets for a healthy adult:
  - Deadlift 1-1.5x bodyweight for reps.
  - Farmer's carry your bodyweight 60 seconds.
  - 10 strict pull-ups.
  - Push-ups: 20+ consecutive.
- Add grip, core, glute work. Weak glutes = future back problems.

### 3. VO2 max intervals (1x/week)

- The 4x4 protocol: 4 minutes at very hard effort (can barely talk), 4 minutes easy, repeat 4 times.
- Do this on a bike, rower, or hill. Not a flat run, unless you are experienced.
- VO2 max is the single best predictor of all-cause mortality. Protect and grow it.

### 4. Stability and mobility (2-3x/week)

- DNS (Dynamic Neuromuscular Stabilization) or Foundation Training.
- Hip mobility, thoracic spine mobility, single-leg balance.
- This is the boring one everyone skips. It is also the one that prevents the back injury that ends everything else.

## Step 1: What is this week?

Ask the user:
- How many days can you train this week? (Count realistically.)
- Any time-of-day constraints?
- Any physical flags? (Injury, tight something, recovery from illness, travel.)
- Any days where the cognitive/emotional load makes hard training wrong?

## Step 2: Build the week

Default template for a 5-day week:

| Day | Morning | Notes |
|-----|---------|-------|
| Mon | Strength — lower (squat / deadlift focus) | Priority |
| Tue | Zone 2 — 60 min (bike, ruck, swim) | Recovery |
| Wed | Strength — upper (push/pull focus) | |
| Thu | Zone 2 — 45 min + 10 min stability | |
| Fri | VO2 intervals — 4x4 | Priority |
| Sat | Long Zone 2 — 75-90 min | Outdoor |
| Sun | Stability, mobility, walk | Recovery |

For 4 days: collapse Thu into optional; keep strength 2x, Zone 2 2x, intervals 1x.

For 3 days: Mon strength, Wed Zone 2 + intervals, Fri strength.

Adjust by constraint. If travel week, ruck in the hotel gym, do hotel-room bodyweight, walk everywhere.

## Step 3: The one thing most miss

Ask: "Are you doing any stability work?"

Most people answer no. Press: "Which of these 5 can you do?"

- Single-leg stand, eyes closed, 30 seconds, each leg.
- Deep bodyweight squat (heels down, chest up), held 60 seconds.
- Hanging from a pull-up bar for 60 seconds.
- Farmer carry your bodyweight for 60 seconds.
- Touch your toes without bending knees.

If 2 or more of those are shaky, stability/mobility becomes the priority for 8 weeks.

## Step 4: Fuel and recovery

Quick check:
- Protein target: aim for 0.8-1.0g per lb goal bodyweight daily. Most under-eat protein.
- Sleep: run `/sleep-protocol` if sleep is slipping.
- Hydration + electrolytes around training.
- Alcohol capped. Drinking in training weeks degrades everything.

## Step 5: Output

```
# Training plan — week of <date>

## Schedule
Mon: <...>
Tue: <...>
Wed: <...>
Thu: <...>
Fri: <...>
Sat: <...>
Sun: <...>

## Priority sessions (don't miss)
- <...>
- <...>

## Stability focus this week
<specific drill>

## Notes
- Body state this week: <...>
- Missed last week: <...>, moved to: <...>

## Calendar
Put sessions on the calendar now. Not "I'll fit it in." Blocks.
```

## The Centenarian Decathlon check (quarterly)

Once per quarter, not weekly: ask "What are the 10 physical tasks I want to be able to do at 85?"

Examples:
- Pick up a 30-lb grandchild off the floor.
- Hike a 5-mile trail with 1,500 ft elevation.
- Get up off the floor without using hands.
- Travel alone, carry my own luggage.
- Swim a lap pool.
- Walk 3 miles without stopping.

For each, what is the training today that makes that possible? Reverse engineer. That is the real plan.
