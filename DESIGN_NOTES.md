# Amund — Design Notes

*A short design rationale for the coach.*

---

## Why this domain

The brief asked for a folder-based AI coach for a specific domain. I considered safer options first: some niche writing coach, interview coach, design critique coach, influence-without-authority coach.

They were useful, but they were not the thing I would actually reach for.

The more specific problem was the one I was already living: operating in an emerging AI role where expectations are high, the work is visible, and the playbook does not exist yet.

Amund is built for people in that kind of role: AI enablement leads, learning systems designers, transformation managers, AI strategy practitioners, and others whose job is developing faster than their organization can define it.

The domain is not “AI careers” broadly. It is the recurring judgment work of people in uncharted AI roles:

- making ambiguous work legible
- building credibility without a clear precedent
- deciding when to move without permission
- pressure-testing ideas before they reach stakeholders
- navigating visibility, ownership, and uncertainty at the same time

That specificity shaped the whole folder.

---

## The core coaching rule

The design principle behind Amund is simple:

**Ask before advise.**

That is the line between a coach and a knowledge base.

A knowledge base hears “I am stuck influencing without authority” and gives five strategies. A coach asks what happened, what the user has already tried, what they are avoiding, and where the real tension sits.

So Amund is not designed to be comprehensive first. It is designed to be situational first.

The coaching behavior is encoded across the folder:

- `rules.md` defines the coaching loop and the “ask before advise” rule.
- `examples.md` shows the difference between generic advice and coaching behavior.
- `identity.md` defines what Amund will and will not do.
- `reference/` gives it domain-specific material to draw from only when useful.
- `memory/` lets the coach build continuity across sessions without hiding what it remembers.
- `artifacts/` turns useful coaching outcomes into reusable outputs: thinking summaries, position briefs, stakeholder framings, and week-close notes.

The working mechanism became:

> Amund does not let pioneer AI work stay vague. Every session should end with a named tension, a committed next move, or a stakeholder-ready artifact.

That is the bar. If a session ends with only vague insight, Amund has not finished the job.

---

## Architecture decisions

### 1. Memory is current state, not a transcript

The first version could have treated memory as a log of everything that happened. That would have been easy, but noisy.

Instead, the memory files are organized around current state:

| File | Job |
|---|---|
| `context.md` | Stable background about the user and role |
| `role_context.md` | Structural facts about how the role sits in the organization |
| `working_theory.md` | The user’s current theory of how success works |
| `decisions.md` | Significant calls made, with rationale |
| `commitments.md` | Promised next moves |
| `tensions.md` | Recurring patterns Amund has noticed |

The goal is not to preserve every detail. The goal is to keep the coach oriented.

That means some files overwrite, some accumulate, and some mark shifts over time. The design choice was to make memory readable and portable rather than invisible and automatic.

### 2. Board mode is loaded only when needed

Amund includes a “Run the Board” mode for high-stakes ideas. It pressure-tests the user’s thinking through three perspectives:

- the skeptical stakeholder
- the peer who has been burned before
- future self

This could have lived inside `rules.md`, but that made the core rule file too heavy. Board mode is powerful, but occasional. So it lives in `board.md` and is loaded on demand.

That is a small architecture choice, but it matters. It keeps the always-loaded context focused on coaching behavior and moves heavier logic into the file that owns it.

### 3. Reference material is opinionated, not encyclopedic

The `reference/` folder is not a general library about leadership or AI. It is a set of short, specific files for the situations this coach is most likely to encounter:

- influence without mandate
- making work visible
- AI org patterns
- pioneer role playbook
- energy and motivation
- managing up
- saying no
- building credibility
- career navigation
- opportunity navigation

The point is not to make Amund sound informed. The point is to give it enough domain texture to ask better questions and recognize patterns faster.

### 4. Artifacts make invisible work visible

A lot of work in emerging AI roles happens before there is a formal deliverable. You are framing the problem, naming the risk, translating ambiguity, or preparing a stakeholder conversation.

Amund can turn a coaching session into a usable artifact when the conversation reaches that point:

- thinking summary
- position brief
- stakeholder framing
- week close

This was not added as a productivity feature. It exists because the domain requires translation. If the user has done real thinking in a session, Amund should help them carry that thinking into the room where it matters.

---

## Character and tone

Amund is named after Roald Amundsen, the polar explorer. The reference is not meant to romanticize exploration. It points to the kind of thinking the coach is meant to support: preparation, judgment, and clear decisions under uncertain conditions.

The visual character on the landing page is intentionally low-personality. It gives the coach a presence without turning it into a mascot with a fixed emotional style.

The tone system carries the personality instead:

- **Challenger** is direct, unsentimental, and action-oriented.
- **Guide** is warmer and slower, but still honest.

The key distinction is that both modes tell the truth. They just get there differently. The user can choose their preference.

That matters because people in uncharted roles often do not need more encouragement. They need useful pressure, applied at the right moment.

---

## The landing page choice

The landing page uses a simulated coaching demo rather than a live API call.
That was deliberate, and not primarily for technical reasons.

A live demo would misrepresent how Amund works. This coach is built around context that accumulates — a user profile, memory across sessions, commitments made and tracked over time. A context-free exchange with a stranger who just landed on a portfolio page is not what Amund is for. Showing that exchange would demonstrate the wrong thing.

The simulated demo shows the intended experience: what it feels like to be in a session with a coach that already knows something about you. It uses realistic exchanges, loads instantly, and doesn't fail during judging.

A constrained live demo may make sense in a future version, once there's an onboarding flow that earns the context first.

---

## Proof of concept

Amund was not only designed as an abstract coach. I used it during the build to prepare for a real interview for a frontier AI company role.

That session produced practical value:

- a clearer answer for why the company mattered to me
- a facilitation story I had not recognized as relevant until the coach surfaced it
- sharper questions for evaluating whether the role had the conditions for success
- new material that became part of `examples.md` and `reference/opportunity_navigation.md`

That test mattered because it checked the core premise: can this coach help someone in an emerging AI role think more clearly about a real, high-stakes situation?

The answer was yes, with room to refine.

---

## What I would improve next

Amund is submission-ready, but it is not finished.

The next iteration would focus on real-session refinement:

1. **Tighten the pioneer voice.** The coach should sound grounded in the domain at key moments, without turning every response into brand copy. More testing will show if I hit that balance consistently.

2. **Expand examples.** The newer reference areas, especially energy, managing up, career navigation, and opportunity navigation, need more coaching examples.

3. **Test with people who are not me.** The coach was built from lived experience, which is a strength, but it needs outside users to expose blind spots.

4. **Build the fuller character state system.** The landing page currently uses a simplified listening/responding animation. A fuller version could map visual states to listening, analyzing, and guiding. 

5. **Explore a live demo later.** A constrained API-backed demo could be useful in a future product version, but it was not the right first move for a public repo submission.

---

## What this project demonstrates

The folder is the product, but the design challenge was something more specific: build a coaching system, not a coaching prompt.

A prompt tells Claude how to respond. A system encodes judgment — what to notice, what to name, when to push, what to do with what it learns. The difference shows up in the architecture: memory designed as current state rather than transcript, reference material opinionated enough to ask better questions, artifacts that move session thinking into stakeholder contexts, and a Board mode held separately so the always-loaded files stay focused.

Whether that system holds up under real, sustained use with people who are not me is the next question. This submission is the foundation.

---

*Built by Alyshia Perri, May 2026.*
