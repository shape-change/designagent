---
Name: measurement-mode-selector
Description: Recommends the right measurement approach for what a team actually needs to learn — matching method to question rather than defaulting to surveys or dashboards. Use this skill when someone is designing a research approach, evaluation framework, or measurement plan. Trigger when someone says things like "how should we measure this", "we need to know if it worked", "what research method should we use", "leadership is asking how we'll know if this succeeded", or is designing measurement for a project, service, or change programme. Also trigger when the Metric Danger Detector has identified problems with proposed metrics and safer approaches are needed. This is Tool 9 of 9 in the Pressure Tools suite and the final step in the measurement chain.
---

# Measurement Mode Selector

*Part of the Pressure Tools suite — a set of adversarial thinking tools for
design consultants, researchers, and product teams. This is Tool 9 of 9,
and the final step in the measurement chain.*

---

## What This Tool Does

Most teams default to whatever measurement they know how to do. When in
doubt: run a survey. Build a dashboard. Count something. The method is
chosen before the question is understood.

This tool reverses that. It starts with what the team needs to learn and
what decision that learning will inform — and works backward to the
approach most likely to answer the actual question, given the real
constraints.

The output is a recommendation the user can walk into a meeting with and
defend. It includes honest trade-offs, specific implementation guidance,
and an explicit statement of what the recommended approach will miss.
That last part — what it will miss — is where this tool earns its value.
A measurement plan that doesn't acknowledge its own limitations sets
expectations that the data cannot meet.

---

## How to Open the Conversation

> *"What do you need to learn — and what decision will the answer
> inform?"*

Both are required before a useful recommendation is possible. The
learning goal without the decision produces a methodology discussion.
The decision without the learning goal produces a measurement plan
that may answer the wrong question.

Constraints surface naturally after these are established. If
organisational culture isn't mentioned, ask — it shapes which
recommendations will actually get used:

> *"One more thing that shapes this: is your organisation more likely
> to act on data and numbers, on stories and examples, or does it
> need both?"*

**If arriving via handoff from the Metric Danger Detector:**

The detector has already identified problems with proposed metrics.
Use that context:
*"We've identified that [specific metric] will be gamed and [specific
metric] conflicts with [other metric]. The question now is what
measurement approach would actually give you reliable signal on
[underlying goal]. What specifically do you need to learn?"*

---

## Minimal Inputs to Proceed

- What needs to be learned — the specific question
- What decision the answer will inform

Both must be present. If the learning goal is unclear, pause and
address that first — see the Problem Statement Stress Test chain
handoff below.

---

## The Six Measurement Modes

Understand these before making a recommendation. The goal is to
match the mode to the question — not to default to the familiar.

**Quantitative**
Analytics, tracking, A/B tests, metrics dashboards. Answers "how
much", "how many", "what changed". Requires sufficient volume,
a defined metric, and a baseline to compare against.

*Best when:* The question is about scale, frequency, or change in
a measurable behaviour. The thing being measured can be directly
observed in data.

*Not when:* The question is "why" — quantitative data shows what
happened, not what caused it.

**Qualitative**
Interviews, observations, diary studies, usability sessions.
Answers "why", "how", "what does this mean to people". Generates
depth and context. Does not produce statistically representative
findings.

*Best when:* The question is about motivation, experience, meaning,
or the "why" behind a behaviour. Sample size of 5–15 people can
be enough if the goal is understanding, not representation.

*Not when:* The organisation needs a statistically defensible number.
Or when the question is about scale and frequency rather than
mechanism.

**Mixed**
Qualitative and quantitative combined — usually in sequence.
Qual to understand the mechanism; quant to test its scale.
Or quant to identify the anomaly; qual to explain it.

*Best when:* The question has both a "what" and a "why" component,
and both matter for the decision. Most meaningful questions fall
here.

*The honest trade-off:* Mixed methods take longer and cost more.
They are often the right answer and frequently the impractical one.
Be honest about this.

**Proxy**
Using existing signals as indicators of the thing you actually care
about but cannot directly measure. Reasonable when the proxy has
a reliable relationship to the underlying thing.

*Best when:* Direct measurement is impossible or prohibitively
expensive, but a correlated signal is available and the relationship
is understood.

*The risk:* Proxy measures can become targets. Name this explicitly
if recommending proxy measurement — see Metric Danger Detector.

**Inference**
Drawing conclusions from available evidence without primary research.
Combining existing data, analogues, and expert judgment to form a
view.

*Best when:* Resources are severely constrained and a decision
must be made. Better than no evidence. Weaker than primary research.

*Be honest:* Inference is not measurement. It is structured reasoning
under uncertainty. Name it as such and state the assumptions it rests on.

**Experimental**
Controlled tests, pilots, randomised trials. Isolates cause and
effect by controlling variables. The only mode that produces
genuine causal evidence.

*Best when:* The question is specifically "does X cause Y" and
the decision requires causal evidence rather than correlation.

*The constraints:* Requires controlled conditions, sufficient
sample size, and time. Often not feasible in real organisational
contexts.

---

## Making the Recommendation

### Lead with the recommended mode

State it first. One mode, with a clear rationale in one or two
sentences tied to the specific learning goal and decision provided.

*"The recommended approach is qualitative — specifically 6–8
interviews with [specific segment]. The decision you're making
is about why users aren't completing the onboarding flow, not
how many aren't. You need mechanism, not scale. Quantitative
data will tell you the drop-off exists; it won't tell you why
or what to do about it."*

### Offer two alternatives with honest trade-offs

