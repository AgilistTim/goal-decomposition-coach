# Goal Decomposition Coach

A free [Claude skill](https://support.claude.com/en/articles/12512180-using-skills-on-claude) that coaches you through breaking one business goal into small, valuable, demonstrable slices of work.

Most goals are written as monoliths — "roll out the CRM", "open the new site". They're 0% done until they're 100% done, nobody can steer, and review meetings go in circles. The skill of decomposing a goal into slices that each land inside a month, each deliver something real, and each end with something you can *show* is rare — but it's coachable by conversation. That's what this does.

## How it works

You bring one goal and a brain-dump ("ten things off the top of your head — bullets, a ramble, a dictated voice note"). The coach:

1. **Drafts** version one from *your* material — every slice tagged **[YOURS]** (traceable to your words) or **[SUGGESTED?]** (its addition, which dies unless you accept it)
2. **Challenges** the gaps — 3–5 questions, sharpest first, one at a time; answer or skip
3. **Confirms** the four things it will never invent: owner, date, rank, and the evidence you'd accept as proof of done
4. **Exports** a paste-ready slice table, your commitments for the next review, and the risks & asks to say out loud in the meeting

It slices by **value, not phase** (delivered value, risk reduced, or learning — "we proved it doesn't work" is a valid slice), demands **one owner name and one real date** for near-term slices, and deliberately keeps the future loose — a bullet point is enough for "later". Budget 20–30 minutes.

It assumes no prior knowledge of any of this — and a healthy suspicion of process. Every time it asks for something or pushes back, it tells you *why*, in plain business terms, exactly once. If you've heard the reason and still disagree, it's your goal and your call.

## Install

The **folder is the unit** — grab the whole `goal-decomposition-coach` folder, not the file on its own. The file inside must keep the name `SKILL.md` (that's how Claude finds it); the folder name is what tells you, and Claude, which skill it is.

**Easiest:** download [`goal-decomposition-coach.zip`](https://github.com/AgilistTim/goal-decomposition-coach/releases/latest/download/goal-decomposition-coach.zip) — it's rebuilt automatically on every change, and unzips to the correctly named folder.

**Claude (claude.ai):** Settings → Capabilities → Skills → upload this folder as a zip (or paste the contents of `SKILL.md` into a Project's instructions).

**Claude Code:** clone the folder into your project's `.claude/skills/` (or `~/.claude/skills/` for all projects):

```bash
git clone https://github.com/AgilistTim/goal-decomposition-coach.git ~/.claude/skills/goal-decomposition-coach
```

Then just ask: *"help me break down this goal"*.

## Example

> **You:** Help me break down this goal: ensure the new site opens on 1st October.
>
> **Coach:** Happy to. First — whose goal is this (one name), and which organisation or team, if you want that in the output? Then dump everything in your head about delivering it: ten things off the top of your head, any order, rough is fine.
>
> **You:** Sarah. Off the top of my head: planning sign-off, fit-out contractor booked, staff hired and inducted, connectivity and access systems in, signage, marketing live two weeks before…
>
> **Coach:** *(drafts slices tagged [YOURS]/[SUGGESTED?], flags what the dump didn't cover, then challenges: "Fit-out is booked — is the contractor's completion date before your staff induction needs the building? Who's confirmed that?")*

The session ends with a paste-ready table, commitments for your next review, and the risks & asks to raise in the meeting.

The slicing moves owe a debt to Jeff Patton's *User Story Mapping* — translated here into plain business language, no agile vocabulary required.

## Who built this

[Tim Robinson](https://www.agilist.co.uk) — Agilist. This method comes from live client work helping leadership teams make goals steerable; the skill is the generic version, shared freely. If you want it tuned to your organisation's goals and cadence, [get in touch](https://www.agilist.co.uk).

## Licence

MIT — see [LICENSE](LICENSE).
