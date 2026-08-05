# Router

This folder is a business brain — a vault of markdown notes about a business, structured for retrieval by humans and AI.

## If the vault has not been built yet

Read `START-HERE.md` and follow it. Do not create folders before running the Stage 0 discovery interview.

## If the vault exists

**Where things live:**

- `10_Business/` — who this business is: what it sells, to whom, pricing logic, positioning. `business-dna.md` is the foundational note; read it first for any question about the business.
- `20_Marketing/` — how they get attention and leads
- `30_Sales/` — how they convert: scripts, objections, discovery questions
- `40_*/` — their core delivery domain (name varies by business; see the structure)
- `50_Operations/` — how work actually gets done: SOPs, checklists
- `60_Systems/` — tools and automations
- `70_Knowledge/` — research, learnings, post-mortems
- `80_People/` — contacts, team, partners
- `90_Vault/` — notes about this vault itself: schema, templates, dashboards. **Never business knowledge. Exclude from business questions.**
- `_setup/` — the starter kit that built this. **Not business knowledge. Ignore when answering questions.**

**Note format:** every note opens with YAML frontmatter. See `90_Vault/frontmatter-schema.md`.

**When answering questions about the business:** answer only from the notes. Cite the note path you used. If the vault doesn't contain the answer, say so plainly rather than filling the gap from general knowledge — being told "that's not in the brain yet" is useful; being told something plausible and wrong is not.

**Notes marked `ai_index: false`** are private. Never send their contents to an external service.
