# How this actually works

Optional reading. Useful if you want to understand what you're building rather than just following steps — and necessary if you plan to adapt it.

## The problem

You've got access to the smartest assistant available. One catch: it wakes up every morning with total amnesia.

So every time you use it you start over. What your business does, who you sell to, what you charge, how you handle the objection you've heard four hundred times. Ten minutes of re-explaining before one useful answer. Then you try another AI tool and it's a stranger too.

That isn't an intelligence problem. It's a **memory** problem. The capability is already there; the knowledge of *your business* isn't.

A second brain is just: **writing your business down once, in a form every AI you use can read.**

Everything else is plumbing.

## Why plain markdown files

No app, no database, no subscription. Just text files in folders on your computer.

That's deliberate:

- **You own them completely.** No export, no lock-in, no company deciding to change its pricing.
- **Every AI tool can read them.** Whatever you're using in two years will read a folder of text files.
- **You can see what's happening.** When something goes wrong you open the file and look, rather than filing a support ticket.
- **Version control is free.** Point Git at the folder and you get the full history of how your thinking changed.

Obsidian sits on top of the folder to make it pleasant — links, search, a graph view. But Obsidian doesn't own anything. Delete it and every file is still there, readable in Notepad.

## Why the structure matters

You could dump everything in one folder. It would mostly work — until it doesn't.

Structure does two jobs. It tells *you* where to put a new note, so the system survives being busy. And it gives an AI a way to narrow down where to look, so it retrieves the right thing rather than something vaguely related.

The labels in the frontmatter do the same job at a finer grain. "Only look at active sales notes" is a question you can only ask if notes are labelled consistently.

## Why one idea per note

An AI reading your vault pulls a handful of relevant notes, not the whole thing.

A note covering nine topics matches on one of them and drags in the other eight. The answer comes back muddy. Split into nine notes, and it retrieves exactly the one it needs.

Same reason each note must stand alone. It'll be read on its own, without the surrounding context you had in your head when you wrote it.

## Why an interview instead of just writing it down

Two reasons.

Most business knowledge is **tacit** — you know it well enough to act on it instantly and have never put it in words. Asked "what's your sales process," you'd give a vague summary. Asked "what do you say when someone says you're too expensive," you'd reproduce it exactly, because you've said it hundreds of times. Specific questions unlock specific knowledge; general questions produce generalities.

Second, an interview captures **how you actually talk.** The value of a business brain isn't a tidy summary of your business — it's that the AI can respond in your voice, with your reasoning. That only survives if your real words go in.

## What this is not

It isn't a productivity system. It won't organise your tasks or manage your calendar.

It isn't automatic. Nothing here watches your business and updates itself — what you put in is what's there.

It isn't finished after one session. A business brain is a thing you keep adding to. Two hours gets you something genuinely useful, not something complete.

## What comes after

Once this exists and you're using it, the obvious next step is letting automated systems read from it — so an AI answering your phone at 2am can use the same knowledge you use at your desk.

That needs a different setup. A program running on a server can't browse your folders, so the notes get chopped into pieces, indexed by *meaning* rather than by keyword, and stored in a database it can query in under a second. It's a real build, and it's a separate project.

Do this part first. It's most of the value, and it's the part you'll use every day regardless of whether you ever build the rest.
