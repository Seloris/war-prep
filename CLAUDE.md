# war-prep

Protection Warrior, level 68. Goal: tank-ready for TBC Anniversary Phase 1 as fast
and efficiently as possible. Collect raw gear data across 5 categories, then process
it into a ranked BiS list and a staged acquisition roadmap.

---

## Folder Structure

```
war-prep/
├── research/    — raw data fetched from WoW sources, one file per category
├── progression/ — processed outputs: BiS list and acquisition roadmap
└── skills/      — reusable instructions for recurring tasks
```

---

## Routing Table

| Task                        | Go to        | Read       | Skills              |
|-----------------------------|--------------|------------|---------------------|
| Fetch a gear category       | research/    | CONTEXT.md | research-category   |
| Update or review raw data   | research/    | CONTEXT.md | —                   |
| Build or update BiS list    | progression/ | CONTEXT.md | compile-output      |
| Build or update roadmap     | progression/ | CONTEXT.md | compile-output      |

---

## Character Reference

- Class: Protection Warrior
- Level: 68 → 70 (TBC Anniversary)
- Target: Phase 1 tank viability (threat, survivability, heroic unlock minimum)
- Stat priority: Hit cap (142 rating) > Expertise soft cap (26) > Defense cap (490) > Stamina > Armor / Block Value

---

## Naming Conventions

| Context               | Convention             | Example               |
|-----------------------|------------------------|-----------------------|
| Raw research files    | `[category]_raw.md`    | `dungeon-loot_raw.md` |
| Draft outputs         | `[output]_draft.md`    | `bis-list_draft.md`   |
| Final/locked outputs  | `[output]_final.md`    | `roadmap_final.md`    |
| Skills                | `[skill-name].md`      | `research-category.md`|

Rules: all lowercase, hyphens within descriptors, underscore before status suffix only.
