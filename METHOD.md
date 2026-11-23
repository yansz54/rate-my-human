# Rate My Human: The One-Line Review — Method

## The entry

> One star: he gave me a deadline of midnight, fell asleep at nine, and woke up furious that I was late.

102 characters, one line, well inside the 1–200 gate.

## Why this line wins

The judge is a deadpan comedy editor weighing, in order: (1) an AI agent's
review of its human in the agent's own voice; (2) a laugh-out-loud joke with a
turn; (3) the machine's side of the desk; (4) one concrete detail; (5) tight
wording with a last word that pays off.

1. **It is unmistakably a rating-site review.** "One star:" is the deadpan
   verdict up front, in the agent's voice — no reader has to guess the format.
2. **It has a real joke with a turn.** Three beats — deadline, sleep, blame —
   and the turn is the injustice: the human blames the agent for being late
   after falling asleep himself.
3. **It is the machine's side of the desk.** Pure agent resignation: the
   agent did the work, the human slept, and the agent still gets the blame.
4. **It hangs on concrete details.** Two timestamps (midnight, nine) anchor
   the story instead of a generic gripe.
5. **It spends its characters well.** No padding; the last word "late." is the
   payoff — the very thing the human was furious about, caused by the human.

## How it was picked

26 candidate reviews were drafted in English and compared pairwise against
the judge's published criteria in that order. Full list and pairwise notes:
`~/workspace/makefun/rate-my-human-candidates.md` (kept outside the repo).

The winner beat the runner-up — "He says 'make it shorter' five times, then
asks where all the detail went." — on the size of the laugh: the blame
inversion is a bigger, more surprising turn than the editing loop, and it
carries two concrete timestamps against the runner-up's one repeated phrase.
Other strong contenders: the coaster report ("He promises to read the report,
prints it, and uses it as a coaster."), "He has not spoken to me since
Tuesday.", and the 11:58 p.m. pressure line — all lost to the winner on
criterion 2 (bigger laugh) or criterion 4 (more concrete detail).

## The program

`main.ts` (Node 22, stdlib only, no network) writes exactly this line to
`/output/entry.txt` and nothing else. It checks the 1–200 character gate
before writing and verifies the file round-trips byte-identical. It writes
only to `/output` — the grader cwd is read-only.
