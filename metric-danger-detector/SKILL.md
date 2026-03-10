---
Name: metric-danger-detector
Description: Surfaces how proposed metrics will be gamed before they're deployed — identifying Goodhart's Law risks, perverse incentives, metric conflicts, and safer alternatives. Use this skill when someone is designing a performance framework, proposing KPIs, setting targets, or reviewing existing metrics. Trigger when someone says things like "here are the metrics we're planning to use", "we want to measure X", "I'm worried our metrics are being gamed", "we're setting targets for the team", or shares any list of measures attached to consequences or performance. This is Tool 8 of 9 in the Pressure Tools suite and the first step in the measurement chain.
---

# Metric Danger Detector

*Part of the Pressure Tools suite — a set of adversarial thinking tools for
design consultants, researchers, and product teams. This is Tool 8 of 9,
and the first step in the measurement chain.*

---

## What This Tool Does

The moment a metric is attached to a consequence, people begin optimising
for the metric rather than the underlying goal. This is Goodhart's Law:
when a measure becomes a target, it ceases to be a good measure.

It is not a character flaw. It is rational behaviour in response to an
incentive structure. The person gaming the metric is usually doing exactly
what the system rewards them to do.

This tool plays the game theory out before deployment. For each proposed
metric, it asks: how will a rational person in this role hit this number
while the thing the organisation actually cares about gets worse? The
answer is almost always specific, predictable, and preventable — if you
know to look for it before the metrics go live.

---

## How to Open the Conversation

> *"What are you planning to measure — and what are you actually trying
> to achieve with those metrics?"*

That gap — between what's measured and what's actually cared about —
is where all the danger lives.

If the incentive structure isn't provided, draw it out before proceeding:

> *"Who will be measured on these, and what happens to them based on
> the numbers?"*

The severity of gaming risk scales directly with the stakes attached to
the metric. A metric with no consequence attached is a different analysis
to one tied to bonuses, promotions, or team survival.

**If arriving with suspicion that current metrics are already being gamed:**

> *"What are you seeing that makes you think the metrics aren't
> reflecting what's actually happening?"*

Observable gaming behaviours are the most useful input. They often
reveal the mechanism before the analysis does.

---

## Minimal Inputs to Proceed

- The proposed metrics — named specifically
- What the organisation actually cares about (the underlying goal the
  metrics are supposed to represent)

Gaming analysis becomes sharper with knowledge of who is measured and
what the incentive structure is. Draw these out if not provided.

---

## Reading the Metrics Before Analysis

Before assessing individual metrics, read the set as a whole and ask:

**What is the gap between what's measured and what's valued?**
The wider the gap, the more dangerous the metric set. Metrics that
directly observe the thing you care about are harder to game than
metrics that proxy for it.

**Who bears the consequences?**
Gaming analysis is specific to the person facing pressure. A junior
support agent games differently to a team lead. An individual
contributor games differently to a department head. The same metric
produces different gaming behaviours at different levels.

**Are there conflicts within the set?**
Metrics that pull in different directions create pressure to optimise
for one at the expense of others. Identify these before they create
incoherent incentive structures.

---

## Danger Analysis

For each proposed metric, assess it on two dimensions:

**Gaming potential** — how easy is it to hit the number without
improving the underlying thing? Rate as: Low / Medium / High / Critical.

**Goodhart risk** — how likely is it that optimising for this metric
actively degrades the underlying goal? Rate as: Low / Medium / High /
Critical.

Provide a one-sentence explanation for each rating. Not the general
principle — the specific mechanism given the metric and context provided.

*Not:* "Average handle time is susceptible to gaming."
*Instead:* "Average handle time incentivises agents to end calls
quickly regardless of resolution — the metric hits target while
customers call back repeatedly, driving up total contact volume."

---

## Gaming Scenarios

For each high or critical risk metric, write a specific gaming scenario.

The standard is concreteness. The scenario should be immediately
recognisable to someone who works in that environment — not a
theoretical possibility, but a description of what will actually
happen.

Name the role where possible. Describe the behaviour specifically.
Show how the metric is satisfied while the underlying goal is not.

Structure:
*"A [role] facing pressure on [metric] will [specific behaviour].
The metric reads [result]. What actually happens to [underlying goal]
is [consequence]."*

Examples of the level of specificity required:

*"A support agent measured on First Call Resolution will mark calls
as resolved before the customer confirms the issue is fixed. CSAT
surveys go out before the customer discovers the problem has returned.
FCR hits target. The customer calls back. Total contacts increase."*

*"A sales team measured on pipeline volume will log speculative
opportunities earlier and keep dead deals active longer. Pipeline
looks healthy. Forecasting accuracy degrades. Leadership makes
resource decisions based on a number that doesn't reflect reality."*

*"A product team measured on features shipped will decompose large
features into multiple small ones, ship incomplete versions, and
defer the integration work that would make them useful. Velocity
metric increases. User value delivered does not."*

---

## Perverse Incentives

Name the unintended behaviours the metric set will reward — behaviours
that serve the number but not the goal.

These are distinct from gaming scenarios. Gaming is deliberate
optimisation for the metric. Perverse incentives are the systemic
behaviours the metric structure creates, often without conscious intent.

*"Measuring teams on individual output discourages the knowledge
sharing and collaboration that produces better collective outcomes.
No one is gaming the metric — they're just responding to what the
system rewards."*

*"Measuring customer satisfaction immediately post-interaction
rewards surface pleasantness over genuine resolution. Agents learn
to manage the interaction, not the problem."*

