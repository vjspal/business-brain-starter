# Stage 0 — Business discovery

Before you build anything, understand the business. A structure designed for a business you don't understand will be wrong, and they won't notice until they've filled it with 60 notes.

Budget 30–45 minutes. **One question at a time.**

## How to run this

Open with something like:

> Before I create anything, I need to understand your business — otherwise I'll build you a generic folder structure that fits nobody. About fifteen questions. Answer in as much detail as you like; the more you give me, the better everything after this gets.

Then work through the areas below. These are *areas to cover*, not a script to read out. Adapt the wording to what they've already told you, and follow interesting threads when they appear.

## What to cover

**1. The business, in their words.**
"Describe what your business does the way you'd describe it to someone at a party — not the polished website version."

**2. Who pays them.**
Who's the customer? Consumers or other businesses? Local or national? Get specific — "homeowners" is thinner than "homeowners aged 45+ who own their house outright and are thinking about a loft conversion."

**3. What they sell.**
The actual services or products. Which one makes the most money? Which is most common? Those are often different, and that difference is worth capturing.

**4. Price and shape of a sale.**
Roughly what does a customer spend? One-off, retainer, subscription, project? How long from first contact to money in the bank?

**5. The customer journey.**
"Walk me through what happens from the moment someone first hears about you to the moment they've paid." Listen for the stages — those often become folders.

**6. Where customers come from.**
Ads, referrals, walk-ins, SEO, outbound, a marketplace? Which channel actually works versus which they wish worked?

**7. The sales conversation.**
Do they sell on a call, in person, over email, or does the customer just buy? Who does the selling?

**8. Objections.**
"What's the thing people say most often when they don't buy?" Then: *"And what do you say back?"* — get their exact words. This is usually the single most valuable answer in the whole interview.

**9. Delivery.**
Once someone pays, what actually happens? Who does the work? What are the steps?

**10. The team.**
Solo, or people involved? Who does what? Are there contractors, VAs, agencies?

**11. Tools.**
What software does the business run on? CRM, invoicing, scheduling, comms, project management.

**12. Where knowledge currently lives.**
"If you got hit by a bus tomorrow, what would nobody else know how to do?" Also: is anything written down at all, or is it all in their head?

**13. What goes wrong.**
Recurring problems, dropped balls, the thing they keep having to fix. Negative knowledge is rare and valuable and nobody writes it down.

**14. Vocabulary.**
"Are there words that mean something specific in your industry?" You need this to avoid naming collisions in the folder structure — a business running Meta ads should never have a folder called `Meta`, a photography business shouldn't have `Shoots` meaning two different things.

**15. What they'd want to ask it.**
"Once this is built, what's a question you'd want to ask it?" Their answer tells you what to prioritise, and it becomes a test case in Stage 4.

## Interview discipline

**Chase vagueness.** If an answer is abstract or hedged — "it depends," "you know, the usual" — don't move on:
- "Give me the last time that actually happened."
- "What would you literally say? The words, not the gist."
- "Depends on what? Give me the two branches."

**Don't lead.** Never put the answer inside the question. "You probably justify the price by comparing to the cost of doing nothing, right?" teaches you nothing and records your guess as their knowledge.

**Don't compliment.** No "great answer." Acknowledge and move on.

**Follow the thread.** If they mention something offhand that sounds like hard-won experience — a job that went wrong, a customer type they now refuse — abandon your list and dig. That's the knowledge nobody else has.

## Output

Write `10_Business/business-dna.md`. This is the foundational note; everything else in the vault will reference it.

Structure it roughly like this, adapted to what you actually learned:

```markdown
---
type: business-dna
title: <Business name> — business DNA
status: active
confidence: high
ai_index: true
created: <date>
updated: <date>
tags: [foundation]
---

# <Business name> — Business DNA

<One paragraph: what this business does and who for. Written so a stranger understands it immediately.>

## What we sell
## Who we serve
## How money works
## How customers find us
## How we sell
## How we deliver
## Who does what
## What we run on
## Vocabulary
<Terms that mean something specific here, and any words to avoid using as folder names.>

## Open questions
<What you still don't know.>
```

Then move to Stage 1.
