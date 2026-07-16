# Presentation & Public Speaking — Vanderbilt Learning Series

Single-page interactive classroom experience (Learning on Demand). Live at
https://me5231979.github.io/Presentation-Public-Speaking/ (GitHub Pages,
`gh-pages` branch — publish with
`git branch -f gh-pages main && git push -f origin gh-pages`).

Sister programs: AI_Classroom, AI-Advanced, Difficult_Conversations,
Coaching-for-Performance, Emotional-Intelligence; catalog at
me5231979/Course_Library. Same engine, same standing principles.

## Standing design principles (do not regress these)

1. **Simulators, practice, and play throughout.** Every teaching section
   has an interaction; the SCQA Exec Briefing Lab and the live delivery
   round are the signature pieces, Guess the Number is the myth-buster.
2. **This is a practice-heavy speaking course.** Everyone speaks out loud
   at least once (live round, 60–90s, strictly timed, ONE note each).
   Never cut the live round from any path — a presentation course where
   nobody presented is a contradiction.
3. **A reason and facilitation behind every activity.** Learner-visible
   "Why this matters" lines; activities labeled As a group / On your own
   with steps, timings, and solo variants.
4. **Every section facilitatable, learning validatable.** ATD runbook in
   `facilitator/notes.json`. Kirkpatrick: L1 fist-to-five, L2 recap, L3
   rebuild card + 7-day pulse + 30/60/90 structure check.
5. **Facilitator edition is generated, never hand-edited** — run
   `python3 tools/build-facilitator.py` after ANY change to index.html or
   notes.json. Its QR encodes the LEARNER url.
6. **Skills tagging.** Hero carries the skills row (pills): core VU
   competency "Continuously strives for excellence" + Public Speaking,
   Storytelling, Strategic Communication, Stakeholder Communications.
   Keep in sync with the Course Library card and syllabus.
7. **Trademark hygiene.** Big Idea™, Presentation Sparkline™, and
   Persuasive Presentation Form™ are Duarte, Inc. marks — keep the ™ on
   first use per page and credit Duarte, Minto, Anderson, Gallo, AMA,
   Hewlett/Coqual by name. Keep stats verifiable (see README citations).
8. **Brand: Vanderbilt FLH system.** Black #1C1C1C / white / flat gold
   #CFAE70; Libre Caslon Display headlines (one italic word), Inter body,
   Antonio eyebrows; motion ≤400ms; real VU lockups (authorized use only).
9. **No frameworks.** One CSS file, one JS file, vendored QR lib,
   self-hosted fonts; hero montage streams from Higgsfield CDN with the
   particle canvas fallback.

## Layout (15 slides)

Welcome/QR (everyone-speaks contract) → Hero (6 objectives + skills row +
montage) → Agenda → 01 The myth & the case (Guess the Number) →
manifesto ("You can coach out a weak delivery. You can't coach in a weak
idea.") → 02 Executive presence (pillar trainer) → 03 The Big Idea
(topic-judge + private drafter + Duarte video) → 04 The Sparkline (beat
tagger) → 05 SCQA (graded Exec Briefing Lab) → 06 Delivery (fix-it
trainer + Anderson video + live round rules) → 07 The tough question
(bridge judge + SHRM six questions) → Recap quiz → Capstone Presentation
Rebuild → Glossary → Closing (spoken opening line).

## Editing map

- Copy: `index.html` · Recap: `QUESTIONS` in `assets/js/main.js`
- Trainers: `makeTrainer` configs (statGuess, pillarSpot, topicJudge,
  beatTag, deliveryFix, bridgeJudge)
- Big Idea drafter: `bigIdea` block · SCQA lab: `SLOTS` + reaction tiers
- Capstone maps: `STRUCTURE` / `CUT` / `WHEN` in main.js
- Runbook: `facilitator/notes.json` (timing must sum: Full 90 / Core 60)
- Videos: Duarte TEDxEast (1nYFpuc2Umk), Anderson TED (-FOCpMAww28)