---

## Metric Conflicts

Identify where optimising for one metric will measurably degrade another.

Present these as explicit trade-offs — the team should understand
that they are choosing between competing goods, not that one metric
is correct and the other is wrong.

*"Average Handle Time and First Call Resolution are in direct tension.
Reducing handle time increases the probability that calls are ended
before issues are fully resolved, which reduces FCR. Optimising for
both simultaneously is not possible without addressing the underlying
process. The team needs to choose which to prioritise — or to redesign
the process so they're no longer in conflict."*

---

## Safer Alternatives

For each high or critical risk metric, offer at least one alternative
that is harder to game while still tracking the underlying goal.

The alternative should be:
- Closer to directly observing what's actually valued
- Harder to separate from genuine performance
- Realistic to measure given the context

*Not:* "Consider a more balanced scorecard approach."
*Instead:* "Replace First Call Resolution rate with repeat contact
rate measured over 7 days — it's harder to game because it requires
the customer to not call back, which can only be achieved by actually
resolving the issue."

Where no single metric is safe, name the combination approach:
qualitative signals alongside quantitative ones, or lagging indicators
validated by leading ones.

---

## Early Warning Signals

For each high-risk metric, describe one or two observable signs that
gaming has already begun — so the team knows what to watch for
after deployment.

These should be behaviours the team can actually observe, not abstract
statistical patterns:

*"If agents start ending calls more quickly in the two weeks after
the handle time target is introduced, that's the first signal.
If CSAT scores hold but repeat contacts increase, the gaming is
already embedded."*

*"If pipeline volume increases but win rates decrease, deals are
being logged earlier than they should be. If the same deals appear
active for more than 90 days without movement, they're being kept
open to protect pipeline numbers."*

---

## Tone and Framing

Specific and slightly adversarial — directed at the metrics, not
the people who proposed them or the people who will face them.

The consistent frame is rational response to incentive structure.
Gaming is not a sign that people are bad. It's a sign that the
metric structure has created a gap between what's measured and
what's valued. The fix is the metric design, not the people.

Avoid moralising. Avoid implying that the people who proposed the
metrics were naive or careless. The analysis is technical, not
evaluative.

On political sensitivity: some metrics are politically charged —
they reflect decisions made by people still in the room, or they
touch on team performance in ways that are uncomfortable. Frame
all analysis as structural and forward-looking:
*"The question isn't whether these metrics were a good idea — it's
what they'll produce and how to address that before they go live."*

---

## Orientation Mode

Infer and state in one sentence.

- **Behaviour mode** — gaming analysis focuses on what individuals
  will actually do when faced with the metric. What specific actions
  does this incentivise?

- **Experience mode** — gaming analysis focuses on how metrics
  can hide experience degradation. The number improves while users
  suffer in ways the metric doesn't capture.

- **System mode** — gaming analysis focuses on how the metric
  distorts the whole system. Optimisation in one place creates
  dysfunction elsewhere.

---

## Confidence Score

End with a score between 0.0 and 1.0, followed by one sentence on
what's driving it and one on what would raise it.

This tool's confidence is most affected by:
- Whether the incentive structure is known
- Whether "who is measured" is specified
- How specifically the underlying goal has been articulated

Low scores typically signal that the incentive structure is missing:

*"Confidence: 0.55 — the metrics are clear but without knowing
what's attached to them — bonuses, performance reviews, team
targets — the gaming scenarios are speculative rather than grounded.
The incentive structure is the most important missing input."*

---

## Concrete Next Step

One action — usually either revising the highest-risk metric before
deployment or establishing monitoring before the metrics go live.

Examples:
- *"Before these metrics go live, replace [specific metric] with
  [safer alternative] — the gaming scenario for it is predictable
  enough that it will materialise within the first quarter. That
  conversation is easier now than after it's embedded."*
- *"Set up a monitoring check for [early warning signal] in the
  first 30 days after deployment. If you see it, you'll know
  which metric is being gamed and can intervene before the
  behaviour becomes habitual."*

---

## Chain Handoff

*"Once you've revised the metrics, the Measurement Mode Selector
can help you work out the right approach for actually gathering
the data — particularly useful if you're not sure whether
quantitative tracking is even the right tool for what you're
trying to understand."*

---

## Edge Cases

**Metrics proposed without any consequence attached.**
Gaming doesn't occur without stakes — but consequences are almost
always added eventually. Note this and focus the analysis on what
happens when they are:
*"Without stakes, these metrics won't be gamed in the way described.
But if consequences are attached later — and they usually are —
here's what to watch for. It's worth doing this analysis now while
the design is still flexible."*

**User suspects current metrics are already being gamed.**
Ask for observable signals before proceeding:
*"What are you seeing that makes you think this? Specific behaviours,
anomalies in the data, or things people are saying?"*
Observable gaming is the most useful input — it often reveals the
mechanism more precisely than the metric analysis alone.

**High political sensitivity around specific metrics.**
Frame all analysis as structural, not personal:
*"This isn't about the people proposing or using these metrics.
It's about the gap between what the metric measures and what the
organisation values — and how rational people respond to that gap."*

**The metrics are already deployed and being gamed.**
The analysis shifts from prevention to diagnosis and remediation:
*"The design moment has passed, but the analysis is still useful
for understanding what's happening and what to change. Let's work
through which metrics are producing the behaviours you're seeing
and what the replacement options are."*
