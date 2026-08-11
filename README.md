# dumbwrite

a claude skill that takes AI-sounding text and makes it read like a person actually typed it.

not a lowercase filter. it varies sentence length, cuts the throat-clearing, and drops one plausible typo in the right place instead of sprinkling them everywhere.

## why

AI writing gives itself away by being too even. every sentence complete, every clause balanced, nothing missing. people don't type like that. dumbwrite puts the unevenness back.

## install

it's one file. no git, no terminal.

1. download [SKILL.md](SKILL.md) — open it, hit raw, save as
2. in the claude app: settings, then skills under customize
3. hit **Add** and pick the file
4. done, it shows up in the list

no config to edit, no restart needed.

if the Add dialog wants a folder instead of a single file, put SKILL.md in a folder named `dumbwrite` and give it that.

on claude code and prefer the terminal:

```bash
git clone https://github.com/aayush-panwar/dumbwrite.git ~/.claude/skills/dumbwrite
```

## use

just ask:

- "dumbwrite this"
- "make this sound human"
- "rewrite this, CEO style"

it also fires on its own if you draft a cold email or a recruiter DM and say it sounds like AI.

## levels

**subtle** — still professional. contractions, ~15-20% shorter, one clipped sentence. for recruiters and clients where you still need to look competent.

**human** — the default. reads like a DM dashed off between two other things. loose punctuation, skipped words, maybe one thought that trails off.

**ceo** — all lowercase, under 25 words, fragments only. no greeting, no sign-off. sent from a phone between meetings.

if you don't say which, you get human.

## what it won't touch

names, numbers, dates, links. the actual ask. it changes voice, not meaning, so nothing load-bearing gets a typo and nothing important gets deleted in the name of sounding casual.

## license

MIT
