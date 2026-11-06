# Individual Insights: Development Process

> Module 6 · Launch Impactful GTM Plans, ★ Deliverable 6 (reflection)
>
Coming from deeptech, I expected product management to feel like a different language. It didn’t. In mechanical engineering you are metric-first whether you like it or not, a design hits the thermal spec or it doesn’t, and the course pointed that same discipline at something softer, a user’s behavior instead of a part’s performance. The 20-minute watch rate became my spec. The real adjustment was the ambiguity: in hardware my baseline comes off a sensor, while here it was a proxy I had to flag as an assumption and measure for real without the clean instrumentation I’m used to.

The output-to-outcome shift is where it clicked. Engineers ship outputs, the part, the feature, the rail, and the course kept pushing me past that to whether the behavior actually changed. The rail was never the point; the watch rate was. What I’ll carry is the vocabulary of measurement, north star, leading indicator, guardrail, and knowing which is which. In hardware I already think this way without the names, in-process readings that tell you early, field reliability that tells you late, constraints you cannot violate. Seeing software run on the same logic gave me a repeatable way to process a messy problem: start from the persona and the friction, define the one metric, write the hypothesis, and let that structure decide what ships and what gets killed. That is first-principles thinking in a new domain, and it is the piece I’ll move between hardware and software.

## Friction points

The baseline was the hardest single thing. I kept trying to state my primary metric’s current rate and realized the number wasn’t in my data, the closest figure was all-user and at the wrong threshold, and it probably overstated my actual segment. Working through it meant admitting the honest answer was “instrument it first,” and flagging 11% as a proxy rather than pretending it was fact. That one wrong cell cascaded into sample size, duration, and the split, so fixing it fixed four other things.

The second friction was separating the primary metric from the guardrail. I kept letting a session-length number leak into a metric that should have been a rate. They measure different things for different segments, and keeping them clean took real discipline

_____

## Key learnings

Constraints move the effort axis, not the value axis. When the timeline changed from three weeks to six months, the only feature that changed quadrant was the one that was worth building but blocked by time, the Sales and Engineering pet features stayed worthless, because their problem was never effort. Value is set by the persona, not the calendar.

“Quick win” and “must have” are different questions. The cheap, easy feature scored high on effort-value but was only a “could” on MoSCoW, because easy to build doesn’t mean necessary to ship. Running both frameworks on the same backlog showed me they rank things differently, and conflating them is how sprints fill with cheap optional work while the real must slips.

The dependency you don’t own can sink your metric. My 20-minute watch rate lived or died on a playback bug three teams away. Naming it as a blocking dependency was the one line that separated a real PRD from a wish, and the prototype proved it by mislabeling a buffering exit as a curation signal, exactly the confound I’d have missed on paper.

_____

## Aha! moment

The persona realignment. I built the whole case around Priya, the loyal film buff who scrolls and finds nothing, and then the segment data said the payoff wasn’t with her at all. By the numbers she’s a Power User who already retains. The money was with the Wanderer, the low-engagement drifter I hadn’t even interviewed. The aha: the persona you design for is not always the segment that pays off, and when the data relocates the opportunity, you follow the data instead of marrying the vivid story. Priya stayed as the human face, but the ROI lived one segment over.

_____
