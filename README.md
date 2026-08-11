# dumbwrite

a claude skill that takes AI-sounding text and makes it read like a person actually typed it.

not a lowercase filter. it varies sentence length, cuts the throat-clearing, and drops one plausible typo in the right place instead of sprinkling them everywhere.

## why

AI writing gives itself away by being too even. every sentence complete, every clause balanced, nothing missing. people don't type like that. dumbwrite puts the unevenness back.

## install

it's one file. no git needed.

1. open [SKILL.md](SKILL.md) and hit the download button (raw view, then save as)
2. drop it in a folder called `dumbwrite` inside your skills folder, so the path ends up:
   - mac/linux: `~/.claude/skills/dumbwrite/SKILL.md`
   - windows: `C:\Users\<you>\.claude\skills\dumbwrite\SKILL.md`
3. restart claude

that's it. claude picks it up on its own, no config to edit.

using claude on the web or the desktop app instead? zip that `dumbwrite` folder and upload it under settings, capabilities, skills.

if you'd rather clone:

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
