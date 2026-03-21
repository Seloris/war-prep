# progression/CONTEXT.md

## Purpose

This room processes research/ data into two actionable outputs: a BiS list and an
acquisition roadmap. Mental mode: **evaluate, rank, and sequence.**
Nothing is fetched here — all raw data comes from research/.

---

## Files in This Room

| File               | Purpose                                              | Status |
|--------------------|------------------------------------------------------|--------|
| bis-list_draft.md  | Working BiS list — updated as research completes     | Empty  |
| roadmap_final.md   | Staged acquisition plan, derived from BiS list       | Empty  |
| advisor_log.md     | Persistent Q&A log — decisions and rationale         | Active |

Promote `bis-list_draft.md` → `bis-list_final.md` only when all 5 research categories are complete.
Build `roadmap_final.md` only after `bis-list_final.md` exists.

---

## Process

### BiS List

1. Read **all** `_raw.md` files in research/ before building or updating.
2. Use the `compile-output` skill (skills/compile-output.md).
3. Evaluate items slot by slot. For each slot: pick Best in Slot, 1st alt, 2nd alt.
4. Record source, approximate time cost, and current status.
5. Stat priority (from CLAUDE.md): Hit cap (142) > Expertise soft cap (26) > Defense cap (490) > Stamina > Armor / BV
6. Tie-breaking rule: prefer the easier-to-acquire item over marginally better stats.

### Roadmap

Built only after `bis-list_final.md` exists. Group BiS sources into dependency-ordered stages:

| Stage | Focus | Dependency |
|-------|-------|------------|
| 1 | No-prereq crafts + AH purchases | None — do day 1 |
| 2 | Rep grinding + group quests | None — run in parallel with stage 1 |
| 3 | Heroic dungeon farming | Requires Revered with relevant factions |
| 4 | PvP gear fills | No raid needed — run in parallel with stage 3 |

---

## Output Formats

### BiS List Table (per slot group)

| Slot | Item | Source | Est. Time | Status | Alt 1 | Alt 2 |
|------|------|--------|-----------|--------|-------|-------|

**Status values:** Needed / In Progress / Done

### Roadmap Table (per stage)

| Stage | Item | Slot | Source | Est. Time | Dependency | Priority |
|-------|------|------|--------|-----------|------------|----------|

---

## Slot Evaluation Order

Head > Neck > Shoulders > Back > Chest > Wrists > Hands > Waist > Legs > Feet > Ring 1 > Ring 2 > Trinket 1 > Trinket 2 > Main Hand > Shield

---

## What Good Output Looks Like

The BiS list answers "what is best in each slot and where does it come from" at a glance.
The roadmap answers "what do I do today, tomorrow, and this week" without re-reading the raw data.
If either output requires cross-referencing to answer those questions, it is not done yet.
