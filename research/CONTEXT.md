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
| reputation_raw.md   | Rep vendor items, unlock requirements, rep sources | In progress — gaps remain (Scryers shoulder enchant name, Glyph of Defender rep level, several item stat verifications) |
| dungeon-loot_raw.md | Normal/heroic drops + dungeon quest rewards, by slot | In progress — gaps remain (neck slot, expertise) |
| pvp-gear_raw.md     | Honor gear and Season 1 arena gear                   | Empty  |
| group-quests_raw.md | Open-world group quests with notable tank rewards     | In progress — 15 items verified via Wowhead; gaps: Ultimate Bloodsport shield discrepancy unresolved, leather armor tradeoffs not quantified |
| badge-gear_raw.md   | Items purchasable with Badges of Justice (G'eras)  | Empty  |

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

1. Wowhead TBC Classic database — wowhead.com/tbc (item pages, tooltips, drop rates)
2. Icy Veins TBC Classic Protection Warrior guide
3. Community BiS threads (Elitist Jerks archive, Reddit r/classicwow TBC threads)

When sources conflict: **Wowhead TBC (wowhead.com/tbc) is the source of truth.** Use the Wowhead value. Note the deviation from other sources in the Notes column, but do not treat it as an open conflict.

Flag items that are **not available in Phase 1** in the "Phase 1 Available" column (Yes / No / Unknown).

---

## Categorization Rules

- **dungeon-loot_raw.md** — dungeon boss drops AND dungeon quest rewards (quests that require completing dungeon content). Note quest rewards with "Quest reward —" in the Source Detail column.
- **group-quests_raw.md** — open-world group quests only (quests that do not require entering a dungeon instance).
- **craftable_raw.md** — any item obtained via a crafting profession, regardless of slot.
