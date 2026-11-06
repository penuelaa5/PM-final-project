# GTM Strategy & Success Dashboard (Module 6)

## Get your prior work ready
- **The feature you're launching from your M4 PRD, one feature, not a list:** A1	Spotlight Curated Rail
- **What your M5 experiment told you shipped / iterating, the evidence behind the launch:** Ship. The Spotlight rail cleared the pre-committed criteria: the 20-minute watch rate rose ≥2 points (11% → 13%+) for exposed Wanderers at p < 0.05, while the Power User guardrail held (session length and 58% curated share within 5%).
- **Your persona pull your M2 persona, this anchors your audience:** The Wanderer: 41% of the base, $8.40 LTV, 1.1 sessions/week, 18% curated / 61% trending. Opens the app passively out of habit, drifts through a trending feed, finds nothing worth staying for, and churns quietly, the segment where Spotlight moves churn the most (22 points when exposed, the largest effect of any segment).

## Set your goal, then your audience
- **Primary GTM goal awareness · engagement · conversion, pick one:** Engagement
- **Why this goal? what makes this the right goal for this feature right now:** Engagement is the lever that moves the 20-minute watch rate, which is the leading indicator ahead of the retention and churn payoff.
- **Target audience the specific segment your goal implies, be precise:** Active-but-shallow Wanderers - still opening the app (roughly 1.1 sessions/week), but exiting without reaching a 20-minute watch.

## Size your launch
- **Launch tier S (minimal) · M (targeted) · L (multi-channel) · XL (full GTM):** M (targeted)
- **Justification reach + revenue impact + what silence would risk:** ~41% of base reached; lowest per-user LTV ($8.40) but the largest aggregate churn opportunity (22-pt swing); silence risks non-adoption, Wanderers scroll past an unannounced rail and the engagement lift never materializes
- **Is this a launch or a release? does it need go-to-market, or can it just ship?:** Launch, light and targeted. The engagement goal requires the Wanderer to notice the rail, so it needs one in-app surfacing.

## Choose your top three channels and plan assets
- **Channel 1 owned / earned / paid, and why it reaches your audience:** Channel 1 — Owned, in-app. The rail placement plus a light surfacing nudge (“new: picked for you”).
- **Channel 2 owned / earned / paid, and why:** Channel 2 — Owned, email/push. Wanderers log in ~1.1×/week, so a big slice is drifting and won’t catch an in-app message. Email/push (a “this week’s picks” that links into the rail) .
- **Channel 3 owned / earned / paid, and why:** Channel 3 — Owned, lifecycle/notification. A push when the weekly picks refresh, or a continue-watching prompt. Gives the returning Wanderer a reason to come back, which is the engagement loop.
- **Enablement & assets what Sales / CS / Support need, plus the assets to build (one-pager, demo, etc.):** CS/Support: a short FAQ so they can answer “what is this rail / why did it appear / where did my usual rows go.” 
Internal one-pager: the feature, the Wanderer persona, the 20-min watch metric, the positioning (“Picked by StreamLine editors”), so marketing, CS, and the editorial team speak the same language.
Editorial/curator brief: how curators pick (tone, no spoilers, the human one-line note), since the curation is the product.
Assets to build: in-app nudge copy, the email/push creative, a 15-second demo GIF of the rail in action, the support FAQ, the one-pager.

## Make it executable
- **Ownership named owner per key activity, individual, not department:** In-app rail + surfacing nudge → Product Manager. Owns the feature and its placement.
Email/push lifecycle campaign → Lifecycle/CRM Manager. Owns the off-app reach.
Weekly curation (the picks themselves) → Editorial Lead. Owns what goes in the rail.
Instrumentation + A/B readout → Data Analyst. Owns the 20-min watch-rate measurement and the exit-classifier fix.
Playback dependency (BUG-1042/1061) → Eng Lead. Owns the blocker your metric depends on.
CS/Support readiness → Support Lead. Owns the FAQ and ticket deflection.
- **Budget & resource gaps what costs extra, and any asset you can't currently build:** The recurring cost everyone misses: human curation is ongoing opex, not a one-time build. Someone picks 6–10 films every week, forever. That’s standing editorial labor. 
Playback fix (BUG-1042/1061) is engineering cost. 
Lifecycle tooling for email/push.
Creative: demo GIF, email template, in-app nudge copy, minor design time.
What you can’t currently build: the true Wanderer 20-min baseline.
- **Timeline Phase 1 beta → Phase 2 launch moment → Phase 3 post-launch:** Phase 1 — Beta/Test (~2–3 weeks). Ship the rail to the Wanderer test cohort only, no marketing. Fix the two instrumentation bugs first, instrument the real baseline, run against the matched holdout, read the 20-min watch rate.
Phase 2 — Launch moment (post ship-decision). If the ship criteria clear, roll out to the full Wanderer segment and now turn on GTM: the in-app nudge plus the email/push announcing weekly picks. 
Phase 3 — Post-launch (weeks → Month 5–6). Weekly curation cadence runs; monitor the guardrail (Power User session length / 58% curated share, pause if either drops >5%); watch the lagging churn confirmation mature to Month 5–6; iterate the picks using the curation_signal exits to learn which titles miss.

## Define how you'll know it worked
- **Success metrics 2 to 3 metrics that match your GTM goal:** Feature adoption rate → % of exposed Wanderers who click into the rail. 
20-minute watch rate --> the share of exposed Wanderer sessions reaching 20 continuous minutes.
Time to first key action → keep. Time from app open to pressing play on a rail title. Directly measures the “zero effort, fast” promise against the 20-minute-scroll moment of misery.
- **Bad signal to watch for e.g. high reach, zero signups = message-market mismatch:** High adoption, low 20-min watch rate → the rail gets clicks but the curation misses. Fix the picks, not the placement.
Low adoption, but high watch rate among those who use it → the curation is good but nobody notices the rail. Fix the surfacing (the nudge, the placement), not the picks.
Watch rate up, but Power User session length or 58% curated share drops >5% → you won the Wanderer by bleeding the Power User. Pause and investigate, this is the guardrail breach, not a success.
- **Most likely post-launch decision double-down · iterate · pivot · deprioritize, and what would trigger it:** double-down. Trigger: the 20-min watch rate sustains at or above 13% across the full Wanderer rollout AND the Month-1 retention lift holds for the launch cohort. Then fund the A5 personalized queue to scale it.
