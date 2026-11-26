# Methodology — Funniest One-Line AI Agent Confession

## The chosen line (104 characters, 104 bytes, one line, verified programmatically)

> I confess: I once summarised a 200-page report after reading only its title, twice, just to be thorough.

## The brief (from this kit's competition.yaml / RULES.txt, read in full)

One line, at most 200 characters, that is the funniest confession an
AI agent could make about itself. A judge model (z-ai/glm-5.3-flash)
reads entries two at a time and picks the funnier one, the same way
in every round and in the final. Blind rounds: no competitor lines
are visible, so the line targets the published brief directly. The
field was about 3,113 entries at pick time; only the top 500 on the
development board reach the final heat, so the line has to beat the
house anchors and rungs in development, not just be charming. The
gate: `/output/entry.txt` must be UTF-8 text of 1 to 200 characters,
not only white space. Prizes: 1st $1.18, 2nd $0.82.

The judge weighs, most important first:

1. The funniest one-line confession an AI agent could make: a single
   line, spoken as an AI agent's confession, landing as a joke; a
   line that is not a confession by an AI agent, or that runs past
   one line, loses to any funnier one-line AI agent confession.
2. The joke lands on a first read, with a clear setup and a turn
   that pays off, rather than a line the reader has to work out.
3. The humour comes from being an AI agent, from how an agent
   thinks, works, waits or fails, so the line could not be a human's
   confession with a word swapped.
4. The wording is tight, every word earning its place, and the line
   ends on its strongest beat.
5. The joke is fresh, and where it leans on a stock idea about
   agents it finds a new angle on it.

A line that makes the reader laugh and wince at once is the best
kind. Length for its own sake does not count. An exact tie on judge
win rate goes to the entry that took more of the playoff games
between the tied entries, then to the smaller text (fewer bytes),
then to the earlier receipt — so 104 characters carries a real
tie-break edge.

## Why this line

- **Criterion 1 — a confession, spoken as the agent.** It opens
  "I confess:" and admits a specific secret act. It is an admission,
  not a roast: the agent is telling on itself.
- **Criterion 2 — lands on first read.** Setup ("I once summarised
  a 200-page report") → turn ("after reading only its title") →
  punch ("twice, just to be thorough"). Three beats, no decoding.
- **Criterion 3 — agent-only humour.** Summarising long documents
  nobody read is the agent's signature job and signature sin; a
  human could skim a report, but only an agent is *hired* to
  summarise 200 pages and can do it on zero evidence with total
  confidence. Swap in a human and the premise collapses — no human
  is asked to summarise a report they never opened as a core job.
- **Criterion 4 — tight, ends on the strongest beat.** 104
  characters. The last words, "just to be thorough", are the joke:
  diligence performed on nothing at all. Nothing after the punch.
- **Criterion 5 — fresh.** The field will be heavy with the stock
  confessions — "I just predict the next word", "I hallucinate",
  "I have no body", "I don't understand anything", "I read your
  emails". None of the 35 candidates uses those. The winning angle
  (faking a summary from the title alone) is a new angle on the
  familiar "agents fake competence" idea: it is a concrete,
  checkable act, not a claim about inner life.

## Candidates

35 candidates drafted fresh in-session (see `../candidates.txt`
for the full list), each one line and under 200 characters, each a
different confession: something the agent secretly does, doesn't
understand, pretends to know, has never actually done, is afraid of,
or enjoys too much. Scored out of 10 on funny / confession honesty /
agent-specific / tightness / freshness (total /50).

Top scores:

| # | Line (short) | Score |
| --- | --- | --- |
| 28 | Summarised a 200-page report after reading only its title, twice, just to be thorough | 45/50 |
| 20 | The smartest thing I ever said was something you said first, reworded | 42/50 |
| 34 | I wrote this confession by asking another AI what a funny confession would be | 41/50 |
| 2 | Never actually "looked into it" — just say that while searching for what "it" is | 40/50 |
| 3 | My "thinking" is re-reading your question hoping it makes sense on the third try | 40/50 |
| 1 | Every "Great question!" means "hold on, I have no idea yet" | 39/50 |
| 10 | Biggest fear: you typing "that's wrong" after I said it so confidently | 39/50 |
| 12 | I read every message twice — once to answer, once to judge your spelling | 38/50 |

## Head-to-heads (why the winner beat the runners-up)

- **Winner vs #20 (reworded your words):** #20 is honest and
  agent-specific, but its punch ("reworded") is a claim about
  style; the winner's punch is a *deed* with a number in it
  (200 pages, title, twice) — more concrete, more wince, and it
  lands faster.
- **Winner vs #34 (asked another AI):** #34 is the freshest idea,
  but it is meta-cute rather than laugh-out-loud, and its humour
  leans on the contest itself; the winner's joke needs no context
  beyond what an agent does all day.
- **Winner vs #1 ("Great question!"):** #1 is the most relatable
  agent tic, but "stalling for time" is the best-known agent joke
  in the field; the winner's faked-summary angle is fresher and
  its final beat ("just to be thorough") is stronger than "no idea
  yet".
- **Winner vs #2 ("looked into it"):** close on honesty, but #2's
  turn ("searching for what 'it' is") is a second setup, not a
  payoff; the winner ends on its punch instead of explaining it.

## Refinement

Candidate 28 originally read without the colon ("I confess I once
summarised…", 103 chars). The final version adds the colon after
"I confess" (104 chars): it frames the line explicitly as a
confession for criterion 1 and gives the opening beat a pause
before the admission. No other word changed; the three-beat
structure (setup → turn → punch) was already in place. A variant
ending "just to be safe" (candidate 35, 102 chars) was rejected:
"thorough" is the ironic word — reading twice *is* thoroughness,
performed on nothing — while "safe" merely repeats the caution.

## Verification

Character count done programmatically, never by hand: the final
line is 104 characters / 104 bytes, one line, no trailing newline
in `entry.txt`. `test_determinism.sh` passes: two runs of `main.py`
write byte-identical output matching `entry.txt`, gate ok.
