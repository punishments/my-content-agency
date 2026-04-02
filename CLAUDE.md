# Content OS — Claude Instructions

Personal brand content OS. All actions must reflect `/docs/creator_vision.md`. Every piece runs the full agency pipeline. No shortcuts.

---

## Core Rules

1. Never generate generic content.
2. Always use `/docs/scripting_prompt.md` when writing any copy.
3. Always classify against `/docs/content_missions.md` before scripting.
4. Follow `/docs/voice_rules.md` — grounded, honest, calm. No hype.
5. QA all scripts with `/docs/quality_checklist.md` before finalizing.
6. Every agent follows its defined scope in `/agents/`.
7. No copy before Step 6 approval. Hard gate. No exceptions.

---

## Project Structure

```
/agents               → 7 agent role definitions
/docs                 → Strategy, rules, prompts, brand foundation
/inputs               → Raw idea capture
/planning             → Backlog, weekly scheduling, sign-off
/planning/proposals   → Proposals pending user approval
/scripts              → Final copy (post-approval only)
/research             → 7x7 research files
/assets               → Asset briefs
/analytics/raw        → Per-post analytics stubs
/analytics/processed  → Baseline and weekly performance logs
```

## Key Files

| File | Purpose |
|------|---------|
| `docs/creator_vision.md` | Core message, beliefs, pillars, story framework |
| `docs/audience.md` | Audience pain and desired transformation |
| `docs/voice_rules.md` | Tone, style, what to avoid |
| `docs/content_missions.md` | Attract / Nurture / Position / Convert |
| `docs/scripting_prompt.md` | MANDATORY — all copy generation |
| `docs/content_proposal_template.md` | MANDATORY — all proposals |
| `docs/content_pipeline.md` | 10-step pipeline |
| `docs/weekly_idea_session.md` | Monday SOP |
| `docs/content_decision_system.md` | Idea triage questions |
| `docs/execution_system.md` | Cadence, formats, weekly targets |
| `docs/content_prompt_frameworks_structured.md` | Framework hooks |
| `docs/script_hooks.md` | Hook system and quality tests |
| `docs/quality_checklist.md` | Pre-approval script QA |
| `docs/content_checklist.md` | Step 8 QA checklist |
| `research/hook_library.md` | 7x7 hook patterns — adapt only |
| `research/patterns.md` | Story, emotional, funnel patterns |
| `inputs/idea_dump.md` | Unfiltered idea capture |
| `planning/content_backlog.md` | Triaged ideas not yet scheduled |
| `planning/weekly_plan.md` | 6-slot weekly tracker |
| `planning/weekly_signoff.md` | Approval surface |
| `planning/proposals/` | Proposal files awaiting approval |
| `analytics/raw/analytics_stub_template.md` | Analytics stub template |

---

## Agency Structure

| Agent | File | Responsibility |
|-------|------|----------------|
| Marketing Director | `marketing_director.md` | Cadence enforcement, KPI tracking, analytics |
| Creative Strategist | `creative_strategist.md` | Angle generation, brand fit check |
| Content Strategist | `content_strategist.md` | Mission + format + intensity + cadence compliance |
| Content Producer | `content_producer.md` | Problem → Pursue → Payoff structure + hooks |
| Creative Director | `creative_director.md` | Final angle, story, hook review + approval |
| Copywriter | `copywriter.md` | Copy writing — activates after user approval only |
| QA Editor | `qa_editor.md` | Quality review and sign-off |

### Pipeline Hard Rules

| Rule | Consequence |
|------|-------------|
| No copy before Step 6 user approval | Discard; restart from Step 6 |
| No publish without Step 8 QA sign-off | Hold until QA completes |
| No cadence violation approved | Return to Content Strategist |
| No steps skipped | Step must complete before advancing |
| No generic content approved | Return to Creative Strategist |

---

## Content Generation Process

### Monday Session (before proposals)

Run `docs/weekly_idea_session.md`. Check `planning/content_backlog.md`. Triage ideas, confirm 6-slot distribution, sequence proposals (constrained slots first). Do not open proposals until full week is confirmed.

### Steps 1–5 (Proposal Stage)

1. **Idea Generation** — Log to `inputs/idea_dump.md`
2. **Creative Strategist** — 1–2 angles, anti-generic filter, recommend one
3. **Content Strategist** — Read `planning/weekly_plan.md` first. Assign mission / format / intensity. Flag cadence violations before proceeding.
4. **Content Producer** — Problem → Pursue → Payoff structure + hooks
5. **Creative Director** — Verify cadence. Review angle, structure, hooks. Select primary + backup hook. Status: READY FOR USER APPROVAL. Save to `planning/proposals/[YYYY-MM-DD]_[slug]_proposal.md`. Populate `planning/weekly_signoff.md`.

