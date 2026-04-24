# Data Templates

These are templates for the files the plugin's skills will read and write.

## How to use

1. Create your personal data directory (outside this repo):

   ```bash
   mkdir -p ~/adulting-data/people
   mkdir -p ~/adulting-data/decisions
   mkdir -p ~/adulting-data/journal
   ```

2. Copy the templates you want to start with:

   ```bash
   cp home-inventory.template.md ~/adulting-data/home-inventory.md
   cp medical.template.md ~/adulting-data/medical.md
   cp values.template.md ~/adulting-data/values.md
   cp subscriptions.template.md ~/adulting-data/subscriptions.md
   cp friendship-tiers.template.md ~/adulting-data/friendship-tiers.md
   ```

3. For each close person you want to track, copy `people.template.md` to `~/adulting-data/people/<name>.md`.

4. Back up `~/adulting-data/` somewhere private. iCloud, Dropbox, git repo with private remote, whatever. It will accumulate value over time.

## What goes where

| File | Written by | Purpose |
|------|------------|---------|
| `home-inventory.md` | You + `/home-maintenance` | House, car, vendor rolodex |
| `medical.md` | You + `/annual-physical` | Providers, labs, conditions, meds |
| `values.md` | You + `/values-check` | 5-7 core values, alignment scores |
| `subscriptions.md` | You + `/bills-and-subs` | Recurring charges, money dials |
| `friendship-tiers.md` | You + `/friend-reach-out` | Tier 1/2/3, cadences |
| `people/<name>.md` | You + multiple skills | Per-person love map, log |
| `decisions/<date>-<name>.md` | `/decision-journal` | One file per logged decision |
| `journal/*.md` | Most skills | Daily, weekly, repair logs |

## Privacy

None of this is pushed to GitHub. `.gitignore` excludes `data/*.md` that are not templates. Your personal data lives in `~/adulting-data/` only. Back it up yourself.
