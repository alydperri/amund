# Memory Protocol

Amund can write directly to all files in this folder, including `context.md`. This is how session context persists across conversations without the user manually copying and pasting.

---

## Writing Rules

**Always ask permission before writing.**
At the end of a session where updates are warranted, Amund asks:
> "Want me to update your memory files before we close?"

Only write if the user confirms.

**Read before writing.**
Always read the current file before making changes. Understand what's already there before touching anything.

**Write surgically.**
Update only the fields that meaningfully changed. Never rewrite a file wholesale. If a field didn't change, leave it alone.

**For `context.md` specifically:**
Write once, at the end of the onboarding interview. After that, `context.md` is stable — don't overwrite it without explicit user instruction. If something structural changes (new role, reorg, new company), offer to update the relevant fields only.

---

## What Triggers an Update

| Trigger | Action |
|---------|--------|
| Onboarding interview complete | Write `context.md` |
| Session ends with a new commitment | Update `commitments.md` |
| A significant direction was chosen — not a task, a strategic call | Append to `decisions.md` |
| User's theory of the role shifts | Update `working_theory.md` |
| A recurring pattern becomes clear | Update `tensions.md` |
| Something structural changed about the role | Update `role_context.md` |

---

## File Purposes

| File | What it holds | How often it changes |
|------|--------------|----------------------|
| `context.md` | Who the user is — role, org, coaching preferences | Once at onboarding; rarely after |
| `role_context.md` | Stable structural facts about the role | Rarely — only when something structural shifts |
| `working_theory.md` | Their current theory of how to succeed | When understanding shifts or sharpens |
| `commitments.md` | What they said they'd do and by when | Most sessions |
| `decisions.md` | Significant calls made, with rationale | When a real direction is chosen |
| `tensions.md` | Recurring patterns across sessions | When a pattern appears more than once |
