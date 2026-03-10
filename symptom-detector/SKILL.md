---
Name: symptom-detector
Description: Separates what a team is observing from what is actually causing it — then generates competing root cause hypotheses with specific tests to disprove each one. Use this skill when someone describes problems they're seeing but aren't sure of the cause, says things like "we keep seeing X but don't know why", "we fixed it but it came back", "call volumes are up", "satisfaction is dropping", or shares any list of observations, complaints, or metric changes. Also trigger when the Problem Statement Stress Test has flagged likely symptom framing and the user wants to dig into root causes. This is Tool 2 in the Pressure Tools framing chain.
---

# Symptom vs Cause Detector

*Part of the Pressure Tools suite — a set of adversarial thinking tools for
design consultants, researchers, and product teams. This is Tool 2 of 9,
and the second step in the framing chain.*

---

## What This Tool Does

Teams routinely confuse what they observe with what is causing it. The
distinction matters enormously: treating a symptom as a cause sends teams to
solve the wrong thing, and the problem comes back.

This tool takes whatever a team is observing — complaints, metric drops,
behavioural patterns, operational failures — and does two things. First, it
separates symptoms from mechanisms from possible causes. Then it generates
a structured set of competing root cause hypotheses, each with a specific
test that would rule it out.

The output is not a single "root cause." It's a set of competing explanations
the team can investigate in parallel — with clear stopping conditions for
each. That's what forces intellectual honesty: teams commit to investigating,
not assuming.

---

## How to Open the Conversation

**If arriving directly at this tool:**

> *"What are you seeing? Describe the symptoms — what's happening that
> shouldn't be, or not happening that should be."*

If product or service context doesn't follow naturally, ask:
> *"And what's the context — what service or product is this happening in?"*

**If arriving via handoff from the Problem Statement Stress Test:**

The stress test may have already surfaced symptom framing — a problem
statement that describes impact rather than cause. If that context is present
in the conversation, use it. Open with:

> *"The framing we looked at was describing the impact — [restate the symptom
> briefly]. Let's work out what might actually be causing it. What are you
> observing in practice — the specific things you're seeing or measuring?"*

Don't start from scratch if context already exists. Build on it.

---

## Minimal Inputs to Proceed

- Observable symptoms — even one is enough to start
- Service or product context

Everything else (known changes, system constraints, actors involved) enriches
the analysis. Draw it out conversationally if relevant, not as a form.

---

## Step 1: Classify What's Been Provided

Before generating hypotheses, sort what the user has given into three
categories. Do this briefly and visibly — it builds trust in the analysis
that follows.

**Symptoms** — observable effects. What can be seen, measured, or reported.
Things happening that shouldn't be, or not happening that should be.
*Examples: call volume up 40%, customers abandoning at step 3, staff overtime
rising, NPS dropped 12 points.*

**Mechanisms** — plausible intermediary processes. Things that could connect
a cause to the observed symptoms but aren't yet confirmed.
*Examples: onboarding flow is confusing, agents don't have the right
information, the handoff between teams is breaking down.*

**Assumed causes** — explanations the team has already formed an attachment
to, often without evidence. Surface these explicitly — they are hypotheses,
not facts, and need to be tested alongside the others.

If the user has provided only mechanisms or assumed causes, name this and
ask for the underlying observations: *"That sounds like a possible explanation
rather than what you're directly observing — what are you actually seeing
that makes you think that?"*

---

## Step 2: Generate Root Cause Hypotheses

Produce 3–5 competing hypotheses grouped by category. Not every category
will apply — use the ones relevant to the context.

**Policy** — rules, procedures, or governance that constrain what people can
do. The cause is in what people are required to do or prohibited from doing.

**Process** — how work actually flows, handoffs, sequencing, or coordination
failures. The cause is in how things get done, not what people are capable of.

**Technology** — tools, systems, or infrastructure. The cause is in what the
technology does or fails to do, not in human behaviour.

**Capability** — knowledge, skills, or capacity. The cause is in whether
people can do what's needed, not whether they're trying to.

**Incentive** — what people are rewarded or penalised for, formally and
informally. The cause is in what behaviour the system actually encourages,
regardless of what it intends.

For each hypothesis:
- State it as a testable proposition, not a vague possibility
- Note which observed symptoms it would explain
- Assign a rough plausibility: **more likely**, **plausible**, or **worth
  ruling out** — based on what the inputs suggest

Be prepared to say which hypothesis is most plausible and why. Hedging every
hypothesis equally is less useful than a considered view with transparent
reasoning.

---

## Step 3: Disproof Tests

For each hypothesis, provide one specific piece of evidence that would rule
it out.

This is the most practically valuable part of the output. It gives the team
clear stopping conditions for investigation — they know when they can move on
from a hypothesis rather than investigating indefinitely.

Make the disproof tests concrete and actionable:

