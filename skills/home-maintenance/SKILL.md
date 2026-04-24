---
name: home-maintenance
description: House and car maintenance radar. Rotating checklist of filters, batteries, fluids, inspections. Reads from your home inventory and tells you what is due. Run monthly.
---

# /home-maintenance

A house is a system with dozens of subsystems, each with a maintenance cadence. If you don't track them, they will track you: a furnace that fails in February, a water heater at 4 a.m., a car battery in a parking garage.

This skill keeps you ahead of it.

## Step 1: Load inventory

Read `~/adulting-data/home-inventory.md` if it exists. If it does not, walk the user through creating one from `data/home-inventory.template.md`.

Minimum inventory items (adapt to the user's home):

**HVAC and air**
- Furnace filter (replace every 3 months, more often with pets)
- AC service (annual, spring)
- Humidifier filter (season-specific)
- Range hood filter (every 6 months)

**Water**
- Water heater flush (annual)
- Water softener salt (monthly check)
- Whole-house water filter (as spec'd, usually 6-12 months)
- Refrigerator water filter (every 6 months)
- Shutoff valve function (annual)

**Safety**
- Smoke detector batteries (annual, daylight saving change is a common trigger)
- CO detector batteries (annual)
- Fire extinguisher check (annual, check gauge)
- Sump pump test (spring and fall)
- Circuit breaker labels correct (annual walk)

**Exterior**
- Gutter clean (spring and fall)
- Roof inspection (annual, visually after any major storm)
- Dryer vent cleaning (annual — this is a fire risk)
- Foundation inspection (annual walk)
- Window and door seals (annual)

**Seasonal**
- Winterize outdoor faucets (fall)
- Tree trim (as needed, winter dormant season)
- Lawn / garden schedule (season-specific)
- Driveway sealing (every few years)

**Appliances**
- Dishwasher filter (quarterly)
- Washing machine hose inspection (annual)
- Refrigerator coil vacuum (annual)
- Garage door maintenance (annual — lube rollers, check cable)

**Cars (per vehicle)**
- Oil change (every X miles or months — check manual)
- Tire rotation (every 5-7,500 miles)
- Tire tread and pressure (monthly)
- Brake inspection (annual)
- Registration renewal (annual, state-specific)
- Insurance renewal (annual)
- Inspection sticker (state-specific)
- Wiper blades (annual)

## Step 2: What is due

For each inventory item, compare last-done date vs. cadence. Surface:

**Overdue** (past due date, red flag)
**Due this month**
**Due next month**
**On track**

Present a short prioritized list. The overdue list first.

## Step 3: Book the next action

For the top 3 items on the list, ask:
- Is this DIY or do I need a pro?
- If DIY, when will I do it? Put it on the calendar.
- If pro, do I have a trusted name? Book it, or ask for a referral.

Do not leave this skill with "I'll do it soon." Give specific days.

## Step 4: Update inventory

When items are done, the user updates `~/adulting-data/home-inventory.md`:

```
## Furnace filter
Replaced: 2026-04-23
Next due: 2026-07-23
Size: 20x25x4
Notes: Buy 3 at a time from [vendor]. MERV 11.
```

The notes field is critical. It is where you record the answers to questions Future You will not remember: which filter size, which HVAC tech, which plumber's number, which brand of softener salt.

## Step 5: Vendor rolodex

Maintain a list of trusted vendors in the inventory file:

```
# Vendors
HVAC: [Name, phone, last used]
Plumber: [Name, phone]
Electrician: [Name, phone]
Handyman: [Name, phone, rate]
Roofer: [Name, phone]
Landscaper: [Name, phone]
Mechanic (Car 1): [Name, phone]
Mechanic (Car 2): [Name, phone]
```

When you are standing in a puddle at midnight, you do not want to be Googling plumbers.

## Output

Return:
```
# Home Maintenance Status — <date>

## Overdue (<count>)
- <item> — <days overdue>
- ...

## Due this month
- <item> — <date>
- ...

## Due next month
- <item> — <date>
- ...

## Actions to book today
- <item, DIY or pro, proposed date>
```

Then ask: "Want me to draft any vendor messages, or block time on the calendar for the DIY ones?"
