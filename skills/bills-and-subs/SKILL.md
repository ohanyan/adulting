---
name: bills-and-subs
description: Monthly bills and subscriptions audit. Surfaces every recurring charge, flags duplicates and zombies, and guides cancellation or renegotiation. Run the first Sunday of each month.
---

# /bills-and-subs

The median American household is leaking 15-25% of their subscription spend on services they no longer use. You are probably paying for something right now that you forgot you signed up for.

This skill is the audit. 20 minutes, once a month.

## Step 1: Pull the list

Sources to check, in order:

1. **Credit card statements**, all cards, last 30 days. Search for "recurring" if your bank supports it.
2. **Bank account**, same period.
3. **Apple subscriptions:** Settings → [your name] → Subscriptions.
4. **Google Play subscriptions:** play.google.com/store/account/subscriptions.
5. **Amazon:** Your Account → Memberships and Subscriptions.
6. **Domain and hosting:** registrars, AWS, Vercel, Railway, Supabase, etc.
7. **SaaS you use for work:** are any personal-card expenses that should be on the company card?
8. **Charity and nonprofit recurring gifts.**

Capture every recurring charge into `~/adulting-data/subscriptions.md`.

## Step 2: The three buckets

For each subscription, ask the user: bucket 1, 2, or 3?

### Bucket 1: Keep.
You use it. You love it. It provides value worth the price.

### Bucket 2: Renegotiate.
You use it. But you are paying the default price. Call (or use a service) to negotiate.
- Cable / internet: call every 12 months.
- Cell phone: check the family plan; check per-line cost.
- Insurance (car, home, umbrella): re-quote every 24 months minimum.
- Streaming bundles: audit for overlap. Do you have both Disney+ and Hulu separately?

### Bucket 3: Cancel.
You don't use it, or the value is not worth the price, or it is a zombie you forgot about.

The test: "If this were not already a subscription and I was seeing it for the first time today, would I sign up at this price?" If no, cancel.

## Step 3: Common zombies to look for

Checklist, ask the user to scan:

- [ ] Gym memberships at a gym you haven't been to in 2+ months.
- [ ] Streaming services you have not watched in 30+ days.
- [ ] Cloud storage you don't need (duplicated across Apple, Google, Dropbox).
- [ ] Domains you registered and never used.
- [ ] Substack / newsletter subs that are piling up unread.
- [ ] Paid apps that do what a free one does.
- [ ] Audible credits piling up.
- [ ] Magazine / newspaper digital subs that auto-renewed.
- [ ] Free trials that converted to paid without you noticing.
- [ ] Insurance add-ons (rental car coverage that your CC already provides, etc.)

## Step 4: The cancel sprint

Cancel the Bucket 3 items TODAY. Not "this week." Today. The longer you wait, the more you pay.

For each, capture:
- Date cancelled.
- Refund requested (Y/N).
- Effective end date.

If a service makes cancellation hostile (dark patterns, chat bots, phone-only), note it. Never re-subscribe to those.

## Step 5: Bills review

Review fixed monthly bills:

- Mortgage / rent — know the exact number, and the portion that is principal vs. interest vs. escrow.
- Utilities — watch for anomalies month over month.
- Insurance — all of it, once a year, re-quote.
- Auto loans / lease.
- Student loans.
- Childcare.
- Tuition.

If any jumped 10%+ this month without explanation, investigate.

## Step 6: Autopay hygiene

- Which bills are on autopay? (Good.)
- Which are on the best credit card for category rewards? (Optimize.)
- Are any autopays pulling from an account that doesn't always have the money? (Move them.)

## Step 7: The "money dial" check (Ramit Sethi)

Once a quarter, not monthly: look at the cancel list. Is there one category where you cut mercilessly but actually want to spend MORE? Travel with the family. Good coffee. Books. Meaningful gifts.

Ramit's point: cut savagely on what you don't value. Spend extravagantly on what you do. Do not live in the middle on everything.

## Output

```
# Bills & subs audit — <date>

## Recurring charges, total
$<X>/month   |   $<X>/year

## Kept (<count>)
<table>

## Renegotiating (<count>)
- <service>: called <when>, result <...>

## Cancelled this month (<count>)
- <service>: cancelled <date>, saves $<X>/year

## Annual savings from this audit
$<X>

## Flag for next month
- <item to monitor>
```

End with one line: "The cheapest raise you can give yourself is cancelling what you're not using."
