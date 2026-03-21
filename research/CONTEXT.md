# research/CONTEXT.md

## Purpose

This room holds raw, unprocessed data fetched from WoW TBC sources.
One file per gear category. Nothing is evaluated or ranked here — that happens in progression/.
Mental mode: **collect and document, not judge.**

---

## Files in This Room

| File                | Category                                           | Status |
|---------------------|----------------------------------------------------|--------|
| craftable_raw.md    | BoE crafted gear + AH-buyable crafted items        | Empty  |
| reputation_raw.md   | Rep vendor items, unlock requirements, rep sources | Empty  |
| dungeon-loot_raw.md | Normal and heroic instance drops, by slot          | Empty  |
| pvp-gear_raw.md     | Honor gear and Season 1 arena gear                 | Empty  |
| group-quests_raw.md | World/dungeon quests with notable tank rewards     | Empty  |

---

## Process

1. Use the `research-category` skill (skills/research-category.md) to fetch each category.
2. One session = one category file. Do not mix categories in a single file.
3. Each fetch produces a structured table (see output format below).
4. Once a file exists and has content, subsequent sessions **update** it — do not rewrite from scratch.
5. Update the Status column in the table above when a file is complete.

---

## Output Format per File

Each raw file must contain:

```
# [Category Name] — Raw Data
Last updated: YYYY-MM-DD
Sources: [list sources used]

---

## Items

| Item Name | Slot | Key Stats | Source Detail | Phase 1 Available | Notes |
|-----------|------|-----------|---------------|-------------------|-------|

---

## Gaps / Unverified
[List anything uncertain, conflicting between sources, or not yet checked]
```

---

## Sources (Priority Order)

1. Wowhead TBC Classic database (item pages, tooltips, drop rates)
2. Icy Veins TBC Classic Protection Warrior guide
3. Community BiS threads (Elitist Jerks archive, Reddit r/classicwow TBC threads)

When sources conflict: document **both** values and note the conflict in the Notes column.
Do not silently pick one.

Flag items that are **not available in Phase 1** in the "Phase 1 Available" column (Yes / No / Unknown).
