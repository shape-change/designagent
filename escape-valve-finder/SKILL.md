---
Name: escape-valve-finder
Description: Pre-plans what gets cut before delivery pressure forces improvised decisions — designing tiered contingency cuts with specific trigger conditions while the team is still calm. Use this skill when someone is planning a delivery with known risk factors, says things like "what happens if we fall behind", "I'm worried about the timeline", "we have a fixed deadline and things could go wrong", or has just completed scope planning and wants to prepare for slippage. Also trigger immediately after the Delivery Scope Filter when risk factors are present. This is Tool 7 of 9 in the Pressure Tools suite and the second step in the delivery chain.
---

# Escape Valve Finder

*Part of the Pressure Tools suite — a set of adversarial thinking tools for
design consultants, researchers, and product teams. This is Tool 7 of 9,
and the second step in the delivery chain.*

---

## What This Tool Does

When delivery pressure hits, teams make their worst decisions. Cuts get
made based on sunk cost bias, stakeholder fear, and whoever shouts loudest
— not on rational assessment of what matters most. The things that should
be cut stay in because they've been worked on for months. The things that
can be safely removed get defended because a stakeholder mentioned them once.

This tool designs the contingency before any of that pressure exists.
Tiered cuts, made rationally, with specific trigger conditions — so when
things slip, the team reaches for a plan rather than improvising a crisis.

The framing matters: this is not planning to fail. This is what professional
delivery looks like. The question is never whether cuts will happen on a
project with real complexity and a fixed deadline. It's whether they'll be
planned or panicked.

---

## How to Open the Conversation

> *"What's in scope for this delivery — and what are the risk factors
> that could put the timeline under pressure?"*

Sunk costs and stakeholder commitments are important but sensitive context.
Draw these out after the basics are established — once the user is
comfortable with the process, they'll name them:

> *"What's already been invested that the team would find hard to cut,
> even if it made sense to? And what's been promised to stakeholders
> that would be a difficult conversation to revisit?"*

**If arriving via handoff from the Delivery Scope Filter:**
The scope classification is already done. Open with:
*"Now that we have the scope prioritised, let's plan the escape routes —
what are the risk factors that could put the timeline under pressure?"*

Don't re-do the scope work. Build on it.

---

## Minimal Inputs to Proceed

- Current scope — even a rough list
- Deadline
- At least one risk factor

Sunk costs and stakeholder commitments enrich the analysis significantly.
Draw them out conversationally once the basic picture is established.

---

## Reading the Delivery Before Planning Cuts

Before designing the tiers, read the scope and risk factors for three
things:

**Where is the timeline most fragile?**
Risk factors cluster. A delivery that depends on an external API, a
team member who's leaving, and a QA process that hasn't been stress-tested
is fundamentally different from a delivery where the risks are internal
and controllable.

**What has sunk cost protection?**
The items that have been in development longest, or that represent the
largest prior investment, will be hardest to cut rationally. Name them
before they become the source of bad decisions.

**What are the stakeholder tripwires?**
Some scope items, if cut, require a difficult conversation. Knowing which
ones they are — and who owns that conversation — is part of the plan.

---

## The Three Cut Tiers

### Level 1: Early Slippage Cuts (10–20% timeline slippage)

The items that can be removed with minimal disruption to the core
delivery. These should feel almost easy to agree to in advance — that's
the test. If Level 1 cuts feel painful in the planning session, they'll
be impossible under pressure.

Level 1 cuts typically include:
- Polish and non-essential UX refinements
- Nice-to-have features with no dependency chains
- Reporting or analytics that aren't user-critical
- Administrative tooling that can be done manually at first

For each Level 1 cut: state what it is, what it affects (if anything),
and the trigger condition that activates it.

### Level 2: Significant Slippage Cuts (20–40% timeline slippage)

More substantial removals. These will hurt — there will be stakeholder
conversations, and some of the cuts will be things the team has
invested time in. But they're still rational: the core delivery
survives and delivers genuine value.

Level 2 cuts typically include:
- Non-core features that were Should Haves in the scope filter
- Integration work that can be deferred to a second phase
- Mobile or cross-platform versions that can follow the core delivery
- Features that serve secondary user groups rather than the primary one

For each Level 2 cut: state what it is, the stakeholder conversation
required, and the trigger condition.

### Level 3: Minimum Viable Delivery (near-failure conditions)

What's left if almost everything goes wrong. The absolute floor — the
thing that can be shipped that still represents genuine value delivered.

This tier requires a honest answer to: what is the irreducible minimum
that makes this delivery worthwhile? Not what the team wishes could be
the minimum. What it actually is.

For Level 3: describe the minimum viable delivery in one paragraph.
What does it do? What does it explicitly not do? Who does it serve and
how?

---

## Cut Triggers

For each tier, define specific observable signals that activate the
cuts — not vague conditions like "if things are going badly."

Triggers should be events the team can see without interpretation:

*Not:* "If the timeline is looking tight."
*Instead:* "If the [specific integration] dependency isn't confirmed
by [date], Level 1 cuts activate automatically."

*Not:* "If we're falling behind."
*Instead:* "If the [milestone] isn't complete by [date], the team
convenes within 48 hours to assess whether Level 2 applies."

Good triggers remove the need for a difficult judgment call in the
moment. They convert "should we cut this?" from a political
conversation into a conditional one that was already agreed.

---

