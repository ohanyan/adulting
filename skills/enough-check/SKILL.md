---
name: enough-check
description: Pre-big-spend sanity check against your "enough" statement and values. Run before any significant purchase (house, car, upgrade, large gift, big trip). 5 minutes.
---

# /enough-check

Before you spend meaningful money, run this 5-minute check.

This skill is not a veto. It is a pause. Most regretted purchases were not stopped because no one asked these questions.

## Usage

`$ARGUMENTS` should be the item and amount. "A new Tesla, $62k." "Kitchen remodel, $85k." "Ski trip to Japan, $15k." "Watch, $8k."

If missing, ask.

## The seven questions

### 1. What is this purchase actually buying?

Not the object. The experience or outcome. 
- The Tesla is buying: status? Daily comfort? Zero emissions conviction? All three? Be honest about the ratio.
- The kitchen is buying: functional improvement? Enjoyment of cooking? Resale value? Hosting pride? Be honest.
- The watch is buying: craftsmanship appreciation? Daily delight? A signal to others? A family heirloom?

Write the real answer in one or two sentences. If status is a big part, it is fine, but name it.

### 2. Is this on my "enough" statement?

Pull the statement from your last `/money-date`. Does this purchase move you toward the enough-state, or is it independent, or does it push that state further out?

If it pushes enough further out: is it worth the delay? Sometimes yes. Often no.

### 3. Is this aligned with my money dials?

From your CSP, which dials are UP this quarter? Is this purchase in one of those categories?

- Yes: proceed with confidence. You already decided this matters.
- No: why is this exception happening? Is this a dial you should be adjusting?

### 4. The 1% and 10% tests

- **1% test:** Is this purchase less than 1% of your net worth? If yes, proceed without further agonizing. This is a "just buy it" (Ramit) purchase.
- **10% test:** Is this more than 10% of your net worth? If yes, sleep on it for at least 30 days.
- Between 1% and 10%: this check.

### 5. The one-year question

"Will I be glad I bought this in one year?"

Not "will I still have it." Will I actively be glad.

- A $2,000 dinner jacket that fits perfectly and you wear 50 times a year: probably yes.
- A $2,000 espresso machine that will sit on the counter looking great but you actually use for drip coffee 80% of the time: probably no.
- A $40k extension on a home you plan to live in 20 more years: probably yes.
- A $40k bathroom remodel to a house you're selling in 2 years: maybe not.

### 6. The "if it broke tomorrow" test

"If this broke or disappeared one year from the purchase date, would I be devastated, annoyed, or indifferent?"

- Devastated: strong signal this mattered.
- Annoyed: maybe you'd replace it, maybe you wouldn't.
- Indifferent: you didn't need it.

### 7. The partner check

If you have a partner:
- Have you talked about this explicitly, not just mentioned it?
- Are you both enthusiastic, both neutral, or split?
- If split: do NOT proceed until you have talked about it for real. Use `/hard-conversation` if it's heavy.

There is no cumulative version of this rule that survives. Couples who make big financial decisions unilaterally erode trust. Do not do it.

## Step 2: The call

After the seven questions, ask the user:

"Based on your own answers above, what is the right call — buy it now, buy it but a different version, delay 30 days, or no?"

Whatever they say, respect it. This skill is not a ledger of NO. Sometimes the right answer is "yes, buy the thing you love." Especially when it aligns with the dials and you have the margin.

## Step 3: If yes

- Confirm the partner is aligned.
- Confirm you are paying in a way that doesn't spike debt.
- Put it on the books. Update the plan for the rest of the quarter.
- Enjoy it without guilt. Guilty spending is the worst of both worlds.

## Step 4: If delay

- Set a specific date (30 days from today).
- Put it on the calendar.
- Re-run the check on that date. If the answer is still yes, proceed without the meta-loop.

## Step 5: If no

- Write why. One sentence.
- Decide what you are doing with the money instead. Money saved on a "no" that then leaks into random spending is not saved.
- Release. Do not relitigate. A decided no is done.

## Output

Append to `~/adulting-data/journal/enough-checks.md`:

```
# <date>

Item: <...>
Amount: $<...>
% of net worth: <%>

## What it's actually buying
<...>

## Aligned with enough statement: <Y / N / unclear>
## Aligned with current money dials: <Y / N>
## 1-year-from-now feeling: <glad / neutral / regret>
## Partner aligned: <Y / N / not discussed>

## Decision: <buy | different version | delay 30 days | no>
## Rationale (one sentence): <...>

## If delay, revisit on: <date>
```

## The principle

Morgan Housel: "Modern capitalism is excellent at two things: generating wealth, and making you feel you don't have enough."

The "enough" check is a small friction, once, on the way to yes or no. Once you have it, the impulse to upgrade every 18 months quietly evaporates. You have more money AND more peace.
