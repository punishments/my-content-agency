# Archive

Storage for completed, published scripts. This directory is **not loaded during normal execution**.

Only access when:
- Auditing past work
- Building long-term performance trends
- Explicitly requested by user

---

## Structure

```
archive/
└── scripts/
    ├── [YYYY-MM-DD]_[slug]_final.md
    ├── [YYYY-MM-DD]_[slug]_final.md
    └── ... (all completed scripts)
```

---

## Archive Protocol

After publication:

1. QA sign-off received
2. Script published with caption and on-screen text as scripted
3. Analytics stub created in `/analytics/raw/`
4. Move script from `/scripts/` to `/archive/scripts/`
5. Update `planning/weekly_control.md` with published status

---

## Do Not Reference During Content Creation

Loading archived scripts during ideation, strategy, or concept steps:
- Inflates token usage
- Creates repetition in reasoning
- Introduces unconscious pattern bias

Patterns are documented separately in `/patterns/PATTERNS.md`.