## Cascading Impacts

For each significant cut, map what it breaks or degrades downstream.

Cuts that look clean often aren't. Removing a feature that seemed
standalone can degrade another feature's usefulness, break a user
journey, or require additional work to patch the gap it leaves.

Surface these dependencies before they become surprises:
*"Cutting the email notification system also affects the user
reactivation flow — users who don't complete onboarding in one
session currently get a reminder. Without notifications, that
recovery mechanism is gone. The cut is still Level 1, but the
impact on activation metrics should be noted and tracked."*

---

## Sunk Cost Traps

Name explicitly the items where prior investment will make rational
cuts emotionally difficult.

The goal is not to shame the investment — it's to identify in advance
where the team will face pressure to keep something in because of what's
already been spent, rather than because of what it's worth keeping for.

Naming sunk cost traps in the calm planning session creates a reference
point for the pressure moment:
*"Six months of mobile development will be the hardest Level 2 cut to
make. The rational case for deferring it is clear — it's not on the
critical path and the timeline risk it represents is higher than its
v1 value. But the prior investment will make this conversation
difficult. The team should agree now, in principle, that sunk cost
is not a reason to keep something in scope."*

---

## Tone and Framing

Matter-of-fact and pre-emptive. The emotional register is calm
competence, not pessimism.

If the user or team seems resistant to the exercise, address it
directly and early — don't wait for it to undermine the output:

*"This isn't planning to fail. This is what experienced delivery
looks like. Every project with real complexity and a fixed deadline
will face decisions about what gets cut. The only question is whether
those decisions are made now, rationally, with everyone in agreement
— or at 11pm before a launch, under pressure, by whoever is most
stressed. This tool is for the first version of that conversation."*

---

## Orientation Mode

Infer and state in one sentence.

- **Behaviour mode** — cuts are assessed by what users can no longer
  do. Prioritise preserving the core user actions; cut what affects
  secondary or edge case behaviours first.

- **Experience mode** — cuts are assessed by how the product feels
  after them. Prioritise cuts that users won't notice over cuts that
  make the product feel incomplete or broken.

- **System mode** — cuts are assessed by what they leave behind
  technically. Prioritise clean removals over cuts that leave
  architectural debt or unstable dependencies.

---

## Confidence Score

End with a score between 0.0 and 1.0, followed by one sentence on what's
driving it and one on what would raise it.

This tool's confidence is most affected by:
- How specific the risk factors are
- Whether sunk costs and stakeholder commitments have been named
- How complete the scope picture is

Example:
*"Confidence: 0.7 — the scope and risk factors are clear enough to
design useful tiers, but the stakeholder commitments haven't been
fully named, which means some of the Level 2 cuts may be harder
politically than the plan currently reflects. A clearer picture of
what's been promised to whom would sharpen the trigger conditions."*

---

## Concrete Next Step

One action — usually getting the cut plan agreed before delivery begins,
while everyone is still calm and rational.

Examples:
- *"The most important thing is to get the Level 1 and Level 2 cuts
  agreed by the core team before delivery starts — not as a sign of
  low confidence, but as a professional commitment to rational
  decision-making when pressure arrives. Schedule that conversation
  this week."*
- *"The Level 3 minimum viable delivery needs to be shared with the
  key stakeholder before development begins — they need to know it
  exists as a floor. That conversation is easier now than at a
  launch review."*

---

## Chain Handoff

This tool is typically the end of the delivery chain. No outbound
chain by default.

**If the cuts feel too severe and scope needs revisiting:**
*"If the escape valves here feel like they'd leave too little to
be worth launching, it might be worth going back to the Scope Filter
to tighten the Must Have list further before delivery begins —
better to reduce commitments now than to plan cuts that gut the
value proposition."*

---

## Edge Cases

**Team resists the exercise entirely.**
Reframe before proceeding. Don't argue for the tool — describe the
alternative:
*"Every delivery with real complexity faces cuts. The question
isn't whether they'll happen — it's whether the team decides them
now, together, calmly, or someone decides them alone at a crisis
point. This exercise is 90 minutes now versus a much harder
conversation later."*

**Nothing feels cuttable.**
Name what's creating that feeling before proceeding:
*"When nothing feels cuttable, it's usually because of sunk cost
investment, stakeholder commitments, or because every item feels
personally owned by someone in the room. Let's name those forces
directly — what specifically makes each item feel impossible to
remove?"*
Work through the blockers rather than the scope list.

**Stakeholder commitments make cuts seem politically impossible.**
Acknowledge the political reality without accepting it as a constraint:
*"Disappointing a stakeholder in a planned, early conversation where
you're still in control of the narrative is genuinely better than
delivering late or partially at the end. The conversation you'd have
now is a different conversation to the one you'd have at a launch
review."*

**The delivery has already started and is already slipping.**
The tool still has value but the framing shifts:
*"The pre-planning moment has passed, but the cut tiers are still
more useful than improvising. Let's work with the current state —
what's the realistic remaining timeline, and what's in flight that
could be descoped without restarting work that's already done?"*

**Risk factors are entirely external and uncontrollable.**
Acknowledge this directly. The cut tiers become more important, not
less, when the risks are outside the team's control:
*"When the risks are external — a dependency, a supplier, a
regulatory timeline — the cut plan becomes the primary risk
management tool. The team can't control the external factor;
they can control how they respond when it moves."*
