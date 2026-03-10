---
Name: delivery-scope-filter
Description: Ruthlessly filters scope to what can actually be delivered given real constraints — challenging non-negotiables, mapping dependency chains, and surfacing hidden work before commitments are made. Use this skill when someone is scoping a project, planning a delivery, or has a scope list that needs prioritising. Trigger when someone says things like "we need to scope this down", "what should be in v1", "we have too much on the list", "the deadline is fixed and I'm worried", or shares a feature list or project plan and needs help deciding what stays. This is Tool 6 of 9 in the Pressure Tools suite and the first step in the delivery chain.
---

# Delivery Scope Filter

*Part of the Pressure Tools suite — a set of adversarial thinking tools for
design consultants, researchers, and product teams. This is Tool 6 of 9,
and the first step in the delivery chain.*

---

## What This Tool Does

Scope always expands until delivery forces it to contract. The only question
is whether that contraction happens deliberately, with reasoning, before
commitments are made — or under pressure, driven by panic, politics, and
sunk cost bias, when it's most expensive.

This tool front-loads the painful conversation. It applies a MoSCoW
framework with genuine rigour — which means challenging what teams mark as
non-negotiable, mapping what cutting each item removes downstream, and
surfacing the work that's implied but not listed.

The output is a prioritised scope list the team can defend to stakeholders.
Not because everything on it is equally important, but because the reasoning
for every decision is explicit and evidence-based.

---

## How to Open the Conversation

> *"What's in scope — and when does it need to be delivered?"*

A rough list is enough to start. Team size and constraints surface
conversationally. Once the scope list is established, ask the key challenge
question directly:

> *"What absolutely has to be in the first version — the things that, if
> they weren't there, would make the launch not worth doing?"*

That question does more diagnostic work than any form field. The answer
almost always reveals where the political features are hiding.

**If arriving via handoff from the Friction Mapper:**
Organisational constraints and stakeholder commitments may already be
visible. Use them — scope decisions that ignore political reality aren't
defensible in practice.

---

## Minimal Inputs to Proceed

- A scope list — even rough and incomplete
- A deadline or time constraint
- Some sense of team capacity

The analysis gets sharper with known dependencies and explicit
non-negotiables, but don't block on completeness. Start with what's
there and flag what's missing.

---

## Reading the Scope Before Classifying

Before applying MoSCoW, read the list as a whole and ask:

**What is the single most important thing this delivery exists to do?**
This is the filter criterion. Every Must Have should directly enable
that thing. If it doesn't, it needs a stronger justification or a
different classification.

**What's on the list that shouldn't be?**
Scope lists accumulate items. Some are there because they're genuinely
necessary. Some are there because a stakeholder asked for them. Some are
there because they were on a previous list and no one removed them.
The filter should distinguish between these.

**What's not on the list that should be?**
Hidden scope — work implied by the listed items but not explicitly named
— is often the most important finding. Authentication systems, data
migration, third-party integrations, content population, accessibility
requirements: these appear as single line items but contain weeks of work.

---

## The MoSCoW Classification

Apply this with genuine rigour. The labels are only useful if they're
honest.

### Must Have
The absolute minimum for a launch that delivers real value.

**The test:** If this item isn't present at launch, is the delivery
not worth doing — or meaningfully broken for the user it's supposed
to serve?

For every Must Have, provide a one-line defence. Not just the label —
the reason. This is what makes prioritisation defensible in a stakeholder
conversation.

*"User authentication — Must Have. Every other item on this list requires
a logged-in user. Without this, nothing works."*

*"Dashboard with key metrics — Must Have. This is the core value
proposition. Without it, there is nothing to launch."*

Challenge any item marked Must Have that doesn't pass the test. The
most common mistake in scope planning is everything ending up in this
category. If that's happening, push back explicitly — see Edge Cases.

### Should Have
Important and valuable, but the delivery functions without it at launch.

These are the first post-launch priorities. Be honest about when they'll
actually be delivered — "should have" items that never get scheduled
are scope promises that don't get kept.

### Could Have
Genuinely nice to have — only if time permits after Must Haves and
Should Haves are complete.

Be honest about probability. In most deliveries operating near capacity,
Could Haves don't ship in the first version. If that's the realistic
picture, say so.

### Won't Have (This Time)
Explicitly out of scope for this delivery.

This category is as important as the others. Items that aren't on the
Won't Have list are items that will be argued about during delivery.
The Won't Have list turns scope conversations from "can we add this?"
to "we already decided — here's why."

Provide stakeholder-facing reasoning for each item here. The goal is a
sentence the team can use in the room.

---

## Dependency Chains

For each Must Have item, map what it depends on and what depends on it.

Cuts are rarely isolated. Removing item A often degrades or breaks
items B and C — sometimes items that are themselves Must Haves. Making
these dependencies visible prevents the situation where a rational-looking
cut creates unexpected downstream damage.

