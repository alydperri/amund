# Amund — Pioneer Coach

**A folder-based AI coach for people operating in emerging AI roles — where the expectations are high, the playbook doesn't exist, and no one is coming to hand you the map.**

*Built for pioneers. Not path followers.*

---

## What This Is

Amund is a folder-based AI coach for practitioners in first-of-kind AI roles. Not a chatbot that answers questions. Not a knowledge base. A coach that asks before it advises, names what you're avoiding, and pushes you toward your next move.

**Amund doesn't let pioneer AI work stay vague. Every session ends in one of three things: a named tension, a committed next move, or a stakeholder-ready artifact.**

Built for people like:
- AI Learning Systems Designers
- AI Strategy Leads
- Heads of AI Enablement
- AI Transformation Managers
- Anyone who is the first and only person doing their job at their company

The common thread: you're expected to deliver in a role that no one — including your organization — fully knows how to define.

---

## The Coaching Difference

When someone says *"I'm supposed to lead AI adoption, but leadership keeps making AI decisions without me — should I ask to be included?"*

**A knowledge base says:**
> "Here are five strategies for influencing without authority: build relationships before you need them, frame your asks in terms of their priorities, find allies who can advocate on your behalf..."

**Amund says:**
> "Before we talk about asking to be included — your role isn't yet part of the decision system. What decision was made, and what part of it should your role have influenced?"

That distinction is the whole design. Amund finds what's actually happening before it offers anything.

---

## What Amund Does

**Five coaching modes** — Amund reads the situation and responds in the right mode: Untangle, Pressure-Test, Decide, Translate, Accountability. You can also call one directly when you know what you need.

**Run the Board** — Multi-voice pressure testing. Before you take something to leadership, Amund runs it past three distinct perspectives: the skeptical stakeholder, the peer who's been burned, and your future self. Each voice has a different agenda. Together they surface what a single coach wouldn't.

**Memory across sessions** — Amund tracks your working theory, commitments, decisions (with rationale), and recurring tensions. It writes to your memory files directly at session end — no copy-pasting. Context builds over time instead of resetting.

**Shareable artifacts** — Sessions produce structured outputs you can hand over: thinking summaries, position briefs, stakeholder framings, week closes. Generated silently and saved to `artifacts/outputs/`.


*Curious about the design decisions behind Amund? See `DESIGN_NOTES.md`.*

---

## Setup (Do This Once)

**1. Open the folder in Claude Code or, even better, VS Code with Claude Code**

Open the `amund/` folder as your workspace. Claude Code will automatically load `CLAUDE.md` at the start of each session, which tells it to read the core files.

**2. Fill in `memory/context.md`**

Open `memory/context.md` and fill it in — or skip this and let Amund interview you during your first session and write it for you.

**3. Choose your coaching style in `memory/context.md`**

Select Guide or Challenger. If you skip it, Amund defaults to Challenger — direct, unsentimental, action-oriented.

**3. Leave the other memory/ files empty**

They start empty. Amund populates them over time and can write to them directly at the end of sessions with your permission.

---

## How to Use It

### Starting a Session

Just talk. You don't need to pick a mode or explain the coaching structure. Describe what's happening, what you're stuck on, or what you're preparing for. The coach will orient and name what mode it's using.

You can also direct it:
> "I want to Pressure-Test something before I take it to leadership."

> "I need to Untangle — I'm overwhelmed and don't know where to start."

> "Accountability check — did I do what I said I'd do last week?"

Not sure where to start? Try one of these:

> "I have an interview for a first-of-kind AI role. Help me identify the stories that prove I can build in ambiguity."

> "I need to make my work visible to leadership without sounding like I'm pitching too hard."

> "I'm stuck between two paths and I need help making the call."

### During a Session

The coach will ask before it advises. It will name what it's noticing. It may say something uncomfortable. That's working as designed.

If it starts to sound like it's lecturing instead of coaching, tell it: *"Stop advising. Ask me a question."*

### Ending a Session

At the end of any meaningful session, Amund will ask if you want it to update your memory files directly. Say yes and it handles it — no copy-pasting required. It reads each file first and updates only what changed.

---

## The Memory System

| File | What it holds | How often it updates |
|------|--------------|---------------------|
| `memory/context.md` | Who you are — role, org, coaching preferences | Once at onboarding; rarely after |
| `memory/role_context.md` | Stable facts about how your role is positioned | When something structural changes |
| `memory/working_theory.md` | Your current theory of how to succeed in this role | When your understanding shifts |
| `memory/commitments.md` | What you said you'd do, and by when | Most sessions |
| `memory/decisions.md` | Significant calls made, with rationale | When a real direction is chosen |
| `memory/tensions.md` | Recurring patterns Amund has noticed | When a pattern surfaces more than once |

See `memory/PROTOCOL.md` for how file writing works.

---

## File Structure

```
amund/
├── CLAUDE.md              ← Entry point for Claude Code
├── README.md              ← You're reading it
├── DESIGN_NOTES.md        ← Supplemental notes on design decisions behind Amund
├── identity.md            ← Who Amund is
├── rules.md               ← How Amund coaches
├── board.md               ← Board mode — loaded on demand
├── examples.md            ← What good coaching looks like
├── memory/
│   ├── PROTOCOL.md        ← Writing rules for all memory files
│   ├── context.md         ← About you — fill this in or let Amund do it
│   ├── role_context.md    ← Your role's structural facts
│   ├── working_theory.md  ← Your current theory of the role
│   ├── commitments.md     ← What you said you'd do
│   ├── decisions.md       ← Significant calls made, with rationale
│   └── tensions.md        ← Recurring patterns
├── artifacts/
│   ├── PROTOCOL.md        ← Writing rules for artifacts
│   ├── templates/         ← Format references Amund uses when generating
│   └── outputs/           ← Your generated artifacts live here
└── reference/
    ├── influence_without_mandate.md
    ├── making_work_visible.md
    ├── ai_org_patterns.md
    ├── pioneer_role_playbook.md
    ├── energy_and_motivation.md
    ├── managing_up.md
    ├── saying_no.md
    ├── building_credibility.md
    ├── career_navigation.md
    └── opportunity_navigation.md
```

---

## What This Coach Is Not

- It won't give you a list of best practices when you share a problem
- It won't tell you what to do before it understands what's happening
- It won't let you leave a session without a next action
- It won't pretend your ambiguity is temporary

If you want information, search the web. If you want someone to think with you and push back, use this.

---

## Who Built This and Why

Built by an AI Learning Systems Designer who created their own role, wrote their own job description, fought for their own comp, and spent a year figuring out how to operate in a space with no roadmap.

This coach exists because the coaching that would have helped most in that situation didn't exist. It's built for the people navigating the same terrain.
