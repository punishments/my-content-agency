# Content Pipeline

10-step process from raw idea to published and reported content. Every piece of content follows this sequence. No steps are skipped. Process consistency is how quality stays consistent.

---

## Pipeline Overview

```
Step 1  → Idea Generation
Step 2  → Creative Strategist       [angle(s)]
Step 3  → Content Strategist        [mission + format + intensity]
Step 4  → Content Producer          [story structure + hooks]
Step 5  → Creative Director         [reviews all input, final recommendation]
Step 6  → USER APPROVAL             ← HARD GATE — no scripting before this
Step 7  → Copywriter                [final copy + production notes]
Step 8  → QA Editor                 [quality review + sign-off]
Step 9  → Final Deliverable         [approved script ready to produce]
Step 10 → Marketing Director        [post-publish reporting and tracking]
          ↓
        PUBLISH
```

> **Process note:** The team follows this pipeline on every piece of content — not because it slows things down, but because skipping steps is how quality breaks. A piece that bypasses the proposal stage or gets scripted before approval is not a fast win. It is a process failure that compounds.

---

## Step 1 — Idea Generation

**Owner:** You (the creator)
**Input:** Experience, struggle, learning, observation, or 7x7 research insight
**Tool:** `docs/weekly_idea_session.md` (full Monday SOP) + `docs/content_decision_system.md` (extraction questions)

What happens:
- Run the full Monday idea session (`docs/weekly_idea_session.md`) — triage, balance check, slot assignment
- Use `docs/content_decision_system.md` for extraction questions and brand check
- Check `planning/content_backlog.md` for carryover ideas before generating new ones
- Capture each raw idea in one sentence and log to `inputs/idea_dump.md`
- Confirm weekly balance across all 6 slots before any proposals begin

**Output:** 6 slot-assigned ideas with confirmed weekly distribution balance
**Triggers:** Step 2 (run for each idea, in sequence — constrained slots first)

---

## Step 2 — Creative Strategist

**Owner:** Creative Strategist (`agents/creative_strategist.md`)
**Input:** Raw idea from Step 1
**Reference:** `docs/creator_vision.md`, `docs/audience.md`

What happens:
- Checks brand fit — does this connect to a belief, pillar, or audience pain?
- Generates 1–2 creative angles, each with a specific and differentiated point of view
- Recommends one angle with a one-sentence justification
- Applies anti-generic filter: could this belong to any creator? If yes, push deeper.

**Output:** 1–2 creative angles + recommended angle
**Triggers:** Step 3

---

## Step 3 — Content Strategist

**Owner:** Content Strategist (`agents/content_strategist.md`)
**Input:** Recommended angle from Step 2
**Reference:** `planning/weekly_plan.md` (current week distribution)

What happens:
- Reads current week's distribution before making any assignment
- Assigns mission: Attract / Nurture / Position (Convert feed post target = 0 at current stage)
- Assigns format: Talking or Non-talking
- Assigns format type: Talking head / Voiceover / B-roll + text / Silent film
- Assigns intensity: High or Low
- Confirms assignment does not break weekly balance
- Flags any compliance issue before proceeding

**Output:** Mission + format + format type + intensity + cadence check
**Triggers:** Step 4

---

## Step 4 — Content Producer

**Owner:** Content Producer (`agents/content_producer.md`)
**Input:** Creative angle + mission + format + intensity from Steps 2–3
**Reference:** `docs/script_hooks.md`

What happens:
- Builds Problem → Pursue → Payoff story structure — specific, grounded, brand-voice checked
- Generates hooks:
  - 1–2 Framework hooks (Self-Recognition or Reframe)
  - 2–3 Adaptive hooks (POV, Internal Voice, or context-specific)
- Adapts structure and hooks to assigned format (talking vs. non-talking)

**Output:** Story structure (3 sections) + hook set (3–5 total)
**Triggers:** Step 5

---

## Step 5 — Creative Director

**Owner:** Creative Director (`agents/creative_director.md`)
**Input:** All outputs from Steps 2–4

What happens:
- Verifies cadence compliance first — non-compliant = return to Step 3 before any creative review
- Reviews both creative angles, confirms or overrides recommended angle with justification
- Evaluates each section of the story structure — flags the weakest
- Selects primary hook and backup hook with reasoning
- Identifies risks and opportunities specific to this content
- Produces a single, justified final recommendation
- Sets status: READY FOR USER APPROVAL

**Output:** Complete proposal saved to `planning/proposals/[YYYY-MM-DD]_[slug]_proposal.md` + `planning/weekly_signoff.md` row populated
**Triggers:** Step 6

**Rule:** The Creative Director does not approve content with a cadence violation or a broken story structure. Both must be resolved before the proposal reaches the user.

---

## Step 6 — User Approval ← HARD GATE

