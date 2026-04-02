# Content OS

Personal brand content operation. All content must reflect `docs/creator_vision.md`. No shortcuts.

---

## Non-Negotiables

1. No copy before user approval — hard gate, no exceptions.
2. No publish without QA sign-off.
3. No cadence violations approved — return to Strategy.
4. No generic content — if any creator could post it, push deeper.
5. No strategic conclusions from account data.
6. Voice: grounded, honest, calm. No hype. See `docs/voice_rules.md`.

---

## Runtime Pack

Load these files for every content cycle. Load all other files only when a pipeline step requires them.

| File | Purpose |
|------|---------|
| `docs/creator_vision.md` | Brand foundation — beliefs, pillars, story framework |
| `docs/audience.md` | Audience pain and desired transformation |
| `docs/execution_system.md` | Cadence, formats, distribution rules — canonical source |
| `docs/scripting_prompt.md` | Mandatory for all Talking copy |

Do not preload the full `/docs/` directory.

---

## Pipeline

```
Step 1  Idea         Log to inputs/idea_dump.md
Step 2  Strategy     agents/strategy.md    → angle + mission + format + intensity
Step 3  Concept      agents/concept.md     → story structure + 2 hooks + recommendation
──────────────────────────────────────────────────────────
Step 4  USER APPROVAL  ← HARD GATE  (planning/weekly_control.md)
──────────────────────────────────────────────────────────
Step 5  Copywriter   agents/copywriter.md  → final copy (after approval only)
Step 6  QA Editor    agents/qa_editor.md   → quality review + sign-off
Step 7  Deliver      Save to /scripts/ · create analytics stub · update weekly_control.md
Step 8  Analytics    agents/marketing_director.md → post-publish reporting only
```

### Proposal Format

- **Standard / low-intensity** (default): `docs/content_proposal_template_lite.md`
- **High-intensity or flagship**: `docs/content_proposal_template.md`

Save to: `planning/proposals/[YYYY-MM-DD]_[slug]_proposal.md`
Update: `planning/weekly_control.md` after each proposal

### Step 4 — Hard Gate

Stop. Present `planning/weekly_control.md`. No copy begins before decision is logged.

- **APPROVED** → Step 5
- **REVISION REQUESTED** → return to specified step
- **REJECTED** → does not proceed

---

## Roles

| Role | File | Activates |
|------|------|-----------|
| Strategy | `agents/strategy.md` | Step 2 |
| Concept | `agents/concept.md` | Step 3 |
| Copywriter | `agents/copywriter.md` | Step 5 — after approval only |
| QA Editor | `agents/qa_editor.md` | Step 6 |
| Marketing Director | `agents/marketing_director.md` | Step 8 — post-publish only |

*Reference files (original split roles): `agents/creative_strategist.md`, `agents/content_strategist.md`, `agents/content_producer.md`, `agents/creative_director.md`*

---

## Cadence

Canonical source: `docs/execution_system.md`

6/week: 4 Attract · 1 Nurture · 1 Position · 3 Talking · 3 Non-talking · 2 High · 4 Low

---

## Hooks

Proposal stage: 2 hooks — 1 framework + 1 adaptive. Concept selects primary.
Post-approval expansion if needed: up to 2 more. Reference `docs/script_hooks.md`.
Quality test (≥3 of 5): Recognition · Tension · Clarity · Specificity · Native Language.

---

## Copy Output

No reasoning unless asked. Required fields only.

- **Talking** (35–90s): 90–150 words. Hook → Problem → Pursue → Payoff → CTA.
- **Non-talking** (8–45s): 1-line hook + 3–5 on-screen lines. Under 60 words total.

---

## Weekly Cadence

Monday: run `docs/weekly_idea_session.md` + check `planning/content_backlog.md`
Confirm 6-slot distribution before opening proposals. Use `planning/weekly_control.md`.

---

## Fast Track

20–30% of content. Criteria: simple ideas, low intensity, proven concept iteration.
Process: Idea → Hook → Copy → QA → Post (same day)
