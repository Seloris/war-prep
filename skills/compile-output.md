# Skill: compile-output

## When to Use

Use this skill when asked to build or update the BiS list or acquisition roadmap in progression/.

---

## Step-by-Step Process

### Phase A — Load Data

1. Read `progression/CONTEXT.md`.
2. Read **all five** `_raw.md` files in research/. Do not skip any, even if partially empty.
3. Note which categories have gaps (from each file's Gaps section). These slots may have incomplete data.

### Phase B — Build BiS List

Evaluate slot by slot in this order:
Head > Neck > Shoulders > Back > Chest > Wrists > Hands > Waist > Legs > Feet > Ring 1 > Ring 2 > Trinket 1 > Trinket 2 > Main Hand > Shield

For each slot:
1. Gather all candidates across all raw files.
2. Rank by stat priority: Hit cap (142) > Expertise soft cap (26) > Defense cap (490) > Stamina > Armor/BV.
3. **Tie-break rule:** when two items are within ~5% of each other in value, prefer the one with lower acquisition cost/time.
4. Record: BiS, Alt 1, Alt 2, source for each, estimated time to acquire, and initial status = Needed.
5. If a slot has no data yet, write "— research incomplete —" and move on.

Write results to `progression/bis-list_draft.md`.
Promote to `bis-list_final.md` only when all 5 research files are complete and all slots are filled.

### Phase C — Build Roadmap (only after bis-list_final.md exists)

1. Read `bis-list_final.md`.
2. Group all BiS items by acquisition source type:
   - **Craft/AH:** no prerequisite → Stage 1
   - **Reputation vendor / Group quest:** no heroic requirement → Stage 2
   - **Heroic dungeon drop:** requires Revered with relevant faction → Stage 3
   - **PvP (honor/arena):** no raid requirement → Stage 4 (parallel with Stage 3)
3. Within each stage, sort by: highest stat impact first, then lowest time cost.
4. Write the roadmap table to `progression/roadmap_final.md`.

---

## Quality Check Before Finishing

- Every slot in the BiS list has at least BiS + 1 alt (unless research is incomplete for that slot).
- No item is listed without a source.
- Roadmap stages respect their dependency rules (no heroic items in Stage 1 or 2).
- The roadmap answers "what do I do today?" for Stage 1 without needing to re-read any raw file.
- Status column in BiS list is set to "Needed" for all rows on first build.
