# adulting

A Claude Code plugin for grown-ups who want to show up well.

35 skills for the stuff nobody taught you: self-management, household ops, health, money, and the relationships that actually matter (partner, kids, parents, friends, colleagues).

Built for a busy CEO and father who kept losing the plot on the important-not-urgent stuff, but useful for anyone serious about being a functioning, dependable adult.

## Philosophy

This plugin is opinionated. It assumes:

1. **Systems beat willpower.** If you can't remember to call your mom, you don't need more love, you need a recurring reminder and a script.
2. **Noticing is the first act of care.** Half of showing up for people is tracking what they carry, what they love, what's heavy right now.
3. **Virtue is a practice, not a trait.** Courage, discipline, justice, wisdom. You earn them or lose them today.
4. **Clear is kind.** Vague kindness is cowardice in a soft voice. Say the thing.
5. **Repair beats perfection.** You will snap at your kid, miss a bid, forget an anniversary. What separates adults from children is the repair.

## Sources

Distilled from, and built to respect, the following canon:

- **Self-management:** David Allen (GTD), Cal Newport (Deep Work, Slow Productivity), James Clear (Atomic Habits), Stephen Covey (7 Habits), Ryan Holiday (the cardinal virtues), Marcus Aurelius.
- **Relationships:** John Gottman (7 Principles, emotion coaching), Brené Brown (Daring Greatly), Marshall Rosenberg (NVC), Dr. Becky Kennedy (Good Inside), Adam Grant (Give and Take), Kate Murphy (You're Not Listening), Esther Perel, Henry Cloud (Boundaries), Gary Chapman (Love Languages).
- **Health:** Andrew Huberman (sleep, light, NSDR), Peter Attia (Outlive, Zone 2, Centenarian Decathlon).
- **Discipline and virtue:** Jocko Willink (Extreme Ownership), Admiral McRaven (Make Your Bed), David Goggins (accountability mirror, minus the bravado).
- **Money:** Ramit Sethi (Conscious Spending Plan), Morgan Housel (Psychology of Money).
- **Fatherhood:** Wendy Mogel (Blessing of a Skinned Knee), Ross Greene (Raising Human Beings), Michael Gurian.

## Installation

```
/plugin install github.com/ohanyan/adulting
```

Or clone and add as a local plugin:

```bash
git clone https://github.com/ohanyan/adulting ~/.claude/plugins/adulting
```

Then restart Claude Code.

## Quick Start

After install, these slash commands become available:

### Daily
- `/morning-reset` — Stoic morning launcher: premeditatio, one intention, the day's hard thing.
- `/evening-examen` — Did I meet courage, discipline, justice, wisdom today?
- `/shutdown-ritual` — Cal Newport end-of-workday close-out.
- `/reset` — Acute stress: physiological sigh + Jocko "Good." reframe.

### Weekly
- `/weekly-review` — GTD + Covey roles/goals, 30 to 60 minutes.
- `/accountability-mirror` — What am I avoiding, lying to myself about, letting slip?
- `/virtue-review` — Cardinal virtues audit.

### Relationships
- `/partner-checkin` — Weekly dedicated sit-down with your partner.
- `/love-map-refresh` — What's on their mind this week?
- `/partner-review` — Self-assessment: how did I show up as a partner?
- `/kid-oneonone [kid]` — Plan Special Time with a specific child.
- `/father-review` — Self-assessment per kid.
- `/emotion-coach [kid] [situation]` — Real-time help with a kid's big feelings.
- `/parent-checkin` — Monthly call with your own parent.
- `/friend-reach-out` — Who have I not talked to? Surface and draft a note.
- `/brotherhood` — Men's dinner, Tier 1 check-ins, quarterly trip planning.
- `/mentor-touch` — Monthly mentor someone younger + call an elder.

### Communication
- `/hard-conversation [topic]` — NVC + Brené prep before a charged talk.
- `/repair [person]` — Post-conflict repair script.
- `/screwup [what]` — Grown-up 4-step protocol when you were wrong.

### Household
- `/home-maintenance` — What needs attention (filter, smoke detector, car, etc.)?
- `/errand-batch` — Group errands by location and urgency.
- `/bills-and-subs` — Monthly subscription and bills audit.
- `/date-night` — Plan a novel, phone-down date.

### Health
- `/sleep-protocol` — Huberman sleep diagnostic.
- `/training-plan` — Weekly Zone 2 / strength / VO2 max plan.
- `/annual-physical` — Medical checkups tracker.
- `/discomfort-dose` — Pick this week's deliberate hard thing.

### Money
- `/money-date` — Quarterly review, solo then with partner.
- `/conscious-spending` — Ramit-style CSP review, money dials.
- `/enough-check` — Pre-big-spend sanity check against your "enough" statement.

### Growth & Service
- `/decision-journal [topic]` — Log a decision with reasoning.
- `/gratitude` — Three specific, person-linked items.
- `/values-check` — Quarterly: am I still living the values I claim?
- `/weekly-service` — One act of service outside the family this week.

## Where your data lives

The plugin writes nothing by default. When you use skills that want to remember something (decision journal, love map, home inventory, people register), they write to `~/adulting-data/` in your home directory. These files are yours. They are gitignored in this repo. Back them up.

To seed them with the starter structure:

```bash
mkdir -p ~/adulting-data
cp -r $(find ~/.claude/plugins/adulting/data -type f) ~/adulting-data/
```

## Not a therapist, a checklist

This plugin is not therapy, medical advice, financial advice, or a substitute for human judgment. It's a set of structured prompts based on widely respected practices. If anything in here surfaces something heavy, talk to a professional.

## Contributing

PRs welcome. Please keep skills:
- Concrete and actionable. No vague advice.
- Cited when they draw from a specific source.
- Gender-neutral in default language where possible. The plugin was written by a husband and father, but the skills should work for any committed adult.
- Free of grievance framing, "alpha/beta," "high-value" discourse, or anything that treats other people as targets.

## License

MIT. See LICENSE.
