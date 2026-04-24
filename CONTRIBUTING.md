# Contributing

Thanks for considering a contribution. This plugin is opinionated, so not every PR is a fit. Read this first.

## What I'll gladly merge

- **New skills** that fill a real gap and follow the style below.
- **Fixes** to typos, broken paths, wrong citations, or skills that don't work as written.
- **Better examples** in existing skills, especially ones that make a skill more concrete or less preachy.
- **Platform fixes** (Windows paths, Linux, shell differences).
- **Source corrections.** If I've attributed something to the wrong author or summarized a practice incorrectly, tell me.

## What I probably won't merge

- Skills or framings built around grievance, alpha/beta hierarchies, "high-value" discourse, dominance, or treating other people (of any gender) as targets or status objects. See the README for why.
- Skills that require specific paid services, brands, or apps. Skills should work with plain markdown files in `~/adulting-data/`, no SaaS dependency.
- Skills that are essentially lectures. If your skill doesn't produce a concrete action, checklist, or prompt, it's not a skill here.
- Generic "life advice" skills that aren't grounded in a documented practice from a real source.
- Skills with heavy personalization for one user. Keep it portable.

## Style guide for skills

### Frontmatter

```yaml
---
name: skill-name
description: One sentence on what it does and when to use it. Claude reads this to decide when to auto-invoke. Keep it under 200 chars.
---
```

Optional: `argument-hint`, `allowed-tools`. See the Claude Code plugin docs.

### Body structure

- **Open with why.** 2-3 sentences on what this is and why it works. Cite the source.
- **Numbered steps** so a user can follow along without re-reading.
- **Concrete over abstract.** "Write the one sentence you're afraid to say" beats "be vulnerable."
- **End with a log format.** Most skills append to a file in `~/adulting-data/`. Provide the exact template.
- **Pushback clauses.** If the user will try to cheat the skill, name the pattern and push back.

### Tone

- Direct, not preachy.
- No jokes at anyone's expense.
- Masculine virtue framings (discipline, service, courage) are fine. Masculine grievance framings are not.
- Use "partner" as the default for spouse/boyfriend/girlfriend. It's inclusive and still fits married people.
- Use "they" as default singular pronoun when gender is not relevant.

### Length

Most skills are 150-300 lines. If yours is under 100, it may be too thin. If over 400, split or tighten.

## Testing a new skill

Before submitting:

1. Run the skill on yourself for at least a week.
2. Check whether the log file the skill writes is actually useful over time.
3. Check whether the pushback clauses catch the real ways you'd cheat.
4. Ask yourself: does this skill produce a different behavior in me, or just a different feeling?

The test of a skill is whether it changes behavior. Feeling seen for 10 minutes is nice, but it is not the point.

## PR process

1. Fork.
2. Branch off `main`.
3. Add or edit one skill per PR. Multi-skill PRs are harder to review and revert.
4. In the PR description, include:
   - The source the skill draws from.
   - A link to a week of your own logs (redacted is fine) if it's a new skill.
   - Any known edge cases.

## Citing sources

Every skill should name its sources in the body. Not as academic references, as working attribution. "Gottman's research shows" or "From Ramit Sethi's Conscious Spending Plan" is plenty.

If you're drawing from a specific book, name the book once. If you're drawing from a practice that's broader (Stoic evening review, NVC), name the tradition.

## Code of conduct

Be decent. The plugin is about showing up for other people. That applies to interactions on this repo too.

## License

MIT. Contributions are made under the same license.
