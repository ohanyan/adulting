---
name: conscious-spending
description: Monthly Conscious Spending Plan check-in (Ramit Sethi). Lighter-weight than money-date. Reviews whether actual spending matched intentional categories this month, flags drifts.
---

# /conscious-spending

Monthly check-in against the Conscious Spending Plan defined in `/money-date`. Faster. 15-20 minutes.

## Step 1: Pull the month

From whatever budgeting tool the user uses (Monarch, YNAB, Copilot, Mint replacement, bank categories):

- Total income this month.
- Total spending by bucket (Fixed, Invest, Save, Guilt-free).
- Any categories that jumped vs. last 3-month average.

## Step 2: Bucket check

Compare actuals to targets:

| Bucket | Target | Actual | Flag |
|--------|--------|--------|------|
| Fixed | 50-60% | <%> | |
| Invest | 10%+ | <%> | |
| Save | 5-10% | <%> | |
| Guilt-free | 20-35% | <%> | |

For each bucket that is off target, ask one question:
- Over-target? Was this a one-off (big vet bill, surprise fix, gift) or a drift?
- Under-target on invest/save? Did automation fire? If not, why not?

## Step 3: Money dial check

The money dials from the last money date — were they honored?

Example: if you dialed UP on "travel with family" this quarter, did any of this month's spending reflect that? A trip planned, a flight booked, a weekend away?

If you dialed DOWN on something (restaurants, clothes, whatever), did this month's spending reflect that, or did the habit win?

The dials are a promise to yourself. This is the accountability check.

## Step 4: Anomaly scan

Flag anything:
- One-time charges over a threshold (set by user).
- Subscriptions that should have been caught (run `/bills-and-subs` if more than one zombie shows).
- Categories 50%+ above baseline (groceries, gas, whatever).
- A new recurring charge you don't recognize.

## Step 5: Sinking funds

Are the sinking funds on track?

- Vacation fund: still projected to hit goal by target date?
- Tax fund: on track for April?
- Car fund (replacement or repair)?
- Gift fund (for the holidays)?

If any are behind, either adjust the monthly contribution or adjust the goal.

## Step 6: One adjustment for next month

Pick ONE thing to change next month:
- Move $X/month more into investments.
- Cap guilt-free at $Y.
- Freeze a specific category for the month.
- Set up a new sinking fund.

One. Not a portfolio of heroic fixes. One change, tracked.

## Output

Append to `~/adulting-data/journal/spending-log.md`:

```
# Spending review — <month, year>

## Actuals vs. targets
Fixed:       <%>  (target 50-60%)  <flag>
Invest:      <%>  (target 10%+)   <flag>
Save:        <%>  (target 5-10%)  <flag>
Guilt-free:  <%>  (target 20-35%) <flag>

## Dials honored?
Up: <categories and whether spending matched>
Down: <categories and whether spending matched>

## Anomalies
- <item>

## Sinking funds
- Vacation: <status>
- Taxes: <status>
- <other>: <status>

## Adjustment for next month
<one thing>
```

## The month-to-month reality

No month will be perfectly on target. That is fine. The goal is a trend:

- Over 6 months, is the invest bucket trending up?
- Over 6 months, is guilt-free trending toward your actual values?
- Over 6 months, is net worth growing?

If yes on all three, the system is working. Adjust the small stuff, not the big stuff.