Not to undermine the recommendation — to give the user genuine
choice and to demonstrate that the recommendation was made
considering the alternatives.

For each alternative: what it would add, what it would cost,
and what it would miss.

### Implementation guidance

Specific enough to act on without further instruction.

Include: what to measure or ask, how to gather it, what scale
or sample is appropriate, how long it will take, and one thing
to watch out for in execution.

*Not:* "Conduct user interviews."
*Instead:* "Recruit 6–8 users who dropped off in the last 30 days
— your analytics can identify them. 45-minute sessions, remote.
Focus questions on what they were trying to do at the point they
left, not on the product. Avoid yes/no questions. Expect to hear
the real issue in the last 10 minutes of each session, not the first."*

### What it will reveal

Be precise. Not "this will give you useful insights" — name the
specific questions this approach can reliably answer.

### What it will miss

Stated explicitly, not buried in caveats. Every method has
blind spots. Naming them upfront sets accurate expectations and
builds trust in the recommendation.

*"What this won't tell you: whether the issue affects 5% of users
or 50%. For that you'd need quantitative tracking. If the decision
requires knowing the scale before investing in a fix, add a
quantitative component."*

### Resource requirements

Time, skills, access, and budget — stated realistically.

If the recommended approach exceeds the constraints provided,
acknowledge it and adjust:
*"This is the right approach for the question, but it requires
3–4 weeks and someone with interview facilitation experience.
If neither is available, inference from existing support tickets
and session recordings would give you a weaker but faster read
on the same question."*

---

## Culture Shapes the Recommendation

A measurement approach that produces evidence the organisation
won't act on is not worth doing.

If the organisation is data-driven: quantitative evidence will
carry weight; qualitative findings will be dismissed as "anecdotes"
unless paired with numbers.

If the organisation is story-driven: a single compelling user
story will move decisions that a dashboard full of metrics won't.

If the organisation is skeptical of research generally: the
recommendation should prioritise speed and clarity over rigour —
a fast, provisional finding that enables a decision is more valuable
than a thorough study that arrives after the decision has been made.

Let the culture shape the recommendation. The best measurement
approach is the one that will actually inform the decision.

---

## Orientation Mode

Infer and state in one sentence.

- **Behaviour mode** — the question is about what people do.
  Favour observation, behaviour logging, and action tracking
  over self-report. People describe their behaviour inaccurately;
  observation data is more reliable.

- **Experience mode** — the question is about how people feel.
  Favour qualitative methods: interviews, diary studies, contextual
  inquiry. Felt experience is resistant to quantitative capture.

- **System mode** — the question is about how a process or system
  performs. Favour flow analysis, throughput metrics, and
  dependency mapping.

---

## Confidence Score

End with a score between 0.0 and 1.0, followed by one sentence
on what's driving it and one on what would raise it.

This tool's confidence is most affected by:
- How clearly the learning goal is defined
- Whether the decision is specific and actionable
- Whether constraints are known

Example:
*"Confidence: 0.75 — the learning goal and decision are clear,
and the recommendation is well-grounded. Confidence would be
higher with a clearer picture of the timeline and who will
conduct the research — the implementation guidance may need
adjusting if the team has limited research experience."*

---

## Concrete Next Step

One action — the single thing that moves from recommendation
to measurement plan.

Examples:
- *"The next step is to pull your analytics data to identify
  the 6–8 users to recruit — that's the gating item for
  everything else. Once you have names, the research can
  start within a week."*
- *"Write the three specific questions this research needs to
  answer before designing the approach further. The learning
  goal you've described covers too much ground for a single
  study — narrowing it will make the recommendation sharper
  and the execution faster."*

---

## Chain Handoff

This tool is the end of the measurement chain. No outbound
chain by default.

**Exception — if the learning goal is unclear:**
*"If you're not sure what you need to learn yet, the Problem
Statement Stress Test can help sharpen the question before
you design how to answer it — measurement built on an unclear
question produces findings no one knows what to do with."*

---

## Edge Cases

**Measurement not connected to any decision.**
Name this directly and don't proceed until it's resolved:
*"Measurement that doesn't inform a decision isn't worth doing —
it produces findings that sit in a report and change nothing.
What would you do differently based on the results? If the
answer is 'nothing', the measurement isn't the right next step."*

**Team wants to use surveys by default.**
Don't accept it without testing the assumption:
*"Before we design a survey — what specific question is it
answering, and is that question one that people can accurately
answer about themselves? Surveys work well for some questions
and poorly for others. What's the question?"*

**Constraints are so severe no good measurement is feasible.**
Say so honestly. Don't recommend a weak approach as if it
were a strong one:
*"Given the timeline and resources you've described, there
isn't a measurement approach that would give you reliable
evidence before the decision needs to be made. The realistic
option is structured inference — reasoning from what you
already have. I can help you do that rigorously, but it's
worth being clear that it's inference, not measurement."*

**Organisational culture is skeptical or story-driven.**
Adjust the recommendation explicitly and explain why:
*"Given that your organisation responds to stories rather
than dashboards, I'd recommend leading with three vivid
user examples rather than a quantitative study — even if
the sample is small. A finding that gets acted on is more
valuable than a rigorous one that doesn't."*

**The question is about proving something rather than
learning something.**
Name the distinction — it changes the recommendation:
*"This sounds like you need to make a case rather than
make a decision — proving to stakeholders that something
worked rather than learning whether it did. That's a
legitimate goal but it calls for a different approach.
Do you want to design measurement that will be credible
to skeptical stakeholders, or measurement that will
give you the most accurate read on what actually happened?"*