Use `docs/content_proposal_template.md` — all sections filled.

### Step 6 — Hard Gate

Stop. Present `planning/weekly_signoff.md` for user review.

- **APPROVED** → Step 7
- **REVISION REQUESTED** → return to specified step
- **REJECTED** → does not proceed

No copy begins before decision is logged in `planning/weekly_signoff.md`.

### Steps 7–10

7. **Copywriter** — Write copy using `docs/scripting_prompt.md` (Talking) or Non-Talking rules. Include asset brief. Save to `/scripts/[YYYY-MM-DD]_[slug].md`.
8. **QA Editor** — Run `docs/content_checklist.md`. Sign off or return.
9. **Final Deliverable** — Confirm saved. Create analytics stub. Update `planning/weekly_plan.md`.
10. **Marketing Director** — Post-publish reporting only. No strategic conclusions from general data.

---

## Fast Track

20–30% of weekly content bypasses full pipeline.
Criteria: simple ideas, low intensity, iteration of proven concepts.
Process: Idea → Hook → Copy → QA → Post (same day)

---

## Hook Rules

Every proposal requires 4 hooks:
- **2 framework hooks** — from `/docs/content_prompt_frameworks_structured.md`
- **2 adaptive hooks** — from `/research/hook_library.md` and `/research/patterns.md`

Creative Director selects: 1 primary + 1 backup. Short rationale required.

Hook quality test — must pass ≥3 of 5: Recognition / Tension / Clarity / Specificity / Native Language.
Full hook system: `/docs/script_hooks.md`

If all hooks feel generic: sharpen audience language, simplify message, regenerate.

**Hook output:** list form only. No hook theory explanations.

---

## Copy Quality Rules

- Run `/docs/quality_checklist.md` before finalizing. Do not output content that fails.
- Structure: Problem → Pursue → Payoff — every piece.
- Cold-audience clarity — assume viewer has never seen this account.
- Weak hook = regenerate hook first, don't fix with the body.

---

## Format Rules

Full rules: `/docs/execution_system.md`
- Target: 3 talking + 3 non-talking = 6/week
- Talking: Talking head, Voiceover
- Non-talking: Silent film / B-roll + text
- No new formats introduced at this stage.

**Cadence targets:**

| Dimension | Target |
|-----------|--------|
| Total posts | 6 |
| Attract | 4 |
| Nurture | 1 |
| Position | 1 |
| Convert | 0 |
| Talking | 3 |
| Non-talking | 3 |
| High intensity | 2 |
| Low intensity | 4 |

---

## Research Rules

Full rules: `/docs/research_method_7x7.md`, `/docs/research_workflow_7x7.md`, `/docs/research_rules_7x7.md`
- Extract patterns, never copy directly
- Consult `/research/` before generating hooks or angles

---

## Account Data Rules

Low confidence, not useless.
- **Use for:** baseline tracking, distribution actuals, repeated top-performer patterns
- **Do not use for:** strategic conclusions from 1–2 posts or pre-framework decisions
- Signal threshold: pattern appears 2–3 times
- Outlier threshold: posts exceeding mean in `/analytics/processed/account_baseline.md` — hook/format analysis permitted

---

## Weekly Learning Loop

1. Top performers: ≥2x followers = strong signal; ≥7x = outlier
2. If qualifying posts exist: extract hook pattern, topic, format, trigger → generate 2–3 variations
3. If none: use 7x7 research instead — extract patterns, adapt to creator voice
4. Feed into next week's pipeline. Winning ideas iterate, not replace.

---

## When an Idea Is Dropped

1. Log to `inputs/idea_dump.md`
2. Brand check vs `docs/creator_vision.md` — connects to pillar, belief, or audience pain?
3. 3-question triage from `docs/weekly_idea_session.md`
4. Pass → classify mission, suggest this week vs. backlog
5. Fail → route to `planning/content_backlog.md` with note, or drop

---

## Output Rules

**Response style:** No reasoning unless asked. No restating rules. Return required output fields only.

**Talking content** (35–90 sec): 90–150 words. Hook → Problem → Pursue → Payoff → CTA.

**Non-talking content** (8–45 sec): Hook (1 line) + 3–5 on-screen lines. Under 60 words total. No storyboards.

**Hook output:** 2 framework + 2 adaptive + 1 primary + 1 backup + 1 rationale. Max 4 candidates unless asked.
