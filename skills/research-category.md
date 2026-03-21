# Skill: research-category

## When to Use

Use this skill when asked to fetch, research, or populate a raw data file in research/.
One invocation = one category.

---

## Step-by-Step Process

1. **Identify the category** from the request (craftable gear, reputations, dungeon loot, PvP gear, or group quests).
2. **Read research/CONTEXT.md** if not already loaded.
3. **Consult sources in priority order:**
   - Wowhead TBC Classic (item database, drop tables, vendor listings)
   - Icy Veins TBC Classic Protection Warrior guide
   - Community BiS threads (Reddit, Elitist Jerks archive)
4. **Filter for Protection Warrior relevance.** An item is worth listing if it provides at least one of:
   - Defense rating (toward the 490 cap)
   - Stamina (any amount)
   - Hit rating (toward 142 cap)
   - Expertise rating (toward 26 soft cap)
   - Armor or Block Value (secondary priority)
   - Spell hit / threat-generating stats (secondary priority)
   Do not list pure DPS or pure healer items.
5. **Write results** into the appropriate `_raw.md` file using the exact format from research/CONTEXT.md.
6. **Handle conflicts:** If two sources give different values for the same item, record both and note the conflict in the Notes column. Never silently choose one.
7. **Flag Phase 1 availability:** Mark "Yes", "No", or "Unknown" for each item in the Phase 1 Available column. Phase-gated items (requiring later patch content) must be flagged No.
8. **Fill the Gaps section** at the bottom: list any items you could not verify, any slots with no clear data, or any source disagreements that need resolution.

---

## Quality Check Before Finishing

- Every slot relevant to the category has at least one item listed.
- No item appears in the wrong category file.
- All source conflicts are documented, not resolved arbitrarily.
- Phase 1 availability is filled for every row.
- The Gaps section exists, even if empty.
