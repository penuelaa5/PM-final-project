# PRD & Prototype Sprint (Module 4)

## Pick & scope with MoSCoW
- **The “Now” feature I’m scoping (name + one-line core description):** A1 Spotlight Curated Rail — the core intervention. A default hand-picked rail that replaces the zero-payoff scroll with zero effort from the user.
- **My finalized Must-Haves (after overriding the AI):** can a Wanderer find a title, play it, stay 20 minutes. That test deletes anything that isn’t about one user’s screen. I overrode it with three gates, a Must breaks function, measurement, or the guardrail:

Rail renders default-on, zero input.
Human-picked titles (spreadsheet is fine for sprint one).
Tap → plays.
Playback survives to 20 min (no buffering drop, resume holds). Dependency I don’t own but the metric dies without it.
Instrumentation: impression → play → 20-min watch, logged. Without it, no result.
Cohort targeting + holdout. My control group and my Power User guardrail in one.
- **What I demoted from Must → Should/Won’t, and why:** Rule: if the pilot still functions, measures, and stays safe without it, it’s not a Must.

Should: “Why You’ll Love This” label, thumbnail fallback, curator ordering. Help the rail, don’t make it work.
Could: Hidden Gem Badge, curator CMS. Polish and tooling that can wait.
Won’t: Personalized queue (A5, that’s the 6-month build, not sprint one), mood entry (A4, re-adds the effort we’re removing), curator following, filters, offline, watch party. Wrong persona or wrong problem.

## Generate your Simplified PRD
- **One thing my PRD makes explicit that a vague brief would have missed:** My PRD makes explicit that the 20-minute watch metric depends on a playback-reliability fix the rail doesn’t own (FR4: no buffering drop, resume holds across devices), so a buffering bug can’t masquerade as a curation failure, which a “just build a curated rail” brief would have missed entirely.

## Prompt-to-prototype sprint
- **Where did the prototype reveal a gap in my PRD logic? (what I had to update):** The prototype showed three outcomes, reached 20 minutes, player failure, and left early, which exposed that my FR5 instrumentation only logged a pass/fail funnel with no exit reason, so a buffering bug and a bored viewer both counted as “didn’t reach 20 minutes” and confounded the metric. I updated FR5 to log a session exit reason (completed-20 / user-exit / player-failure) so the 20-minute rate measures curation, not playback.
- **My prototype, as a link or a screenshot (publish or share from your tool; in Lovable that is Share → Share Preview, in Bolt Publish → Web. No share URL? Screenshot the working flow):** https://twenty-minute-watch-quest.lovable.app
