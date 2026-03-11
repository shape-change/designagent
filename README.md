# Design Agent

**A suite of adversarial thinking tools for Claude — built for teams who need to do more
before they commit.**

Each tool is a Claude skill: install it once, use it in any conversation.
No platform. No subscription. No login. Just better thinking.

---

## About

Shape & Change works across service design, organisational change, and product strategy.

These tools grew out of a platform we were building. Giving them away turned out to be a better idea.
If you use them and want to talk — or want someone in the room when it matters — shapechange.io

**[shapechange.io](https://shapechange.io)** — talk to me about work and say hello

---

## Why I made these

Have you ever worked on a project that fell apart because the foundation was shaky from day one? Humans are really good at solving symptoms instead of causes, mostly because we’re often too polite to admit when a "must-have" feature is actually a distraction or when the problem we're solving doesn't actually exist.

So, I decided to make some Claude Skills. The idea started out last December, when I was looking at this as a full platform with a subscription service, but with the rate of change in AI, that felt like the wrong move. I've bundled up the Skills as 'DesignAgent'.

I’ve spent time building, testing, and breaking them. I’ve iterated on them, tweaking the prompts and the logic every time they missed a nuance or let a weak assumption slide past. They’ve been "stressed" as much as they "stress-test".

---

## The toolkit

Nine tools across five domains, designed to chain together.

### Framing

**[Problem Statement Stress Test](./problem-stress-test/)**
Takes a draft problem statement and reads it the way the most rigorous
person in the room would — surfacing solution-shaped framing, bundled
problems, symptom confusion, vague language, and missing consequences.
Produces tighter alternative framings and the specific questions that need
answering before the framing can hold.
→ *Use before any research, discovery, or ideation begins.*

**[Symptom vs Cause Detector](./symptom-detector/)**
Separates what teams observe from what is actually causing it. Generates
3–5 competing root cause hypotheses grouped by category (policy, process,
technology, capability, incentive), each with a specific disproof test.
Identifies the most likely causal path and names the misdiagnosis risk —
what the team would waste time doing if the obvious assumption turns out
to be wrong.
→ *Use when you're seeing problems but don't know what's driving them.*

**[Decision Gate](./decision-gate/)**
Converts analysis into a clear decision stance — Stop, Pause for evidence,
Proceed with constraints, Run a test, or Proceed — and defends it with
grounded reasoning. Makes the cost of indecision as visible as the cost
of acting. Includes a regret check: a specific account of what the team
would wish they'd done differently in six months if the decision goes wrong.
→ *Use when analysis has happened but a decision hasn't.*

---

### Organisational

**[Friction Mapper](./friction-mapper/)**
Maps where organisational resistance will derail an initiative before it
launches. Surfaces friction points (rated: will slow / will block / will
kill), stakeholder tensions, hidden blockers, and political dynamics —
including who loses something if the initiative succeeds. Proposes
practical mitigation paths for the highest-severity friction points.
→ *Use before launching anything that requires people to change.*

**[Integration Mode Detector](./integration-mode-detector/)**
Detects whether an organisation is genuinely integrating new ways of
working or assimilating them — adopting the language of change while
keeping the same structures and behaviours underneath. Classifies the
situation (Assimilation / Genuine Integration / Hybrid / Transitioning),
names the say-do gaps explicitly, and assesses trajectory.
→ *Use when a change programme is underway and you're not sure it's sticking.*

---

### Delivery

**[Delivery Scope Filter](./delivery-scope-filter/)**
Filters scope to what can actually be delivered given real constraints —
challenging non-negotiables, mapping dependency chains, and surfacing
the hidden work implied by the listed items. Produces a MoSCoW
prioritisation with a one-line defence for every Must Have designation.
→ *Use before any delivery commitments are made to stakeholders.*

**[Escape Valve Finder](./escape-valve-finder/)**
Pre-plans the cuts before delivery pressure forces improvised ones.
Designs tiered contingency cuts (Level 1: 10–20% slippage / Level 2:
20–40% / Level 3: minimum viable delivery) with specific observable
trigger conditions for each tier. Names the sunk cost traps in advance
— the items where prior investment will make rational cuts emotionally
difficult.
→ *Use immediately after scoping, while the team is still calm.*

---

### Measurement

**[Metric Danger Detector](./metric-danger-detector/)**
Surfaces how proposed metrics will be gamed before they're deployed.
Plays the game theory out: for each metric, describes specifically how
a rational person in that role will hit the number while the thing the
organisation actually cares about gets worse. Identifies metric conflicts,
perverse incentives, safer alternatives, and early warning signals that
gaming has begun.
→ *Use before any performance framework or KPI set goes live.*

**[Measurement Mode Selector](./measurement-mode-selector/)**
Matches the measurement approach to what the question actually requires —
rather than defaulting to surveys or dashboards. Recommends one of six
modes (Quantitative / Qualitative / Mixed / Proxy / Inference /
Experimental) with specific implementation guidance, honest trade-offs,
and an explicit statement of what the approach will miss.
→ *Use when designing research, evaluation frameworks, or measurement plans.*

---

## How the tools chain together

Each tool produces outputs that become inputs to the next. Running a full
chain produces significantly more than the sum of the individual parts.

```
Framing a new piece of work
Problem Statement Stress Test → Symptom Detector → Decision Gate

Understanding organisational change
Integration Mode Detector → Friction Mapper → Decision Gate

Planning an initiative
Friction Mapper → Escape Valve Finder → Decision Gate

Scoping delivery
Delivery Scope Filter → Escape Valve Finder

Designing measurement
Metric Danger Detector → Measurement Mode Selector
```

Claude will suggest the next tool in the chain at the end of each
analysis — you don't need to navigate this manually.

---

## Installation

### Install a single tool

1. Download the folder for the tool you want (or clone the whole repo)
2. Zip the folder if it isn't already zipped
3. In Claude.ai: **Settings → Capabilities → Skills → Upload Skill**
4. Select the zipped folder
5. Toggle the skill on

### Install all nine tools

Download [pressure-tools-complete.zip](./releases) from the releases page.
It contains all nine skill folders. Install each one individually via
Settings → Capabilities → Skills.

### Use in Claude Code

Place the skill folder(s) in your Claude Code skills directory. Skills
activate automatically when relevant queries are detected.

---

## Using the tools

Once installed, you don't need to ask for a specific tool by name.
Just describe what you're working on:

> *"Here's our problem statement — we're trying to solve X..."*

> *"We keep seeing Y but we don't know why..."*

> *"We have a scope list and a deadline and I'm not sure it's achievable..."*

> *"We're rolling out a new performance framework — here are the metrics..."*

Claude will recognise when a Pressure Tool is relevant and use it.
If you want a specific tool, you can ask directly:

> *"Run the Friction Mapper on this initiative."*

> *"Use the Escape Valve Finder on this scope list."*

---

## Watch-outs

**These tools are diagnostic, not decisive.**
They surface what needs to be addressed — they don't make the decision
or have the stakeholder conversation for you. The output is input.
The most important work still happens in the room.

**They work best on real situations with real stakes.**
Hypothetical inputs produce speculative outputs. The more specific
and honest the input, the more useful the analysis. Don't sanitise
the context before sharing it.

**The confidence score.**
Every tool returns a confidence score with plain-language reasoning.
A score below 0.6 means the analysis is speculative — useful as a
hypothesis, not as a basis for significant decisions. Low confidence
usually means more context is needed, and the score will tell you
specifically what.

**Some outputs will be uncomfortable.**
These tools are designed to say things that comfortable conversations
avoid. The Integration Mode Detector may classify a change programme
as assimilation. The Friction Mapper may name resistors the team
hasn't wanted to name. The Metric Danger Detector may describe exactly
how the new performance framework will be gamed.

That discomfort is the point. It's better to surface these things
before significant investment has been made in the wrong direction.

**They are not a substitute for human judgment.**
The tools are rigorous, but they're working from what you tell them.
They can't observe the room, read the politics directly, or catch
the things you haven't thought to share. Use the outputs as a
starting point for a sharper conversation — not as a finished
analysis to be acted on without scrutiny.

**Don't run all nine on the same problem.**
The tool chains are designed for specific situations. Running every
tool on every problem produces analysis fatigue, not insight. Use
the quick-reference guide below to choose the right entry point.

---

## Which tool to start with

| If you need to... | Start here |
|---|---|
| Challenge a problem statement before research begins | Problem Statement Stress Test |
| Understand what's causing something you're observing | Symptom vs Cause Detector |
| Turn analysis into a clear decision | Decision Gate |
| Understand where an initiative will stall | Friction Mapper |
| Assess whether a change programme is actually working | Integration Mode Detector |
| Prioritise scope before delivery begins | Delivery Scope Filter |
| Pre-plan cuts before the deadline pressure hits | Escape Valve Finder |
| Check whether your metrics will be gamed | Metric Danger Detector |
| Choose the right measurement approach | Measurement Mode Selector |

---

## Contributing

This is an open toolkit. If you want to contribute a new tool, improve
an existing one, or adapt these for a specific domain:

1. Fork the repo
2. Follow the existing skill structure (each tool is a folder containing
   a single `SKILL.md` file with YAML frontmatter)
3. Open a pull request with a clear description of what the tool does
   and when it should trigger

New tools should follow the same design principles: one opening question,
diagnostic not judgemental, confidence score with plain-language reasoning,
one concrete next step, natural chain handoff.

---

## Licence

MIT — use these however you want. Credit appreciated but not required.
