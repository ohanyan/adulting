---
name: father-review
description: Weekly self-assessment as a father, per kid. Five dimensions scored 1-5, with one repair and one commitment per kid. Parallel to partner-review but zoomed in on each child.
---

# /father-review

(Named "father" because that was the asker. Works identically for any parent. Rename in your own fork if you want.)

Run this once a week. It takes longer if you have multiple kids because you run it per kid.

If the user did not say which kid, list the kids they have registered in `~/adulting-data/people/` and either run through all of them in sequence, or ask which one.

## The five dimensions (per kid)

Score each 1 (not this week) to 5 (showed up fully). One-sentence reason.

### 1. Presence

- Was I actually with them when I was with them? Phone down, eye contact, knees on the floor?
- Did they get at least one undistracted 1:1 hour?
- When they tried to show me something, did I look, or mumble "uh huh"?

Score: ___ / 5

### 2. Listening more than correcting

- When they told me about their day, did I ask a follow-up question, or move straight to advice?
- Did I let them be wrong about something without correcting?
- Did I ask "what do you think?" before telling them what I think?

Score: ___ / 5

### 3. Struggle within safety (Mogel / Greene)

- Did I solve things for them that they could have worked out?
- Did I let them be bored? Be frustrated? Try and fail?
- Or did I over-engineer their life to remove discomfort?
- A skinned knee test: is the thing I'm stepping in to prevent DANGEROUS, or just UNCOMFORTABLE? If uncomfortable only, step back.

Score: ___ / 5

### 4. Modeling what I tell them to be

- If they grew up to act exactly like I did this week, would I be proud?
- Where did I ask them to regulate when I was dysregulated myself?
- Where did I ask them to be honest when I fudged?
- Where did I ask them to apologize when I didn't apologize for something I did?

Score: ___ / 5

### 5. "I love you" and "I was wrong"

- Did I say "I love you" plainly this week, not just at bedtime?
- Did I say "I was wrong, I'm sorry" when I was, this week?
- Dr. Becky: repair is the most important thing a parent does. Every rupture is an opportunity. Every un-repaired rupture is a lesson I did not mean to teach.

Score: ___ / 5

## The two commitments per kid

1. **One thing to repair this week.** If there is something unrepaired (a yell, a phone-distracted dismissal, a promise I forgot), either repair it today with `/repair`, or schedule it for tomorrow.

2. **One specific thing to give them this week.** In their love language. Could be 10 minutes of 1:1. Could be a note in their lunchbox. Could be a walk.

## The age-aware reminder

Print a reminder appropriate to the kid's age (from their registry):

- **Under 5:** They learn from your tone more than your words. Calm, slow, on their level. Hug rate matters more than almost anything.
- **5-10:** Attention is currency. They are watching which things make your eyes light up. Make sure it is them.
- **10-13:** Their world is shifting. You will be corrected more and sought out less. Do not take it personally. Keep showing up at their rhythm.
- **13-18:** You are losing them to peers, by design. Your job is to remain a safe harbor they return to. Do not lecture. Do not interrogate. Be available. Drive them places. Long car rides are gold.
- **18+:** Shift from parent to trusted elder. Ask, don't direct. Keep calling.

## Output

Append to `~/adulting-data/people/<kid>.md`:

```
## Father review — <date>

Presence:            <score>/5 — <reason>
Listening:           <score>/5 — <reason>
Struggle in safety:  <score>/5 — <reason>
Modeling:            <score>/5 — <reason>
Love / repair:       <score>/5 — <reason>

Total: <sum>/25

Repair owed: <what, by when>
Commitment this week: <what, day>
```

## The line to end on

Remind the user: "They will not remember most of what you said. They will remember how it felt to be around you."
