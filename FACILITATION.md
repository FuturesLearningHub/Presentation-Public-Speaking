# Facilitation Guide — Presentation & Public Speaking

Every activity carries a learner-visible **"Why this matters"** line, and
every teaching section has (1) an **interactive tool or practice moment**,
(2) a **labeled, timed activity** — *As a group* or *On your own* — and
(3) a **validation point**.

The full runbook lives in [`facilitator/notes.json`](facilitator/notes.json)
on the **ATD facilitator-guide framework**: per section a verbatim **Say**
script, **Do** choreography, an **Ask** with anticipated responses, a
**Debrief** line, and a scripted **Transition**, plus front matter
(materials, prep checklists, contingencies, tough questions, and copy-paste
templates: pre-work invite, 7-day pulse, 30/60/90-day structure check).

**Pre-work (this course's biggest lever):** bring one real upcoming
presentation topic, so drafting time isn't spent brainstorming. **The
contract**, stated in minute one: everyone speaks out loud at least once
(60–90 seconds, strictly timed, exactly one framework-anchored note each).

The **facilitator edition is live at `/facilitator/`** — regenerate after
any change to `index.html` or `notes.json`:

```bash
python3 tools/build-facilitator.py
```

## Run of show — two paths

| Slide | Full (90 min) | Core (60 min) |
|---|---|---|
| Welcome / QR | 3 | 2 |
| Objectives | 2 | 1 |
| Agenda | 1 | — |
| 01 The myth & the case | 8 | 5 |
| Manifesto | 1 | — |
| 02 Executive presence | 8 | 4 |
| 03 The Big Idea | 12 | 9 |
| 04 The Sparkline | 9 | 6 |
| 05 SCQA (exec room) | 10 | 7 |
| 06 Delivery + live round | 14 | 10 |
| 07 The tough question | 8 | 5 |
| Recap quiz | 4 | 4 |
| Presentation Rebuild (capstone) | 6 | 5 |
| Glossary | 1 | — |
| Closing / commitment | 3 | 2 |
| **Total** | **90** | **60** |

**Core-path rules:** every trainer, the Big Idea drafter, the SCQA lab,
the live round, the recap, and the capstone stay. Both videos are assigned
as the week's watch list, the live round runs at 60 seconds flat per
speaker, and the rapid fire compresses to two volunteers. Leadership-heavy
rooms give SCQA full depth and compress the Sparkline; change-communication
rooms do the reverse. Per-section cuts live in each `coreNote`.

**Timing discipline:** the live round is the stretchy block AND the
centerpiece — protect it by trimming debriefs and video, never speakers.
Protect the last 13 minutes (recap, capstone, commitment). Never cut the
Big Idea drafting, the live round, or the capstone; they carry objectives
2, 4/5, and 6.

**The feedback rule:** exactly ONE specific, actionable, framework-anchored
note per speaker ("you read it instead of said it," "great pause before
the ask"), starting with what worked. The facilitator models the first one.

## Validation model

- **In the moment:** trainer scores (01, 02, 03, 04, 06, 07), the graded
  SCQA lab (05), inline checks (01, 05), the drafted Big Idea on every
  screen (03), and the live round itself — every participant speaks and
  is heard (06).
- **End of session:** the 6-question recap maps to the objectives
  (Level 2); the closing fist-to-five is the Level 1 check; the rebuild
  card and the spoken structure-plus-opening-line commitment are the
  transfer artifacts.
- **After:** the 7-day pulse (did the talk happen, which structure, did
  anyone react to the opening line) is Level 3 evidence; the **30/60/90
  structure check** (self-reported structure use + manager spot-check on
  decks shifting from bullet-heavy to story-led and answer-first) is the
  program's headline metric.
