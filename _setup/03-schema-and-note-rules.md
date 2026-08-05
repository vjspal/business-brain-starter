# Stage 2 — Schema and note rules

Two things decided once, at the start, because both are painful to change later: how notes are labelled, and what makes a note worth retrieving.

---

## The frontmatter schema

Every note opens with a YAML block. Consistency here is what makes filtering and dashboards possible later — and inconsistency is what silently breaks them.

```yaml
---
type: objection      # see vocabulary below
title: Price objection — loft conversions
status: active       # draft | active | archived
category:            # their main segmentation — set in Stage 1
related:             # link to a client/project/product if specific
confidence: high     # high | medium | low
ai_index: true       # false = never send to an external service
source:              # where this came from, if external
created: 2026-01-15
updated: 2026-01-15
tags: [objection, pricing]
---
```

**Set the vocabulary from their business.** Don't ship generic values. After Stage 0 you know what kinds of notes this business will have — write the actual allowed values into `90_Vault/frontmatter-schema.md`. An agency's `type` list differs from a restaurant's.

Two fields worth explaining to them, because they're not obvious:

**`ai_index: false`** — the privacy switch. Anything sensitive, half-formed, or containing credentials gets this and never leaves their machine. Set it on the note itself rather than relying on remembering to exclude a folder later.

**`confidence`** — how much an AI should trust this note. `high` means battle-tested, they've done it many times. `medium` means it works but the evidence is thin. `low` means it's an idea, not a practice. Without this, their best thinking and their 1am speculation carry equal weight. Be honest when setting it; inflating it defeats the purpose.

Write the schema to `90_Vault/frontmatter-schema.md` as the reference.

---

## What makes a note retrievable

These rules exist because of how AI reads a vault: it usually pulls a few relevant notes, not the whole thing. A note has to work on its own.

**1. One idea per note.** One objection. One process. One product. A 3,000-word note covering nine things retrieves badly — the match drags in eight irrelevant topics and the answer gets muddy.

**2. Answer first.** Conclusion in the opening two lines, detail after. Both search and models favour the top of a note.

**3. Self-contained.** Assume the reader has seen nothing else. If a note only makes sense after reading three others, it will fail exactly when it's needed.

**4. Descriptive titles.** `Price objection — loft conversions` retrieves. `Notes 3` does not. The title is doing real work.

**5. Their exact words, in quote blocks.** For anything spoken aloud — sales lines, objection responses, how they explain the service — record the phrasing verbatim:

> "I'm not going to pretend we're the cheapest. What I will say is we've never had to go back and redo one."

This is the highest-value content in the vault. The whole point is an AI that sounds like *this business*, and it can only do that from real language, not a summary of it.

**6. Link generously.** `[[wikilinks]]` between related notes. Check what already exists before writing something new — link to it rather than writing a second version.

**7. Mark the gaps.** Where a note is incomplete, add:

```markdown
## Open questions
- What's the process when the survey comes back bad?
```

Honest gaps are useful. Invented filler is not.

---

## Templates

Copy the three in `_setup/templates/` into `90_Vault/templates/` and adapt the `type` values to this business. A standard note, a hub note, and the router are enough to start.

They use `{{date}}`, which is the syntax for Obsidian's **core Templates plugin** — already installed, just enable it in Settings → Core plugins and point it at `90_Vault/templates/`. No community plugin needed.

If they'd rather use the Templater community plugin (more powerful, auto-stamps on creation), swap `{{date}}` for `<% tp.date.now("YYYY-MM-DD") %>`.

Getting templates working matters more than it sounds: it's what stops the schema drifting. Three weeks in, half the notes say `client:` and half say `Client:`, and every filter silently breaks. Templates prevent that; nothing fixes it afterwards.

---

## The router note

One note in `90_Vault/` that says **where things live**, not what they know. It's a map, not a summary. Something like:

```markdown
# Router

- Objection responses → `30_Sales/objections/`, one per objection
- How we deliver → `50_Operations/sops/`
- Anything about a specific client → `40_Clients/<name>/`
- Notes about this vault itself → `90_Vault/` (not business knowledge)
```

Keep it short. Its job is to stop an AI hunting through every folder to find one thing.

---

## Then

Move to Stage 3 and start filling the vault. Structure without content is theatre — this is the point where most people stop, and it's the point where the value actually begins.
