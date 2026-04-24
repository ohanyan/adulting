---
name: errand-batch
description: Group errands by location, urgency, and time-of-day. Optimizes the run so you do not make six separate trips. Run when the list has grown.
---

# /errand-batch

Errands are low-status work that eat disproportionate time. The fix is batching.

## Step 1: Pull the list

Check `~/adulting-data/errands.md` if it exists. Merge any items the user names now.

If it doesn't exist, walk the user through creating it. The list should include:

- Returns (with deadlines if any)
- Pickups (dry cleaning, prescriptions, packages)
- Drop-offs (donations, rentals)
- Shopping (Target/Costco/grocery runs with specific items)
- Paperwork trips (DMV, notary, bank)
- Appointments (already scheduled)
- Routine (oil change, car wash, haircut)

Each item gets:
- Name
- Location
- Deadline (if any)
- Time estimate
- Depends on anyone (e.g., tag along with kid, partner consent)

## Step 2: Cluster by location

Use a mental or literal map. Group items that are within a 5-minute drive of each other.

A good cluster = 3+ items in one 30-minute radius.

## Step 3: Time-of-day tactics

- DMV / notary / bank: mid-morning Tuesday-Thursday is the sweet spot. Never Mondays, never Fridays, never lunch.
- Costco: Tuesday morning or Thursday after 7pm. Weekends are a penalty.
- Grocery: right when they open, or late evening. Midday is chaos.
- Post office: early morning.
- Oil change: appointment, not walk-in.

If the user has a route, sort by time-of-day constraints first, then by location.

## Step 4: The "does this need me" filter

For each errand, ask:

1. Can someone else do this? (Partner, teenager, assistant, delivery service.)
2. Can this be automated? (Recurring order, subscription, auto-refill.)
3. Can this be deleted? (Do I actually need the returned thing? Is the dry cleaning worth the trip?)

Errands that do not need your physical presence should not be on your list. Delegate or automate. Be ruthless here. Your time is not for the DMV if it does not have to be.

## Step 5: The run plan

Output a clean sequenced plan:

```
# Errand run — <date>

## Plan: <morning | afternoon | evening>
Start: <location, time>
End: <location, time>
Estimated total: <minutes>

## Stops
1. <location> — <items> — <est time>
2. <location> — <items> — <est time>
3. <location> — <items> — <est time>

## Delegated / automated / dropped
- <item> → <how>

## Still on backlog
- <item> — <next candidate date>
```

## Step 6: Combine with something good

Errand runs pair well with:
- A podcast or audiobook you have been saving.
- A coffee or lunch pit-stop at a place you actually like.
- A friend who lives along the route (drop in).
- A walk in a park if there's one near a stop.

Do not suffer the errand. Make it a pleasant hour.

## Step 7: Update

After the run, check off items from the list, update `~/adulting-data/errands.md`.