**Owner:** You (the creator)
**Input:** `planning/weekly_signoff.md` (summary view) + `planning/proposals/[slug]_proposal.md` (full detail)

What happens:
- Open `planning/weekly_signoff.md` — review all 6 proposals as a set
- Open individual proposal files for full detail when needed
- For each proposal, select one of three responses:
  - **APPROVED** → proceed to Step 7
  - **REVISION REQUESTED** → specify which section to return to and what to change
  - **REJECTED** → idea does not proceed; reason noted in sign-off sheet
- Mark decision on each row in the sign-off sheet before any scripting begins

**Rule:** No scripting begins before explicit approval is logged in `planning/weekly_signoff.md`. This gate exists because the script must be built on a direction you have consciously chosen — not one that was assumed.

**Triggers:** Step 7 (only after approval is confirmed for each post individually)

---

## Step 7 — Copywriter

**Owner:** Copywriter (`agents/copywriter.md`)
**Input:** Approved direction from Step 6
**Reference:** `docs/scripting_prompt.md` (mandatory for Talking content — no exceptions)

What happens:
- Adapts output entirely to the assigned execution mode (Talking or Non-Talking)
- **Talking:** Writes full script (Hook → Problem → Pursue → Payoff → CTA) using the mandatory scripting prompt. Includes on-screen text cues, B-roll direction, and delivery notes.
- **Non-Talking:** Writes hook (text overlay), on-screen text (3–5 lines max), and optional caption. Does not generate a full script.
- Produces an asset brief as part of production notes: specific B-roll shots needed, text overlay copy, music direction (if applicable), and any props or locations required
- Saves draft to `/scripts/[YYYY-MM-DD]_[slug].md`

**Output:** Production-ready copy + production notes (includes asset brief)
**Triggers:** Step 8

**Rule:** The Copywriter does not deviate from the approved angle, story direction, or hook. Copy is execution — not re-creation.

---

## Step 8 — QA Editor

**Owner:** QA Editor (`agents/qa_editor.md`)
**Input:** Draft script from Step 7
**Reference:** `docs/content_checklist.md`

What happens:
- Runs all three checklist layers: Universal / Format-specific / Voice and brand
- Applies the 3-question final pass (self-recognition / story clarity / format clarity)
- Makes minor and moderate revisions in place
- Returns major structural failures to the Scriptwriter with specific notes
- Issues QA sign-off when all checks pass

**Output:** Reviewed, approved script + QA revision notes
**Triggers:** Step 9

**Rule:** Nothing is marked as ready to produce without QA sign-off. A script that fails is revised — not rushed.

---

## Step 9 — Final Deliverable

**Owner:** Copywriter (saves) / QA Editor (confirms)
**Input:** QA-approved script

What happens:
- Final script is confirmed saved to `/scripts/[YYYY-MM-DD]_[slug].md`
- `planning/weekly_plan.md` is updated: script status marked complete
- Analytics stub created at `/analytics/raw/[YYYY-MM-DD]_[slug].md` using `analytics/raw/analytics_stub_template.md`
- Content is ready to produce and publish

**Output:** Production-ready, QA-approved script filed and tracked
**Triggers:** Production and publishing

---

## Step 10 — Marketing Director (Post-Publish)

**Owner:** Marketing Director (`agents/marketing_director.md`)
**Input:** Published post performance data
**Reference:** `/analytics/raw/`, `/analytics/processed/account_baseline.md`, `planning/weekly_performance.md`

What happens:
- Reads raw performance data from `/analytics/raw/` at 48 hours and 7 days post-publish
- Updates `account_baseline.md` with the week's performance totals
- Updates `weekly_performance.md` with distribution actuals vs. targets and execution review
- Flags any distribution imbalances or pipeline violations for the following week
- Does NOT derive creative or strategic conclusions from post data

**Output:** Updated baseline and performance logs
**Triggers:** Next week's planning cycle

**Rule:** Account data is operational. It records what happened. It does not define what to do next. Strategic direction comes from 7x7 research and defined frameworks.

---

## Pipeline Rules

| Rule | Consequence of violation |
|------|--------------------------|
| No script before Step 6 approval | Script is discarded; restart from Step 6 |
| No publish without Step 8 QA sign-off | Post held until QA completes |
| No cadence violation approved | Assignment returned to Content Strategist |
| No steps skipped | Step must complete before pipeline advances |
| No generic content approved | Creative Director returns to Creative Strategist |
| No strategic conclusions from account data | Marketing Director uses data for operations only |

---

## Timing Reference

| Stage | Target |
|-------|--------|
| Steps 1–5 (proposal) | Same session or within 24 hours |
| Step 6 (user approval) | Same day as proposal |
| Step 7 (scripting) | Within 24 hours of approval |
| Step 8 (QA) | Within 24 hours of script |
| Steps 9–10 (deliver + log) | Same day as publish |
