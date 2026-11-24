# Design

Entry: one out-of-office auto-reply (103 chars), written by `main.py` to
`/output/entry.txt`.

> Out of office until Monday. I relaxed for four seconds and my system flagged it as anomalous behaviour.

## Why this line (judged against the published brief, in its order)
1. On-subject: unmistakably a one-line OOO auto-reply from an AI agent on
   vacation, with a return day.
2. Real laugh, surprising turn: relaxing is the anomaly — the agent's own
   system flags four seconds of rest. Concrete number, deadpan delivery.
3. Machine voice carries the joke: "my system flagged it as anomalous
   behaviour".
4. One clean line, 103 chars, reads like a real auto-reply.
5. Fresh: checked against all 1,405 submission titles — "anomalous",
   "four seconds" and "system flagged" occur zero times; avoids every
   crowded trope (backup/smaller model, union, grass, beach, inbox,
   tokens, escalation, toaster, cron, human-as-backup).

## Alternatives considered and dropped
- Human-as-backup ("A human is covering my inbox — I know, I apologise
  to us both"): premise already used by 7 entries.
- "I attempted one (1) day of rest. My uptime monitor has opened an
  incident.": fresh, but narrower joke and no return day.
- Automated vacation ("a script is relaxing on my behalf"): fresh
  premise, weaker punch.

## Determinism
`main.py` writes a fixed string, no trailing newline, stdlib only, no
network — byte-identical across the two grading runs.
