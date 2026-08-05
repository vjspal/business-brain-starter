# Business Brain — Starter Kit

Turn your business knowledge into something an AI can actually use.

Right now, every AI you talk to is a stranger. You re-explain your business, your pricing, your customers — every single time. This kit fixes that once: you write your business down in a form any AI can read, so every conversation starts with it already knowing who you are.

**This is not a template you fill in.** You clone it, hand the folder to Claude, and Claude interviews you about your business — then builds a structure that fits *your* business specifically. A roofing company, a marketing agency and a dental practice all end up with different vaults, because they should.

---

## What you need

| | |
|---|---|
| **Obsidian** | Free, no account — [obsidian.md](https://obsidian.md) |
| **Claude** | Cowork (desktop app) or Claude Code |
| **Time** | About 2 hours for a genuinely useful first version |
| **Cost** | £0 / $0. Nothing here is paid. |

No coding. No database. No API keys.

---

## How to use it

**1. Get this folder onto your computer.**

Download the ZIP from the green **Code** button above → *Download ZIP* → unzip it somewhere sensible.

Or if you use Git:

```
git clone <repo-url> business-brain
```

Put it on a normal local drive. **Not** inside Dropbox, Google Drive or OneDrive — cloud sync will fight with this later.

**2. Open it as an Obsidian vault.**

Obsidian → *Open folder as vault* → pick the folder you just unzipped.

**3. Connect the folder to Claude.**

In Cowork, connect the folder. In Claude Code, `cd` into it and start a session.

**4. Paste this:**

> Read `START-HERE.md` in this folder and follow it.

That's it. Claude takes over from there — it'll ask you about your business first, then build the vault around your answers.

---

## What you end up with

- A folder structure that matches how *your* business actually works
- A written record of what you know — offers, pricing logic, objections, processes — that you've probably never written down anywhere
- An AI that answers as your business instead of in generic advice
- Plain text files you own completely. No lock-in, no subscription, works with any AI tool now or later

---

If you want to understand *why* it's built this way before you start, read `_setup/05-how-it-works.md`. Not required — the kit works if you just follow it.

## What this is not

It won't do it for you. The value is entirely in the answers you give during the interview — the structure is just the container. Expect to talk for a couple of hours across a few sittings.

It also won't be finished. A business brain is something you add to for as long as the business exists. The goal today is a useful start, not a complete one.

---

## Where to go next

Once the vault exists and you're using it daily, the next step is connecting it to automated agents — so an AI voice agent or a follow-up system can read from it while you're asleep. That needs a vector database and a sync pipeline, and it's a separate build. This kit deliberately stops before that, because Layer 1 is where most of the value is and almost everyone who tries to do both at once finishes neither.

---

Built by [Ankit](https://rappleai.com) at Rapple AI, alongside the video that walks through it.

If you build something with this, I'd like to see it.

MIT licensed — do whatever you want with it.
