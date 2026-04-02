# Content Pipeline

8-step process from raw idea to published and reported content. Every piece follows this sequence. No steps are skipped.

*Detailed role references: `agents/creative_strategist.md`, `agents/content_strategist.md`, `agents/content_producer.md`, `agents/creative_director.md` (retained as reference for original split-role logic)*

---

## Pipeline Overview

```
Step 1  → Idea Generation
Step 2  → Strategy              [angle + mission + format + intensity]
Step 3  → Concept               [story structure + hooks + recommendation]
Step 4  → USER APPROVAL         ← HARD GATE — no scripting before this
Step 5  → Copywriter            [final copy + production notes]
Step 6  → QA Editor             [quality review + sign-off]
Step 7  → Final Deliverable     [approved script filed + analytics stub created]
Step 8  → Marketing Director    [post-publish reporting only]
          ↓
        PUBLISH
```

---

## Step 1 — Idea Generation

**Owner:** You (the creator)
**Tool:** `docs/weekly_idea_session.md` + `docs/content_decision_system.md`

- Run the Monday idea session — triage, balance check, slot assignment
- Check `planning/content_backlog.md` for carryover ideas first
- Log each raw idea in one sentence to `inputs/idea_dump.md`
- Confirm weekly balance across all 6 slots before any proposals begin

**Output:** 6 slot-assigned ideas with confirmed weekly distribution balance

---

## Step 2 — Strategy

**Owner:** Strategy (`agents/strategy.md`)
**Reference:** `docs/creator_vision.md`, `docs/audience.md`, `docs/execution_system.md`

- Checks brand fit
- Generates 1–2 creative angles, recommends one with justification
- Reads `planning/weekly_control.md` for current week distribution
- Assigns mission / format / format type / intensity
- Confirms assignment does not break weekly balance
- Flags cadence violations before proceeding

**Output:** Recommended angle + mission + format + intensity + cadence check

---

## Step 3 — Concept

**Owner:** Concept (`agents/concept.md`)
**Reference:** `docs/script_hooks.md`

- Verifies cadence compliance from Step 2 first
- Builds Problem → Pursue → Payoff story structure
- Generates 2 hooks (1 framework + 1 adaptive)
- Reviews angle, structure, and hooks
- Selects primary hook + backup with rationale
- Sets status: READY FOR USER APPROVAL
- Saves proposal to `planning/proposals/[YYYY-MM-DD]_[slug]_proposal.md`
- Updates `planning/weekly_control.md`

**Proposal format:** `docs/content_proposal_template_lite.md` (default) or `docs/content_proposal_template.md` (high-intensity / flagship)

**Output:** Complete proposal + weekly_control.md populated

---

## Step 4 — User Approval ← HARD GATE

**Owner:** You (the creator)
**Surface:** `planning/weekly_control.md`

- Review all slot summaries in weekly_control.md
- Open individual proposal files for full detail when needed
- For each slot, select one of three decisions:
  - **APPROVED** → proceed to Step 5
  - **REVISION REQUESTED** → specify step to return to and what to change
  - **REJECTED** → idea does not proceed

**Rule:** No scripting begins before explicit approval is logged in `planning/weekly_control.md`.

---

## Step 5 — Copywriter

**Owner:** Copywriter (`agents/copywriter.md`)
**Reference:** `docs/scripting_prompt.md` (mandatory for Talking — no exceptions)

- Activates ONLY after user approval confirmed
- **Talking:** full script (Hook → Problem → Pursue → Payoff → CTA) + production notes
- **Non-talking:** hook (text overlay) + 3–5 on-screen lines + optional caption
- Produces asset brief as part of production notes
- Saves draft to `/scripts/[YYYY-MM-DD]_[slug].md`

**Output:** Production-ready copy + production notes

**Rule:** Copywriter does not deviate from the approved angle, story direction, or hook.

---

## Step 6 — QA Editor

**Owner:** QA Editor (`agents/qa_editor.md`)
**Reference:** `docs/content_checklist.md`

- Runs all three checklist layers: Universal / Format-specific / Voice and brand
- Applies the 3-question final pass (self-recognition / story clarity / format clarity)
- Makes minor and moderate revisions in place
- Returns major structural failures to the Copywriter with specific notes
- Issues QA sign-off when all checks pass

**Output:** Reviewed, approved script + QA revision notes

**Rule:** Nothing is marked ready to produce without QA sign-off.

---

## Step 7 — Final Deliverable

**Owner:** Copywriter (saves) / QA Editor (confirms)

- Final script confirmed saved to `/scripts/[YYYY-MM-DD]_[slug].md`
- `planning/weekly_control.md` updated: QA and script status marked complete
- Analytics stub created at `/analytics/raw/[YYYY-MM-DD]_[slug].md` using `analytics/raw/analytics_stub_template.md`
- Content is ready to produce and publish

**Output:** Production-ready, QA-approved script filed and tracked

---

## Step 8 — Marketing Director (Post-Publish)

**Owner:** Marketing Director (`agents/marketing_director.md`)
**Reference:** `/analytics/raw/`, `/analytics/processed/account_baseline.md`, `planning/weekly_performance.md`

- Reads raw performance data at 48 hours and 7 days post-publish
- Updates `account_baseline.md` with week's performance totals
- Updates `weekly_performance.md` with distribution actuals vs. targets and execution review
- Flags distribution imbalances or pipeline violations for the following week
- Does NOT derive creative or strategic conclusions from post data

**Output:** Updated baseline and performance logs

**Rule:** Account data is operational. It records what happened. Strategy comes from 7x7 research.

---

## Pipeline Rules

| Rule | Consequence of violation |
|------|--------------------------|
| No script before Step 4 approval | Script is discarded; restart from Step 4 |
| No publish without Step 6 QA sign-off | Post held until QA completes |
| No cadence violation approved | Assignment returned to Strategy |
| No steps skipped | Step must complete before pipeline advances |
| No generic content approved | Concept returns to Strategy |
| No strategic conclusions from account data | Marketing Director uses data for operations only |

---

## Timing Reference

| Stage | Target |
|-------|--------|
| Steps 1–3 (proposal) | Same session or within 24 hours |
| Step 4 (user approval) | Same day as proposal |
| Step 5 (scripting) | Within 24 hours of approval |
| Step 6 (QA) | Within 24 hours of script |
| Steps 7–8 (deliver + log) | Same day as publish |
