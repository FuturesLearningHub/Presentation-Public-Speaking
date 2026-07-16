# Presentation & Public Speaking — Building and Delivering to a Room or Leadership Audience

An interactive, single-page teaching site for presenting to teams,
stakeholders, and executive audiences. A **Learning on Demand** program:
the facilitator projects it while learners scan a QR code and work every
exercise on their own devices, or share the link for self-paced review.
Practice-heavy by design: everyone drafts for a real upcoming
presentation, and everyone speaks out loud at least once.

Part of the Vanderbilt Learning Series. Catalog:
[Course Library](https://me5231979.github.io/Course_Library/) ·
Sister programs: [Navigating Difficult Conversations](https://me5231979.github.io/Difficult_Conversations/),
[Emotional Intelligence](https://me5231979.github.io/Emotional-Intelligence/)

- **Learner edition:** https://me5231979.github.io/Presentation-Public-Speaking/
- **Facilitator edition:** https://me5231979.github.io/Presentation-Public-Speaking/facilitator/

**Skills:** Continuously strives for excellence (VU competency) ·
Public Speaking · Storytelling · Strategic Communication · Stakeholder
Communications

## Running it

Plain HTML/CSS/JS, no build step:

```bash
python3 -m http.server 8000
```

## What it teaches (7 sections)

1. The myth & the case — public speaking is 59th of 85 fears (Chapman);
   what decides careers is gravitas + communication (Coqual, Deloitte)
2. Executive presence — Hewlett's three pillars (gravitas 67%,
   communication 28%, appearance 5%) and your growth edge
3. The Big Idea — Duarte's one-sentence discipline: point of view + stakes
4. The Sparkline — What Is ↔ What Could Be → New Bliss, the shape of the
   world's great talks
5. SCQA — Minto's Pyramid Principle for the executive room: lead with the
   answer
6. Delivery — Anderson's five keys, Gallo's five tips, AMA's seven
   principles, and a live timed speaking round
7. The tough question — the AMA bridge: acknowledge → answer → return to
   the Big Idea

Ends with a scored recap, the **Presentation Rebuild capstone** (real
talk, Big Idea, structure, literal opening line, one thing cut, date), a
flip-card glossary, and a spoken-commitment close. `worksheet.html`
mirrors the capstone on paper; `cheatsheet.html` is the take-home.

## The interactive tools

| Slide | Tool | What learners do |
|---|---|---|
| The case | **Guess the number** | Call four research findings (Chapman, Coqual, Deloitte) before the reveal |
| Presence | **Spot the pillar** | Read five presentation scenes; name the pillar at work or at fault |
| Big Idea | **Topic or Big Idea?** + **private drafter** | Judge five openers, then assemble their own Big Idea (point of view + stakes) |
| Sparkline | **Tag the beat** | Tag five talk beats as What Is / What Could Be / New Bliss |
| SCQA | **The Exec Briefing Lab** | Build a graded 4-part SCQA briefing and watch the executive room react |
| Delivery | **Fix the delivery** | Pick the research-backed fix for five delivery failures |
| Q&A | **Judge the bridge** | Pick the composed bridge response to five pointed executive questions |
| Recap | **Scored quiz** | 6 questions mapped to the objectives |
| Capstone | **Presentation Rebuild** | Build and copy a rebuild card with the literal opening line written |

## Instructional design

- **Bloom's ladder:** objectives run Explain/Identify → Distill (Apply)
  → Structure (Apply/Analyze) → Practice/Evaluate → Rebuild-and-commit
  (Create).
- **Kirkpatrick:** L1 fist-to-five at close; L2 inline checks + trainer
  scores + recap; L3 rebuild card + 7-day pulse + 30/60/90 structure
  check (are decks shifting from bullet-heavy to story-led?).
- **Adult learning:** learners bring one real upcoming presentation
  (pre-work), every exercise drafts against it, everyone takes a live
  timed speaking rep with peer feedback, and the capstone ships as a
  rebuilt talk with a rehearsal on the calendar.

## The facilitator edition

Generated at `/facilitator/` by `python3 tools/build-facilitator.py` from
`facilitator/notes.json` — ATD-scripted rails (Say / Do / Ask with expected
answers / Debrief / Transition), a briefing slide (prep, materials,
contingencies, tough questions, three copy-paste templates), Full 90 /
Core 60 timing. Its QR encodes the learner URL.

## Editing map

- Copy: `index.html` · Recap: `QUESTIONS` in `assets/js/main.js`
- Trainers: `makeTrainer` configs (stats, pillars, topics, beats,
  delivery, bridges)
- Big Idea drafter: `bigIdea` block · SCQA lab: `SLOTS` in main.js
- Capstone maps: `STRUCTURE` / `CUT` / `WHEN` in main.js
- Runbook: `facilitator/notes.json` (timing must sum: Full 90 / Core 60)
- Citations to keep honest: Chapman Survey of American Fears (2024:
  59/85 at 29%), Coqual/Hewlett Executive Presence (gravitas 67%,
  communication 28%, appearance 5%; EP ≈ 26% of promotion), Deloitte CFO
  Signals 2Q 2024 (39% communication), Duarte (Big Idea™, Sparkline™,
  TEDxEast 1nYFpuc2Umk), Minto Pyramid Principle/SCQA/MECE, Anderson HBR
  + TED (-FOCpMAww28), Gallo HBR, AMA Seven Principles + Effective
  Executive Speaking, SHRM six questions.
- Publish: `git push origin main && git branch -f gh-pages main && git push -f origin gh-pages`
