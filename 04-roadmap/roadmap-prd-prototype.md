# Roadmap, PRD & Prototype (Module 4)

## Your strategic anchors
- **Persona (M2), who are you solving for?:** The wonderer
- **Primary success metric (M3), your leading indicator:** 20+ minutes watch
- **Moment of misery (M2), the specific friction blocking the goal:** the moment it feels most broken
The instant she closes a 15,000-title app with nothing to watch and reaches for a disc. Maximum choice, zero payoff, and the product she pays for just lost to a shelf.
- **Guardrail metric (M3), what must not drop or break:** Power User retention and session length must not drop. Power Users are 22% of the base, the highest LTV ($14.20), already low-churn, and already 58% curated. If reorienting Spotlight toward Wanderers dilutes the curation quality that retains Power Users, you win the cheap segment and bleed the valuable one. Protect their session length and curated-content satisfaction above all. Secondary guardrail: overall app session-completion rate, so a Wanderer-driven redesign doesn’t worsen the mid-session drop-off seen in Snapshot 1.

## Scan the backlog & set a human baseline
- **My instinctive “quick wins” before touching the AI (2 to 3 feature IDs + why):** _(not filled in)_

## Audit, override & decide
- **Where did you override the AI? (feature + old vs. new score + why):** The AI docked A4 because its core move (pick a mood before anything loads) asks the passive Wanderer to do work at the exact point they refuse to. That reasoning is sound for the pure persona. I overrode it because a single tap on login isn’t the same class of effort as a search or a scroll, and because mood-entry serves the adjacent “quiet Sunday” browser even if the hardest-core Wanderer skips it. My guardrail on the override: in the pilot, A4 is an optional enhancement layered on the default rail (A1), not a gate. If the Wanderer ignores the mood picker, the curated rail still loads. That way the feature can only add value, never reintroduce the friction the AI was worried about. If it were a mandatory step, I’d have left the AI’s score alone.
- **Did the AI over-value a Sales/Eng request your M2 interviews don’t support?:** No, the opposite. It did exactly what ruthless scoring should: it gutted every non-research feature.

A8 Watch Party (Sales): Value 1, Time Sinker. No interview mentions social viewing, and the Wanderer is a solo passive viewer. Correctly killed.
A10 Offline Download (Sales): Value 2, Time Sinker. Serves someone who already chose a title. Not a discovery fix, no M2 support. Correct.
A9 Advanced Filter Engine (Engineering): Value 1, Time Sinker. This is the sharp one. More filters is what an engineer thinks discovery means, but it adds effort at the point of choice, which deepens the moment of misery for this persona. The AI scored it against the user, not the sponsor. Correct.

So the AI didn’t over-value any of them. If anything it was appropriately cruel, every Sales/Eng-origin feature landed in the kill zone, and the M2 interviews back that placement (no one asked for parties, downloads, or more filters; they asked for a human to hand them something good).
- **Did it underweight something your M3 cohort/funnel data strongly supports?:** Yes. A6, the Spotlight Digest Email. The AI scored it Value 4 but filed it as a Fill-In, and I’d argue the M3 data supports a higher weight than its placement implies.

The cohort and segment data shows the Wanderer logs in 1.1 sessions a week. Every homepage feature, A1 through A4, only fires when the Wanderer actually opens the app. A6 is the only feature on the board that reaches a drifting Wanderer who isn’t logging in, which is precisely the behavior the M3 data says defines them. Tie it to the retention data: the Month 0→1 drop is the biggest leak in every cohort, and that leak is users quietly disengaging in their first weeks. An off-app re-engagement channel directly fights that leak in a way no homepage feature can. So the data arguably makes A6 a leading-value feature, not a nice-to-have. I’m holding it at Fill-In for the pilot because it’s a reasonable call, but the honest note is that the M3 data underwrites it more strongly than the quadrant shows, and it’s the first card I’d promote if the pilot signal comes in thin.

One thing the AI got right on the M3 side, worth stating: it correctly elevated features that serve the Wanderer’s passivity (A1 default rail) over features that serve curation enthusiasm (A7 curator-following), which matches the data showing the payoff concentrates in the low-curation Wanderer segment, not the already-curated Power User.

## Generate your interactive roadmap
- **My “Now” lane (this sprint), the 2 to 3 quick wins I’ll build first:** Four quick wins, all Effort 1-2, all aimed at one job: get a passive Wanderer to a curated title they’ll still be watching at minute 20.

A1 Spotlight Curated Rail — the core intervention. A default hand-picked rail that replaces the zero-payoff scroll with zero effort from the user. Everything else supports this.
A2 “Why You’ll Love This” Label — a reason at the point of choice, converting a browse into a press-play.
A6 Spotlight Digest Email — the only feature that reaches a Wanderer who logs in 1.1×/week, so it fights the churn that happens off-app.

A3 (Hidden Gem Badge) is the fourth, included because it’s nearly free. If forced to 3, A1 + A2 + A6 are the irreducible core: rail, reason, reach. The job of the sprint is build and instrument, not prove the metric, three weeks at 1.1 logins a week isn’t enough sessions to read the 20-minute rate cleanly.
- **What I cut, and the “no” I’m protecting the scope from:** Cut A8 Watch Party, A9 Advanced Filter Engine, A10 Offline Download. Two came from Sales, one from Engineering, and none came from the user research. Each fails the Wanderer on both axes: wrong persona and too heavy for the window. A9 is the sharpest cut, more filters add effort at the exact point of choice, which deepens the moment of misery instead of removing it.

The “no” I’m protecting: no feature earns a slot because a stakeholder wants it; it earns a slot by moving a passive viewer’s 20-minute watch rate. That single rule is what keeps a 3-person, 3-week sprint from being hijacked by a sales demo or an engineer’s filter preference. I also deferred A5 (right feature, can’t build and measure an AI queue in 3 weeks) and A4 (asks the passive persona to act first), so “not now” is doing as much work as “no.”
- **Prototype/roadmap screenshot link (paste into your deliverables):** https://claude.ai/artifact/9uNUgW27ekFbxQ21UhinjC
