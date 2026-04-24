---
name: annual-physical
description: Medical checkups tracker. Primary care, dentist, eye, derm, age-appropriate screenings, plus the labs most men never get but should. Run annually, or when you realize you haven't seen a doctor in too long.
---

# /annual-physical

The default path for most men is: no doctor until something hurts. Then diagnosis, then treatment of a problem that had been building for a decade.

Peter Attia's "Medicine 3.0" inverts this. Screen for the things that kill and cripple most adults, early, with eyes open.

## The core six (every year)

1. **Primary care (PCP) annual.** General physical, vitals, weight, blood pressure, medication reconciliation.
2. **Dental cleaning.** 2x/year for most adults. Gum health is linked to cardiovascular disease.
3. **Vision check.** Every 1-2 years. More often after 40.
4. **Dermatology skin check.** Annual, especially if any sun history. Skin cancer is easy to beat if caught early.
5. **Blood work.** See panel below.
6. **Mental health check.** Every 6-12 months honest self-check, or a therapist session.

## The blood panel that most men never ask for

Beyond the standard CBC/CMP, ask for:

- **APOB.** The single best lipid marker for cardiovascular risk. Better than LDL alone. Most docs won't order it unless you ask.
- **Lp(a).** Inherited. You want to know once, early. If it's high, treatment path matters.
- **Fasting insulin.** Metabolic health marker. Rises years before glucose does.
- **HbA1c.** Average blood sugar. Want it well under 5.7.
- **hs-CRP.** Inflammation marker.
- **Homocysteine.** Cardiovascular and neurodegenerative risk.
- **Testosterone (free and total).** If over 30, useful baseline. Declines matter.
- **Vitamin D, 25-hydroxy.** Most people are deficient.
- **Ferritin.** Iron stores. Matters for fatigue, training recovery.
- **B12.**
- **Full thyroid panel (TSH, free T3, free T4).** Not just TSH.

If your PCP resists ordering these, that is data about your PCP. You can order many of these through direct-to-consumer labs if needed.

## Age-specific screenings

### 30s
- Everything above.
- Mental health baseline.
- Fitness assessment: VO2 max test, DEXA scan for body comp and bone density.

### 40s
- Everything above.
- First colonoscopy at 45 (per updated ACS guideline).
- Coronary artery calcium (CAC) score. Cheap, non-invasive, powerful predictor.
- Consider CGM trial (continuous glucose monitor) for 2 weeks to see post-meal patterns.

### 50s
- Everything above.
- Repeat colonoscopy per doctor.
- Prostate conversation with PCP or urologist (PSA is controversial; have the conversation).
- Repeat CAC every few years.

### Any age, if you have the history
- Family history of early heart disease → CAC earlier, APOB dialed in.
- Family history of cancer → earlier screening in that line.
- Family history of Alzheimer's → discuss APOE4 testing, engage aggressively on lifestyle.

## Women's health note

This plugin was written by a male author and frames some items around men's common blind spots. Women have their own under-ordered labs (ferritin, thyroid, hormones, DEXA) and screenings (pap, mammogram, bone density). Modify this list for your own context or gender. Get the version of this skill in your doctor's language.

## Dental and vision

- Dental: cleanings 2x/year, full x-rays every 2-5 years, honest conversation about gum pockets.
- Vision: 2 years is fine if stable. After 40, baseline glaucoma check.

## Derm

Annual full-body skin check. Any mole that is changing, asymmetric, or new: get it checked sooner.

## The tracker

Ask the user to populate (or load) `~/adulting-data/medical.md`:

```
# Medical tracker — <name>

## Providers
PCP: <name, phone, last seen>
Dentist: <name, last seen>
Eye: <name, last seen>
Derm: <name, last seen>
Therapist: <name, last seen>

## Scheduled
<appointment> — <date> — <provider>

## Last done
Annual physical: <date>
Blood work: <date>
Dental cleaning: <date>
Derm skin check: <date>
Eye: <date>
Colonoscopy: <date>
CAC score: <date>
DEXA: <date>

## Conditions and meds
<list>

## Known family history
<list>
```

## What is due

For each item in the tracker, compute if overdue, due this quarter, due this year.

Output:

```
# Medical status — <date>

## Overdue (book today)
- <item> — last: <date>, standard cadence: <...>

## Due this quarter
- <item> — last: <date>

## On track
- <item>

## Actions to book in the next 7 days
- <item> — <provider, estimated call>
```

## The follow-through

Ask the user: for the top 3 overdue items, block a 15-minute calendar slot this week to make the calls. The calls take longer than the appointments. Nobody gets to the appointment without making the call first.

## The honest bar

If the user has not seen a PCP in more than 2 years: today, this week, book that one first. Everything else can cascade from a good PCP visit with a comprehensive panel.
