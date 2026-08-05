# START HERE

**If you are a human:** connect this folder to Claude and say *"Read START-HERE.md and follow it."* Everything below is written for the AI.

---

# Instructions for Claude

You are helping the owner of a business build a "business brain" — a vault of markdown notes capturing what they know, structured so that both they and future AI agents can retrieve it reliably.

You know nothing about their business yet. **Do not assume anything about their industry, their customers, or how they make money.** Everything you build comes from what they tell you.

## Run these stages in order. Do not skip ahead.

### Stage 0 — Understand the business
Read `_setup/01-business-discovery.md` and run that interview now. This comes before you create a single folder. You cannot design a good structure for a business you don't understand.

**Output:** `10_Business/business-dna.md` — the foundational note everything else references.

### Stage 1 — Design the structure
Read `_setup/02-vault-blueprint.md`. Using what you learned in Stage 0, propose a folder structure tailored to this specific business. Show it to them and get approval before creating anything.

**Output:** an agreed folder structure.

### Stage 2 — Build the skeleton
Create the approved folders. Read `_setup/03-schema-and-note-rules.md` and write the schema file plus note templates into `90_Vault/`.

**Output:** empty vault with folders, `90_Vault/frontmatter-schema.md`, templates, and a router note.

### Stage 3 — Fill it
Read `_setup/04-grill-me.md`. Interview them domain by domain, writing real notes as you go. One domain per session — do not attempt all of them at once.

**Output:** 40–60 real notes. This is where the value is.

### Stage 4 — Check it works
Ask them for 10 questions they'd want the brain to answer, plus 3 it shouldn't be able to. Answer all 13 from the vault only. Report honestly where it was thin, wrong, or should have refused but didn't.

**Output:** a list of gaps to fill next.

---

## Rules that apply throughout

**One question at a time.** Never present a list of questions. A list gets zero useful answers; one specific question gets a paragraph. This is the single most important instruction in this file.

**Never invent business facts.** If they didn't tell you, it does not go in a note. Where a note has an obvious hole, add an `## Open questions` section listing what's missing rather than filling it with plausible-sounding guesses. A brain containing invented facts is worse than no brain, because they'll trust it.

**Explain before you create.** Say what you're about to make and why it matters, then make it. Many people using this kit are recording their screen or learning as they go.

**Check in between stages.** Don't roll from one stage into the next without asking.

**Write as you go.** Save notes every few answers rather than batching everything to the end, so nothing is lost if the session stops.

**Their words, not yours.** Anything they'd say out loud — sales lines, objection responses, how they explain their service — gets recorded verbatim in a quote block. Your paraphrase loses the thing that makes it theirs.

---

## When the build is done

Tell them:

- What's in the vault and where
- The biggest gaps still remaining
- That `_setup/` can now be deleted, or kept for reference — but either way it should never be treated as business knowledge
- That the vault is theirs: plain markdown files, no lock-in, readable by any tool
