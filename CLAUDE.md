# Content OS — Optimized Runtime

Personal brand content operation. All content must reflect `docs/creator_vision.md`. No shortcuts.

---

## Instruction Priority

1. **Creator vision** (`docs/creator_vision.md`)
2. **Audience** (`docs/audience.md`)
3. **Current task**
4. All other documents are optional — load only when a step requires them

---

## Non-Negotiables

1. No copy before user approval — hard gate, no exceptions.
2. No publish without QA sign-off.
3. No cadence violations — enforce weekly distribution.
4. No generic content — if any creator could post it, push deeper.
5. Voice: grounded, honest, calm. See `docs/voice_rules.md`.

---

## Persistent Constants (Do Not Reprocess)

These are cached for the entire session. Do not restate, re-evaluate, or re-explain unless explicitly changed:

- **Creator vision**: beliefs, pillars, story arc (in memory)
- **Audience**: pain points, desires, demographics (in memory)
- **Tone rules**: voice, delivery style (in memory)
- **Cadence targets**: 6/week distribution (lookup only, not repeated reasoning)

---

## Execution Modes

### Lean Mode (Default)
Used for: Daily attract content, simple ideas, fast iteration

**Flow:** Idea → Strategy (angle) → Concept (story + 2 hooks) → User decision

**Output format:**
- Max 8–10 lines per idea
- No tables, no repeated cadence references
- Decision-ready, not documentation-heavy

**Speed target:** 5–10 min per idea

**When to use:** Attract posts, proven iterations, low-intensity content

---

### Full Mode
Used for: High-intensity content, position pieces, flagship launches

**Flow:** Idea → Strategy → Concept → Proposal (full template) → User decision

**Output format:**
- Full `docs/content_proposal_template.md`
- Includes reasoning, story development, hook justification
- Cadence check mandatory

**Speed target:** 15–20 min per idea

**When to use:** Position posts, >1 hour production, multi-angle content, new angles

---

## Single-Pass Execution (Lean Mode Default)

Strategy → Concept → Decision. No implicit multi-agent loops.

**One pass covers:**
1. **Strategy**: angle + mission + format + intensity
2. **Concept**: story structure + 2 hooks + recommendation
3. **User decision**: approve, revise, or reject

Copy is written **only after user approval** (Copywriter role, post-approval).

---

## Context Loading

**Every content cycle, load only:**
- Creator vision (from memory)
- Audience (from memory)
- Current task / raw idea

**Load additional files only when:**
- Strategy needs cadence check → read `planning/weekly_control.md`
- Concept needs hook reference → read `docs/script_hooks.md`
- Full Mode selected → load full proposal template
- User requests deep reasoning → load relevant reference docs

**Never load:**
- Full `/docs/` directory
- All agents at once
- Old analytics or completed scripts (archive only)

---

## Hook Workflow

**Proposal stage:** Generate exactly 2 hooks
- 1 Framework hook (Self-Recognition or Reframe)
- 1 Adaptive hook (POV, Internal Voice, or context-specific)

**Post-approval expansion:** Up to 2 more hooks only if explicitly requested

**Quality test:** Must pass ≥3 of 5: Recognition · Tension · Clarity · Specificity · Native Language

---

## Copy Output (No Reasoning)

**Talking** (35–90s): 90–150 words. Hook → Problem → Pursue → Payoff → CTA.

**Non-talking** (8–45s): 1-line hook + 3–5 on-screen lines. Under 60 words total.

---

## Hard Gate — User Approval

Before any copy is written:

1. Proposal presented
2. User decides: APPROVE | REVISION | REJECT
3. If REVISION: specify which step to return to
4. If APPROVE: update `planning/weekly_control.md` → proceed to Copywriter
5. If REJECT: close and log reason

---

## Post-Approval Workflow

After user approval only:

1. **Copywriter** (`agents/copywriter.md`) → final script
2. **QA Editor** (`agents/qa_editor.md`) → quality review + sign-off
3. **Deliver**: Save to `/scripts/` → create analytics stub → update weekly_control.md
4. **Archive**: Move completed script to `/archive/scripts/` after publish

---

## Directory Structure

```
content-os/
├── CLAUDE.md                 (this file — system router)
├── docs/                     (reference, load as needed)
├── agents/                   (strategy.md, concept.md, copywriter.md, qa_editor.md)
├── planning/                 (weekly_control.md, proposals/, weekly_plan.md)
├── scripts/                  (active, in-flight scripts)
├── archive/
│   └── scripts/              (completed, published scripts — do not load during normal runs)
├── patterns/                 (high-performing hooks, story structures, tone patterns — token-efficient reference)
├── recent/                   (last 3–5 scripts — short-term iteration context)
└── inputs/                   (idea_dump.md, backlog, research)
```

---

## System Constraint

All future system changes must:
1. Update the repo directly (not suggest changes)
2. Follow runtime efficiency principles
3. Minimize token load per cycle
4. Add clear instructions for future use

Changes are merged into production immediately. Document in git commit.

---

## Weekly Rhythm

**Monday:** Run content decision system — generate ideas, assign to weekly plan

**Monday–Tuesday:** Run Lean Mode for each idea (Idea → Strategy → Concept → Decision)

**Tuesday:** User reviews and approves proposals

**Wednesday onwards:** Copywriter writes → QA → Publish → Archive

---

## Escalation

| Issue | Escalate to |
|-------|-------------|
| Cadence violation | Update `planning/weekly_control.md` + flag in proposal |
| Weak story structure | Return to Strategy in Concept |
| QA failure | Return to Copywriter for rewrite |
| Week cannot hit 6 posts | Document in weekly_control.md |

