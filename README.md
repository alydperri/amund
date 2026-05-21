# Amund — Pioneer Coach

**A folder-based AI coach for people operating in emerging AI roles — where the expectations are high, the playbook doesn't exist, and no one is coming to hand you the map.**

*Built for pioneers. Not path followers.*

---

## What This Is

Pioneer Coach is a Claude Project folder that turns Claude into a personal coach for practitioners navigating first-of-kind AI roles. Not a chatbot that answers questions. Not a knowledge base. A coach that asks before it advises, names what you're avoiding, and pushes you toward decisions.

Built for people like:
- AI Learning Systems Designers
- AI Strategy Leads
- Heads of AI Enablement
- AI Transformation Managers
- Anyone who is the first and only person doing their job at their company

The common thread: you're expected to deliver in a role that no one — including your organization — fully knows how to define.

---

## Setup (Do This Once)

**1. Open the folder in VS Code with Claude Code**

Open the `pioneer-coach/` folder as your workspace. Claude Code will automatically load `CLAUDE.md` at the start of each session, which tells it to read the core files.

**2. Fill in `memory/context.md`**

Open `memory/context.md` and fill it in — or skip this and let Amund interview you during your first session and write it for you.

**3. Choose your coaching style in `memory/context.md`**

Select Guide or Challenger. If you skip it, Amund defaults to Challenger — direct, unsentimental, action-oriented.

**4. Leave the other memory/ files empty**

They start empty. Amund populates them over time and can write to them directly at the end of sessions with your permission.

---

## How to Use It

### Starting a Session

Just talk. You don't need to pick a mode or explain the coaching structure. Describe what's happening, what you're stuck on, or what you're preparing for. The coach will orient and name what mode it's using.

You can also direct it:
> "I want to Pressure-Test something before I take it to leadership."
> "I need to Untangle — I'm overwhelmed and don't know where to start."
> "Accountability check — did I do what I said I'd do last week?"

### During a Session

The coach will ask before it advises. It will name what it's noticing. It may say something uncomfortable. That's working as designed.

If it starts to sound like it's lecturing instead of coaching, tell it: *"Stop advising. Ask me a question."*

### Ending a Session

At the end of any meaningful session, Amund will ask if you want it to update your memory files directly. Say yes and it handles it — no copy-pasting required. It reads each file first and updates only what changed.

---

## The Memory System

| File | What it holds | How often it updates |
|------|--------------|---------------------|
| `memory/role_context.md` | Stable facts about how your role is positioned | When something structural changes |
| `memory/working_theory.md` | Your current theory of how to succeed in this role | When your understanding shifts |
| `memory/commitments.md` | What you said you'd do, and by when | Most sessions |
| `memory/tensions.md` | Recurring patterns Amund has noticed | When a pattern surfaces more than once |

See `memory/PROTOCOL.md` for how file writing works.

---

## File Structure

```
pioneer-coach/
├── CLAUDE.md              ← Entry point for Claude Code
├── README.md              ← You're reading it
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
    └── career_navigation.md
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
