# Modes Quick Start

Two execution modes. Which one to use?

---

## Lean Mode (Default) ⚡

**Fast ideation.** Simple ideas, daily attract content, proven iterations.

### When to Use
- ✓ Daily attract content (recognition, relatable, shareable)
- ✓ Simple, straightforward ideas
- ✓ Iteration on proven concepts
- ✓ Low-intensity content (<1 hour production)
- ✓ When you want output in 8–10 minutes

### How to Invoke
Just run Strategy → Concept as normal. Default output is Lean.

**Outputs:**
- Strategy: ~10 lines max (angle, assignment, cadence check)
- Concept: ~12 lines max (story, 2 hooks, recommendation)

**Total time:** 8–10 min per idea  
**Token cost:** ~10–11K per idea  
**Save:** ~40% tokens vs. previous full cycle

### Prompt
```
Run Lean Mode for this idea:
[raw idea here]

Assignment: Attract | Talking | Low
```

(Strategy and Concept will handle mode selection automatically.)

---

## Full Mode 📋

**Full reasoning.** High-intensity content, position pieces, new angles.

### When to Use
- ✓ Position posts (authority, framework, POV)
- ✓ High-intensity content (>1 hour production, voiceover, multi-angle)
- ✓ Flagship launches
- ✓ Brand-new angles you're uncertain about
- ✓ User explicitly requests full proposal
- ✓ When you want complete reasoning

### How to Invoke
Specify "Full Mode" in your request to Strategy.

**Outputs:**
- Strategy: Full format (angle 1 + angle 2, all reasoning)
- Concept: Full format (story check table, hook justification)
- Proposal: Full template (`docs/content_proposal_template.md`)

**Total time:** 15–20 min per idea  
**Token cost:** ~19K per idea  
**Save:** ~20% tokens vs. previous full cycle

### Prompt
```
Run Full Mode for this idea:
[raw idea here]

This is a position post / high-intensity / new angle
```

(Strategy and Concept will expand output automatically.)

---

## Decision Matrix

| Scenario | Mode |
|----------|------|
| "Quick hook for tomorrow's attract post" | **Lean** |
| "New angle, position post, need to think it through" | **Full** |
| "Proven format, simple idea, morning post" | **Lean** |
| "Flagship launch, multi-angle voiceover" | **Full** |
| "5th post in weekly cadence, straightforward" | **Lean** |
| "First time on this topic, uncertain" | **Full** |
| "Feels simple but I want to be sure" | **Lean** (start here, ask for Full if needed) |

---

## What Changes in Each Mode

### Strategy Agent

**Lean:**
- Single angle or angle 1 only
- No angle 2 unless it fundamentally changes recommendation
- Output: ~10 lines

**Full:**
- Both angles (if applicable)
- Full context and reasoning
- Output: ~20–25 lines

### Concept Agent

**Lean:**
- Story structure (Problem / Pursue / Payoff only)
- 2 hooks (no extended explanation)
- No story strength table
- Output: ~12 lines

**Full:**
- Story structure with development notes
- 2 hooks with justification
- Story strength check table
- Weakest section identified
- Output: ~18–20 lines

### Proposal

**Lean:**
- Template: `docs/content_proposal_template_lite.md` (default)
- Max 8–10 lines per idea
- No repeated cadence references
- Decision-ready, not documentation-heavy

**Full:**
- Template: `docs/content_proposal_template.md`
- Full section breakdown
- Reasoning and justification included
- Cadence check mandatory
- Ready for approval or detailed feedback

---

## Mixed Approach (Advanced)

You can mix modes within a week:
- **Monday:** Lean Mode for all 6 ideas (fast ideation pass)
- **Tuesday:** User reviews Lean proposals
- **Tuesday PM:** Run Full Mode on 2 approved position posts for deeper reasoning before copywriting
- **Wednesday onward:** Standard workflow

This approach:
- Keeps ideation fast
- Allows deep reasoning only where needed
- Reduces redundant full passes on simple content
- Optimizes token spend per week

---

## Remember

**Lean Mode is default.** Only use Full Mode when you genuinely need deeper reasoning or complexity justifies it. Most daily content runs leaner and faster.

When in doubt: Start Lean. User can ask for Full Mode if needed.

