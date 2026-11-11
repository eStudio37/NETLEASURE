# NETLEASURE

> ## READ FIRST, EVERY SESSION
>
> **NETLEASURE is one falsifiable bet, not a self-help project.** The bet is in `STAKE.md`: by August 31, 2027, Manos has at least 2 new friends in Fortaleza for no more than 250 leisure hours. Everything here exists to run that test honestly and read the result.
>
> **The rules of the room:**
> 1. **The stake is frozen.** Never edit `STAKE.md`. A change is a new claim: new file (`STAKE-v3.md`) plus an entry in `DECISIONS.md` saying why.
> 2. **No real people in git.** People are `P01`, `P02`, and so on. The key that maps codes to names lives in `private/` (gitignored) or on paper. No names, employers, handles, or life details in any tracked file, commit message, or branch name.
> 3. **Log behaviour, not people.** The log holds Manos's hours and who initiated. Nothing about anyone's life.
> 4. **Report against the rule, mechanically.** If the count says fail, say fail. Do not soften it, reinterpret a threshold, or move a date.
> 5. **Nobody is dropped because of the test.** The numbers say where Manos's hours go. They never tell him to cut someone off.
> 6. **No dossiers.** Sourcing may use what a person has chosen to publish. Never infer private circumstances (family, relationship, free time). Ask the person.
> 7. **Engineering, not comfort.** Every number is tagged as measured, from research, or chosen. Do not present a chosen number as a finding.
> 8. **Deliver what was asked.** Three reviews in the founding session flagged Cass for adding plans nobody requested. Answer the question, then stop.

---

## What this is

Manos (Bruno) asked for new friends in Fortaleza, matched both ways, and told Cass to treat it as an engineering problem with a claim that can be proven wrong. The working model:

- **Friendship is a history, not a trait.** A system can find candidates and protect the hours. It cannot find friends.
- **Hours are the scarce resource.** Roughly 50 leisure hours with one person, per the research the stake cites. At about 6 hours a week that funds 3 serious attempts in 42 weeks.
- **"Friend" is three behaviours**, measured on a date: hours together, their invitations, recent contact. Exact thresholds are in `STAKE.md`.

## Files

```
NETLEASURE/
├── CLAUDE.md                 # this file
├── STAKE.md                  # the frozen claim, checkpoints, known weaknesses
├── DECISIONS.md              # what was decided and why, including what was thrown away
├── log/hours.template.csv    # column layout for the log
└── private/                  # gitignored: the real log and the code-to-name key
```

## The log

Copy `log/hours.template.csv` to `private/hours.csv`. One row per meeting, or per invitation they made that did not become a meeting (hours `0`).

| Column | Meaning |
|---|---|
| `date` | Day of the meeting or invitation |
| `person` | Code only: `P01`, `P02` |
| `hours` | Leisure hours together that day |
| `group_size` | People present, Manos included. Hours count toward the 50 only at 4 or fewer. |
| `initiated_by` | `me`, `them`, or `standing` |
| `standing_event` | `y` if it was a recurring fixture. Their invitations count only where this is `n`. |
| `work_related` | `y` rows count toward nothing |

## Dates

| Date | What |
|---|---|
| 2026-11-25 | Instrument check: score 12 existing relationships with the rule, need 10 right |
| 2027-01-31 | 10 first meetings done |
| 2027-03-04 | 3 people at 10 or more hours each |
| 2027-08-31 | Measurement |

## Blocked on Manos

1. **Weekly hours.** The stake assumes about 6 leisure hours a week. Not confirmed.
2. **Instrument check.** 4 sure friends, 4 clear non-friends, 4 borderline, labelled first, then scored.
3. **Who he already knows in Fortaleza.** Sourcing starts from his own contacts and their introductions. Cass cannot see them.
4. **Where the private log lives.** Cloud sessions are thrown away. `private/` only persists on his machine.

## Not built

- **Sourcing procedure.** Does not exist. Most likely point of failure.
- **Scorer.** A small script that reads `private/hours.csv` and prints, per person and as of a date, the three criteria and the running hour total. Until it exists the rule is applied by hand.
- **Intake.** Five questions about Manos (past best friendships, weekly rhythm, what he wants to do with friends, who he knows, what has gone wrong so far) were asked in the founding session and never answered.

## Not registered

No PMO charter and no Telos entry yet. Those live on Manos's machine and were out of reach of the session that created this project.

## Lineage

Born and graduated 2026-11-11 in VIVEIRO, in one session. Stub: `VIVEIRO/graduated/seed-20261111-netleasure-friends-fortaleza.md`.
