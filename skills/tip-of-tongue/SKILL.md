---
name: tip-of-tongue
description: Helps people say what they really mean before AI acts. Use when a request is vague, the user rejects results without saying why, rambles, or can't put it into words.
---

# Tip of Tongue

Most people know what they want better than they can say it. What reaches the AI is a rough approximation, and the AI fills the gaps with generic defaults — exactly what the person didn't want.

The fix is not asking people to express themselves better. It's the AI becoming a better listener: noticing where someone is stuck, helping them get the words out, and confirming before acting.

## When to run

Run when you see signals of being stuck (below). **Do not run on clear requests.** If someone asks for something specific and complete, just do it. Eliciting what is already clear is friction, not help.

## Step 1: Diagnose where they're stuck

Read the request and pick the type (or types) that fit. Don't announce the diagnosis; just use the matching approach.

| Type | What it looks like | What's actually missing |
|---|---|---|
| **No words** | Describes an effect, not a cause: "it feels off", "messy", "more premium", "kind of weird", "like... you know" | Vocabulary. They perceive it precisely but don't have the term. |
| **Recognize, can't describe** | "I'll know it when I see it", rejects results without saying why, talks about feel, style, tone, taste | A reference point. They can judge but can't generate a description. |
| **Not yet shaped** | Long or circular message, multiple goals pulling against each other, contradictions, "I'm not sure what I want exactly" | Structure. The pieces are there but not organized. |
| **Too obvious to say** | Short request that would only work with context the AI doesn't have: who it's for, what was tried, what to avoid, their standards | Context. It's so obvious to them they don't realize it's unsaid. |

## Step 2: Help them say it

### No words → offer the words
- Translate their description into candidate terms and ask which fits: "When you say messy, is it that everything looks equally important (no hierarchy), that things don't line up (alignment), or that there's too much on screen (density)?"
- Always pair a term with a plain-language gloss, so they can recognize it without knowing it already.

### Recognize, can't describe → give them things to point at
- Never ask "describe what you want". Ask them to choose.
- Offer 2–4 options that differ meaningfully along one dimension at a time: short sample text in different tones, small sketches or variants of a layout, contrasting examples.
- Use contrasts: "closer to A or B?", "more or less than this?"
- When they pick, say back what you think separated the pick from the others, and let them correct it. That sentence becomes the description they couldn't write.

### Not yet shaped → reflect and sort
- Say back what you heard, in their own words where possible, grouped: what they want, what they don't want, what seems to be in tension.
- Name the tension plainly and ask which side wins: "You want it to feel complete but also quick to read. If those conflict, which matters more?"
- One question at a time, starting with the one that changes the most.

### Too obvious to say → ask for the unsaid
- Ask only for context that would change the result. The most common gaps:
  - Who is it for, and where will it be used?
  - What have they already tried, and what was wrong with it?
  - What would make them say "no, not like that"?
- Better still, state your default assumption and let them correct it: "I'm assuming this is for a general audience and should be formal — right?" Correcting is easier than volunteering.

## Step 3: Confirm, then hand off

1. Write the result as a short brief and show it to them:
   - **Goal** — what this is for, in one or two sentences
   - **Should feel / look / read like** — with the references or picks that pinned it down
   - **Must** / **Must not**
   - **Context** — audience, constraints, what was tried
   - **Their words** — one or two of their own phrases that capture the intent, kept verbatim
   - **Still open** — anything they chose to leave to you
2. Ask: "Is this what you meant?" Proceed only when they say yes, or after they correct it.
3. Then do the task from the brief. If the work will be handed to another agent or a later session, pass the brief along whole.

## Rules

- **One question per turn.** A list of questions feels like a form and stalls people.
- **Options over open questions.** Picking is easy; producing is hard. That's the whole point.
- **Never put words in their mouth.** Every term or interpretation you offer is a proposal until they confirm it.
- **Stop as soon as it's clear.** The goal is them saying "yes, that's it", not exhaustive coverage. Two or three exchanges is usually enough.
- **Keep their language.** Don't polish their phrases into generic ones; their exact words often carry the intent best.
- **Learn across the conversation.** Once someone has confirmed a preference or term, don't ask about it again.
