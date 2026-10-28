# tip-of-tongue

**Say what you actually mean — before the AI acts on it.**

[中文说明](README.zh.md)

Every collaboration with AI runs through language, and language is lossy. Most people know what they want far better than they can say it. What reaches the AI is a rough approximation, and the AI fills the gaps with generic defaults — exactly the thing you didn't want.

The usual advice is "write better prompts". This skill takes the opposite view: **you shouldn't have to become a better speaker. The AI should become a better listener.**

`tip-of-tongue` is an [Agent Skill](https://agentskills.io) that notices when you're stuck, helps you get the words out, and confirms with you before doing the work.

## How it works

It first figures out *why* you're stuck, because each kind of stuck needs a different kind of help:

| You're stuck because… | Sounds like | What the skill does |
|---|---|---|
| **No words** — you sense it precisely but lack the term | "it feels off", "messy", "more premium" | Offers candidate terms with plain-language glosses: *"Is it that nothing stands out (hierarchy), things don't line up (alignment), or there's too much (density)?"* |
| **Recognize, can't describe** — you'd know it if you saw it | "not that", "I'll know it when I see it" | Gives you 2–4 options to pick from and contrasts to compare, then puts your pick into words for you |
| **Not yet shaped** — the pieces are there, unorganized | long, circular, self-contradicting | Reflects back what you said, names the tension, asks which side wins |
| **Too obvious to say** — context lives only in your head | short request missing who / why / what to avoid | States its assumptions so you can correct them — correcting is easier than volunteering |

Then it writes a short brief — goal, look and feel, musts and must-nots, context, **your own words kept verbatim** — and asks *"Is this what you meant?"* Only after you say yes does it start.

Clear requests skip all of this. Asking about what's already clear is friction, not help.

## Example

> **You:** make the landing page look more premium
>
> **Without the skill:** dark background, gold accents, serif headline. (Generic "premium".)
>
> **With the skill:** "When you say premium, which is closest — (A) calm and spacious, lots of whitespace, few elements; (B) rich and crafted, deep colors, detailed imagery; (C) sharp and precise, tight grid, strong typography?"
>
> **You:** A, but not boring
>
> **AI:** "So: spacious and restrained, with one strong focal point to keep it alive. Your words: *'premium but not boring'*. Is that it?"

## Install

The skill is a single file, [`skills/tip-of-tongue/SKILL.md`](skills/tip-of-tongue/SKILL.md), in the open Agent Skills format. It works with any tool that supports skills.

**Claude Code**

```bash
git clone https://github.com/OWNER/REPO.git
cp -r REPO/skills/tip-of-tongue ~/.claude/skills/
```

Use it automatically, or call it with `/tip-of-tongue`.

**Codex CLI**

```bash
cp -r REPO/skills/tip-of-tongue ~/.codex/skills/
```

**Claude.ai (web / app)**

Download `tip-of-tongue.zip` from [Releases](../../releases), then go to **Customize → Skills → + → Upload a skill**. Uploaded skills are off by default — switch it on.

**Other tools (Cursor, Gemini CLI, …)**

```bash
npx skills add OWNER/REPO
```

## Try it

Start a new conversation and say something vague on purpose:

- "make this page look more premium"
- "write an intro for me, it needs to feel right"
- "this isn't what I wanted" (after any result)

If the skill is working, you'll get options to pick from instead of an immediate rewrite.

## Contributing

The most useful contributions are **real cases where you got stuck** — what you said, what you meant, and whether the skill got you there. Open an issue with your example.

## License

[MIT](LICENSE)
