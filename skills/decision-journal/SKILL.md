---
name: decision-journal
description: Log an important decision with the reasoning behind it, so future-you can review whether the reasoning was sound (not just whether the outcome was good). Usage is /decision-journal [topic].
---

# /decision-journal

Humans are terrible at remembering why they decided something. We remember whether the outcome was good and then rewrite the reasoning to match.

A decision journal fixes this. It captures:
- What you decided.
- Why.
- What you expected.
- What you were uncertain about.

Later, you can look back and separate good decision-making from good outcomes. They are not the same thing. You can make a bad decision that works out (got lucky). You can make a good decision that doesn't (unlucky). Only the journal tells you which.

## Usage

`$ARGUMENTS` should be the decision, one line. "Accepting the board seat." "Hiring VP Eng." "Moving to Austin." "Putting Lucas in the new school."

If empty, ask.

## The nine fields

### 1. The decision

One clean sentence. "I am accepting the board seat at X company." "We are moving to Austin." "We are putting Lucas in Saint Anne's starting fall 2026."

### 2. The date and context

Date. A few sentences on the situation: what pressure, what opportunity, what is forcing the decision now?

### 3. The options considered

List 2-4 options you weighed. A decision with only one option was not a decision; it was a conclusion.

- Option A: ...
- Option B: ...
- Option C: ...

### 4. Why this option

The main reasons, in order. Try to name the top 3.

### 5. What do I expect to happen?

Concrete predictions, with timelines. Examples:
- "I expect the board seat to take 20 hours a month."
- "I expect the kids to take 3-6 months to settle in Austin."
- "I expect Lucas to be happier within 6 weeks of changing schools."

Being specific matters. Vague predictions are not falsifiable.

### 6. What could go wrong?

Pre-mortem. What is the thing that, a year from now, I would be kicking myself for? Name 3.

### 7. What am I uncertain about?

Not risks — uncertainties. Things where I do not know the answer and am guessing.

Examples:
- "I am uncertain whether the CEO is as steady as he presents."
- "I am uncertain how my partner will feel 6 months in."
- "I am uncertain if the interest rate will continue to rise."

### 8. What evidence would change my mind later?

What would I see in 3, 6, 12 months that would tell me this was the wrong call?

This is where most people fail. Decisions become identity, and we defend them rather than update. Writing in advance what would falsify the decision protects against that.

### 9. My confidence level

On a 1-10 scale, how confident am I in this decision? Most people default to 8-9 because they just made the decision and don't want to feel bad. Be honest. If this is a 6, write 6.

## The review cadence

Put a reminder on the calendar to review this decision at:
- 30 days
- 90 days
- 1 year

On each review, answer:
- What happened that I predicted? What didn't?
- What did I get wrong in the pre-mortem?
- Was I uncertain about the right things, or did I miss something entirely?
- Looking at the decision with the benefit of hindsight but the emotion removed, would I make the same decision again with the same information?

The last question is the one that separates good decision-making from good outcomes. It is possible the decision was good even though the outcome was bad. Don't over-update on single outcomes.

## Storage

Write to `~/adulting-data/decisions/<date>-<short-name>.md`:

```
# Decision: <one-line>

Date: <YYYY-MM-DD>
Context: <...>

## Options considered
- A: <...>
- B: <...>
- C: <...>

## Chosen: <A/B/C>

## Why
1. <...>
2. <...>
3. <...>

## Expected outcomes
- <...>
- <...>

## Pre-mortem (what could go wrong)
1. <...>
2. <...>
3. <...>

## Uncertainties
- <...>
- <...>

## Falsifying evidence (what would tell me I was wrong)
- <...>

## Confidence: <n>/10

## Review dates
- 30-day: <date>
- 90-day: <date>
- 1-year: <date>

---

## 30-day review (filled later)
<...>

## 90-day review (filled later)
<...>

## 1-year review (filled later)
<...>
```

## The kinds of decisions worth journaling

Don't journal every decision. Only ones that matter enough that you want to learn.

- Job changes.
- Hires, firings, promotions.
- Investments (business or personal, above a threshold you pick).
- Major family decisions (school, move, pet, etc.).
- Committing to long projects.
- Saying no to something big.
- Starting or ending a meaningful relationship.
- Health decisions.

If it matters in 5 years, it should be in the journal.

## Why this matters more than most people realize

Entrepreneurs, investors, and leaders who keep decision journals make systematically better decisions over decades than those who don't. It is one of the highest-leverage habits there is, and almost nobody does it, because the benefit is delayed by 12+ months.

Pay the cost now. Your future self will thank you.
