---
name: dumbwrite
description: Rewrites AI-sounding or overly polished text (emails, LinkedIn messages, Slack, DMs, cold outreach) so it reads like a real person typed it fast, not like a chatbot. Use this whenever the user asks to make text sound "human," "casual," "less AI," "less robotic," "more natural," asks for a "CEO"/"subtle"/"human" style rewrite, mentions tools like Sinceerly, or asks to "dumb down" or "humanize" a message. Also trigger proactively after drafting any outreach message (cold email, recruiter DM, LinkedIn note) if the user reacts that it "sounds like AI" or asks for it "shorter and more real." Produces genuinely varied, unpolished-sounding output — not just a lowercase version of the same sentence.
---

# dumbwrite

Make AI-polished text sound like a real person typed it. Three intensity levels, same idea as tools like Sinceerly — but sharper: real variety, situational typos, and no "sent from my iPhone" crutch every single time.

## The core insight

AI text is recognizable because of **uniformity**: every sentence is complete, every clause is balanced, transitions are smooth, nothing is missing. Real human typing is recognizable because of **inconsistency**: sentence length varies wildly, some thoughts trail off, punctuation is inconsistent, and there's occasionally a genuinely unnecessary word or a missing one.

Don't just lowercase things and call it human. Actually vary the writing.

## Before rewriting, always do this pass on the original text

Strip these first, regardless of level:
- Em dashes (—) → replace with a period, comma, or nothing
- "Not just X, but Y" / "It's not about X, it's about Y" constructions
- "I wanted to reach out" / "I hope this finds you well" / "I hope you're doing well"
- "delve into", "leverage", "robust", "seamless", "streamline", "unlock", "elevate"
- Triplets ("fast, reliable, and scalable") — cut to one or two, or reorder unevenly
- Perfectly parallel sentence structures back to back
- A summary/recap sentence at the end restating what was just said

## The three levels

### Subtle
Goal: still clearly professional, but a real person wrote it in one pass without much editing.

- Contractions throughout (I'm, don't, it's, that's)
- Cut ~15-20% of words — kill hedging and throat-clearing
- One sentence should be shorter than you'd naturally write it, almost clipped
- Vary sentence opener structure — don't start every sentence the same way
- At most one small, plausible slip: a missing comma, "recieve"-style typo, or a word repeated then not caught. Never more than one. Never a typo that makes it confusing.
- Keep the ask/point clearly stated — this level is for messages that still need to look competent (recruiters, clients)

### Human
Goal: reads like a normal text/DM dashed off between other things.

- Everything in Subtle, plus:
- Lowercase sentence starts are fine but don't need to be universal — inconsistency is the point
- Drop words that are grammatically "needed" but conversationally skippable ("gonna check that out" not "I am going to check that out")
- One sentence can genuinely trail off or restart mid-thought
- Contract harder: "lmk", "tbh", "ngl" are fair game if it fits the register
- Punctuation gets looser — periods optional at message end, one comma splice is fine
- Still exactly one point/ask, but it can show up mid-message instead of at the start or end

### CEO
Goal: the busiest person in the world sent this from their phone between meetings.

- All lowercase, no exceptions
- Cut to the actual information only — if a sentence isn't the ask or a fact the reader needs, delete it
- No greeting beyond a name, no sign-off beyond initials or nothing
- Sentence fragments over full sentences
- Target length: under 25 words for the whole message unless the source material genuinely can't compress that far
- Only add "sent from my iphone" if the message doesn't already sound complete without it — don't use it as a crutch on every single output. A message that already sounds terse doesn't need the excuse.

## Typo placement rules (important — this is where most humanizers overdo it)

- Real typos cluster at the **start** of messages (before someone's "warmed up" typing) or happen on **longer/less common words**, not short common ones. Never typo "the", "a", "is".
- One typo maximum per message at Subtle and Human. Zero to one at CEO — CEO messages are usually too short to need one.
- A typo should never land on the actual ask, a name, a number, or anything the reader needs to get right. Never typo something load-bearing.
- Good typo types: doubled letter (definitly), transposed letters (teh, recieve), missing apostrophe (dont, im), a word that's technically wrong but reads fine (there/their swapped only if it won't cause real confusion).
- Bad typo types: anything that would make the reader re-read the sentence to parse it, anything on a proper noun, anything that looks like a formatting error rather than a human slip.

## How to run it

1. Take the user's draft (or write one if they haven't drafted yet).
2. Run the strip pass above.
3. Ask which level if not specified — or just default to **Human** if the user only says "make it sound human" / "dumbwrite this" without specifying, since that's the middle ground.
4. Produce ONE version at the requested level. Don't dump all three unless asked — that's noisy. If the user seems to be deciding, offer to show another level rather than dumping all three unprompted.
5. Keep the actual content/ask intact. This tool changes voice, not meaning. Never drop the core ask, a name, a date, or a number while "humanizing."

## What never changes regardless of level

- The actual point of the message
- Any names, numbers, dates, links — these must survive verbatim
- Basic legibility — a human reading it once should get it immediately, no re-reading required
