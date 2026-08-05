# Stage 1 — Design the structure

Now that you understand the business, design a folder structure that fits it. **Propose, then get approval. Do not create folders before they've agreed.**

## The default

Start here and adapt. This works for most businesses:

```
00_Capture/      unprocessed notes. Should trend toward empty.
10_Business/     identity: what we sell, to whom, pricing, positioning
20_Marketing/    how we get attention and leads
30_Sales/        how we convert: scripts, objections, discovery
40_<Domain>/     ← the one that changes most. See below.
50_Operations/   how work gets done: SOPs, checklists, standards
60_Systems/      tools, integrations, automations
70_Knowledge/    research, learnings, post-mortems
80_People/       team, contacts, partners, suppliers
90_Vault/        notes about this vault: schema, templates, dashboards
```

## Why numbers

They control sort order. Alphabetically you'd get Business, Capture, Knowledge, Marketing... which means nothing. Numbers let you put raw input at the top, daily work in the middle, machinery at the bottom.

Counting in tens leaves gaps — a `15_Partnerships` can be slotted in later without renaming everything and breaking links. Two digits so it still sorts correctly past 09.

## Adapting it — the part that matters

**`40_` is the business's core delivery domain, and it varies:**

| Business type | `40_` becomes | Also consider |
|---|---|---|
| Agency, consultancy, freelancer | `40_Clients` | `45_Projects` |
| Trades, home services | `40_Jobs` | `45_Suppliers`, `35_Quotes` |
| Ecommerce, product | `40_Products` | `45_Suppliers`, `55_Fulfilment` |
| Restaurant, hospitality | `40_Menu` | `45_Suppliers`, `55_Front_of_House` |
| Professional services (legal, accounting) | `40_Matters` | `45_Compliance` |
| SaaS, software | `40_Product` | `45_Support`, `55_Engineering` |
| Coaching, education | `40_Students` | `45_Curriculum` |

**Rules for adapting:**

1. **Add folders the business obviously needs.** A regulated business needs `Compliance`. A business with physical stock needs `Inventory`. If Stage 0 surfaced a whole area of work with nowhere to live, give it a folder.
2. **Drop folders they don't need.** A solo freelancer with no team and no suppliers doesn't need `80_People`. An empty folder is worse than no folder — it's a permanent open question.
3. **Rename to their language, not yours.** If they say "matters" and never "projects," the folder says `Matters`. The vault should read like their business, not like a filing system imposed on it.
4. **Check for vocabulary collisions.** This is the one people miss. If a word already means something specific in their industry, don't use it for something else. Real example: a business running Meta ads should never have a `Meta` folder for system files — it will confuse them and everyone they show it to. Ask yourself, for each folder name: *does this word already mean something else here?*
5. **Keep it under about twelve.** More folders means more decisions every time they write a note, and "where does this go?" is what kills these systems in week three.

## Subfolders

Only where a folder will clearly hold more than about fifteen notes. Common ones:

```
30_Sales/objections/
30_Sales/scripts/
40_Clients/<client-name>/
50_Operations/sops/
```

Don't pre-build empty subfolders. Add them when the parent gets crowded.

## Propose it like this

Show them the structure with a one-line reason for each folder, then ask directly:

> Here's what I'm proposing, based on what you told me. Two things to check: does anything here not match how you actually think about your business, and is anything missing that you'd have nowhere to put?

Take their corrections seriously — they know their business and you've known it for forty minutes. If they hesitate on a name, change it. This costs nothing now and is genuinely painful once there are hundreds of notes and links.

## Then

Once approved, move to Stage 2: create the folders, write `90_Vault/frontmatter-schema.md`, add templates, and write the router note.

Record the final structure and the reasoning in `90_Vault/structure.md` so the decision isn't lost.
