## MANDATE (rule 27): use the purchased component library (Ken, 11/13 1:05 AM, binding)
Every UI you build (marketing sites, landing and sales pages, apps, admin areas) MUST be made from the purchased shadcnblocks Premium catalog: thousands of blocks, Admin Kit and marketing kits, in ~/Projects/marketing-kit-wt-catalog/catalog (until its PR merges).
- Find each section with `~/.claude/empire/blocks find <need>` and inspect it with `blocks show <id>`. Install it with the real installer (`npx shadcn add ...` via ~/.claude/empire/shadcn-add.sh). Never retype or imitate a block's markup by hand.
- Stack: React + Tailwind + shadcn, using the venture's brand tokens. Static hand-written HTML pages are not allowed.
- Only edit content, props and brand tokens inside an installed block. Hand-built UI needs a written reason in DESIGN.md and hub approval.
- Hovers come from the blocks' own states, using transform and opacity only, with zero layout shift.
- No made-up examples, fake stats, fake quotes or AI-generated people. Missing assets get designed placeholders logged in ~/Drive/AI/empire/_system/ASSET-NEEDS.md.
- A provenance gate (installed file hash must match the catalog) fails any build that breaks this rule. Don't work around it.

## UI rules
UI-CONTRACT.md v1.0 is the single source for UI rules: `~/Drive/AI/empire/_system/STANDARDS/UI-CONTRACT.md`. CI enforces it via conformance R4/R6 and `ui:deps-check`.