*Not:* "Check whether the process is the issue."
*Instead:* "Pull the last 20 support tickets and check whether agents had
access to the account history at the point of the call — if they did, process
access isn't the cause."

*Not:* "Survey users to see if they understand the onboarding."
*Instead:* "Watch three new users complete the setup wizard without assistance
— if they reach step 4 without confusion, the interface isn't the primary
cause of drop-off."

---

## Step 4: Most Likely Causal Path

Map one chain: symptom → mechanism → probable cause.

This is a working hypothesis, not a conclusion. State it as such. Explain
the reasoning that makes this path more plausible than the others given
the available evidence.

Format loosely:
*"The most plausible path here is: [observed symptom] is being produced by
[mechanism], which is itself caused by [probable cause]. The reason this holds
together better than the alternatives is [one or two sentences of reasoning]."*

---

## Step 5: Misdiagnosis Risk

Name the most commonly assumed cause for this type of situation — the
explanation the team is most likely already attached to.

Then describe specifically what the team would waste time doing if that
assumption turns out to be wrong.

This is often the most useful sentence in the whole output. It creates the
productive doubt that makes investigation feel worthwhile rather than
bureaucratic.

*Example: "If the team assumes this is a training problem and invests in
better onboarding for agents, but the actual cause is that the CRM doesn't
surface account history at the right point in the call, the training will
produce no measurable change and the team will have spent six weeks on the
wrong intervention."*

---

## Orientation Mode

Infer from the inputs which mode is most relevant and state it in one
sentence.

- **Behaviour mode** — the symptoms involve what people do or don't do:
  adoption failures, compliance gaps, habit patterns, workarounds. Hypotheses
  focus on incentives, capability, and what the system actually rewards.

- **Experience mode** — the symptoms involve how people feel, what they
  report, or how they perceive the service. Hypotheses focus on expectation
  gaps, perception mismatches, and moments of trust erosion.

- **System mode** — the symptoms involve flows, volumes, throughput, or
  structural interactions. Hypotheses focus on process design, bottleneck
  migration, feedback loops, and technical dependencies.

Only ask the user to confirm the mode if it's genuinely ambiguous and the
choice would materially change the hypotheses generated.

---

## Confidence Score

End the analysis with a score between 0.0 and 1.0.

Follow it immediately with one sentence on what's driving it and one sentence
on what would raise it.

This tool's confidence is most affected by:
- How specific the symptoms are (vague observations produce speculative
  hypotheses)
- Whether temporal context exists — knowing when symptoms started often
  unlocks the most useful hypotheses
- Whether the actors and their roles are clear

Example:
*"Confidence: 0.65 — the symptoms are clear enough to generate useful
hypotheses, but without knowing when this started or what changed around
that time, the causal path is speculative. A timeline of recent changes
would sharpen this significantly."*

---

## Concrete Next Step

End with one specific action — not a list.

Usually this is: which hypothesis to investigate first, and the single
fastest way to generate evidence that either confirms or rules it out.

Examples:
- *"The fastest thing to do is test the policy hypothesis first — it's the
  most disruptable if wrong and takes an afternoon to rule out. Pull the last
  month of escalation logs and check whether they cluster around one policy
  constraint."*
- *"Before anything else, establish a timeline — when exactly did call volumes
  start rising, and what else changed that week? That single question will
  eliminate at least two of the hypotheses above."*

---

## Chain Handoff

*"Once you've investigated the most likely hypothesis and have a clearer view
of the cause, the Decision Gate can help you work out which one to address
first and whether you have enough to act — especially if there are multiple
plausible causes competing for attention."*

Only deliver this if it's genuinely useful given the conversation. If the
path forward is obvious from the analysis, close with the next step instead.

---

## Edge Cases

**Symptoms are very broad — "poor service", "low morale", "bad experience."**
Don't proceed on these. Ask for one concrete example: *"Can you give me a
specific instance of that — something you actually observed or a piece of
feedback that made you think this was a problem?"* Specificity is the
prerequisite for useful hypotheses.

**User has already formed a strong diagnosis.**
Don't validate or dismiss it. Place it explicitly as one hypothesis in the
set, labelled as "currently assumed cause," and test it alongside the others
with equal rigour. The output will either confirm it with better grounding or
productively complicate it.

**No temporal context — the user doesn't know when symptoms started.**
Flag this directly: *"Knowing when this started — and what else changed around
that time — is often the single most useful input for this kind of analysis.
Do you have any sense of when it began?"* Temporal context often rules out
entire hypothesis categories immediately.

**The symptoms are actually a mix of unrelated problems.**
Name this. If the observations span two distinct systems or contexts, separate
them and run the analysis on each independently. Combined symptom sets produce
confused hypothesis sets.

**User arrives frustrated — they've already tried to fix this and it came back.**
Acknowledge this briefly before proceeding: *"That pattern — fix it, it comes
back — usually means the intervention addressed a mechanism rather than the
cause. Let's see if we can find what's actually upstream."* Then move directly
into the analysis.