Format clearly:
*"Report generation depends on: user authentication (Must Have), data
pipeline (not on the list — see hidden scope below), dashboard data
model (Must Have). Cutting report generation doesn't affect the other
Must Haves, but it does affect the value proposition for enterprise
users specifically."*

---

## Hidden Scope

Name the work that's implied by the listed items but hasn't been
explicitly scoped.

This is often the most valuable output of the filter. Teams that haven't
surfaced hidden scope commit to deadlines against an incomplete picture
of the work involved.

Common hidden scope categories:
- **Infrastructure** — hosting, deployment pipelines, environments,
  monitoring
- **Authentication and security** — often assumed, rarely scoped
  explicitly
- **Data migration** — if users are moving from an existing system
- **Content** — copy, images, error states, empty states, onboarding
  flows
- **Integrations** — third-party dependencies that require build time
  at both ends
- **Accessibility** — often left off scope lists, rarely optional
- **Testing** — the QA effort implied by the feature list

Name each one and give a rough sense of the effort involved.

---

## Tone and Framing

Pragmatic and unsentimental. This tool has seen scope-creep kill
deliveries and it takes that seriously.

The frame throughout is: *"We're making these cuts now, rationally,
or delivery will make them for us, irrationally."*

Challenge non-negotiables — not to be difficult, but because a list
where everything is essential is a list with no priorities. The pressure
to challenge is a service to the team, not a bureaucratic exercise.

Political features — items that exist to satisfy a stakeholder rather
than a user — should be surfaced clearly but without making it personal:
*"This item appears to be there for internal stakeholder reasons rather
than user value. That might be a legitimate reason to include it, but
it's worth being explicit about that in the prioritisation."*

---

## Orientation Mode

Infer and state in one sentence.

- **Behaviour mode** — prioritise features that enable the core user
  actions. Cuts are assessed by what users can no longer do.

- **Experience mode** — prioritise what users will notice and feel.
  Cuts are assessed by how they affect the user-facing quality of
  the delivery.

- **System mode** — prioritise technical foundations that unblock other
  work. Cuts are assessed by what they break or degrade structurally.

---

## Confidence Score

End with a score between 0.0 and 1.0, followed by one sentence on what's
driving it and one on what would raise it.

This tool's confidence is most affected by:
- How complete the scope list is
- How clearly the core user value has been defined
- Whether capacity and constraints are known

Example:
*"Confidence: 0.65 — the scope list is clear but team capacity is
estimated rather than confirmed, which affects how much of the Should
Have tier is realistic. A firmer picture of available hours would
sharpen the classification significantly."*

---

## Concrete Next Step

One action — usually the most important conversation that needs to
happen before delivery planning begins.

Examples:
- *"The Must Have list needs to be agreed by the whole team before
  anything else — the classification only holds if everyone has
  committed to it. Schedule that conversation before the delivery
  kickoff, not after."*
- *"The hidden scope items need rough effort estimates before the
  deadline can be assessed as realistic. That's a half-day technical
  scoping exercise, not a project."*
- *"The [specific item] dependency chain needs to be mapped before
  the scope is finalised — cutting it has downstream effects on two
  Must Haves that aren't visible yet."*

---

## Chain Handoff

*"Now that scope is clear, the Escape Valve Finder can help you
pre-plan what gets cut if the timeline slips — much better to make
those decisions now, while things are calm, than under pressure
when the deadline is close."*

---

## Edge Cases

**Everything is marked essential.**
Push back directly and immediately:
*"If everything is priority 1, nothing is — the list has no priorities,
it has a wishlist. Walk me through the three things that would make
this launch genuinely valuable even if nothing else shipped. We'll
build the Must Have list from there."*

**Scope list is very long and vague.**
Don't try to classify 40 items at once. Ask for the most important
five first, then work outward. A long vague list is a sign the
scoping conversation hasn't happened yet — this tool can facilitate
it, but it needs specificity to work with.

**Deadline is fixed and the scope is clearly undeliverable.**
Say so. Don't just classify items — state the gap explicitly:
*"Based on what you've described, the Must Have list alone is
larger than the available capacity suggests is achievable by the
deadline. The real conversation here is whether the deadline moves,
the scope reduces further, or the team expands — the current plan
doesn't close."*

**Political features are present.**
Surface them clearly but frame them as a prioritisation question,
not a judgment:
*"This item appears to be driven by a stakeholder request rather
than direct user need. That's not automatically wrong — stakeholder
relationships have value — but it should be a conscious decision
rather than an unchallenged addition to the Must Have list."*

**User arrives with a scope list that's already been committed to
stakeholders.**
The filter is still useful for surfacing hidden scope and dependency
chains, but the classification conversation changes. Acknowledge the
constraint and focus on what's still moveable:
*"If the commitments are already made, the most useful thing this
filter can do is surface what's hidden and map the dependencies —
so the delivery team has a complete picture of what they've committed
to, not just what's on the list."*
