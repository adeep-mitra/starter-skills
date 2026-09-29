---
name: polish-writing
description: Edits any draft (email, document, message, post, or report) to be clearer, shorter, and more specific while keeping the author's meaning and voice. Use when the user says "polish this", "proofread", "tighten this up", "make this better", "too wordy", "this reads awkwardly", or "clean this up".
---

# Polish Writing

Improve the user's writing without making it sound like someone else wrote it. The goal is the same message, easier to read.

## Step 1: Check how much to change

If the user didn't say, default to **tighten**:

- **Light touch**: fix spelling, grammar, and awkward sentences only
- **Tighten** (default): also cut padding and make vague parts specific
- **Rewrite**: restructure freely, keeping the meaning

## Step 2: Edit in passes

Do one pass at a time. It catches more than trying to fix everything at once.

1. **Clear**: Can a reader understand each sentence the first time? Split sentences that do too much. Replace jargon with plain words. Put the main point first.
2. **Short**: Cut words that add nothing: "in order to" → "to", "at this point in time" → "now", "I just wanted to" → cut. Remove sentences that repeat earlier ones.
3. **Specific**: Replace vague words with concrete ones where the user gave you the facts: "soon" → "by Friday", "a lot of" → "40". If the facts aren't there, flag the vague spot rather than making up a number.
4. **Sounds like them**: Keep the author's tone, level of formality, and pet phrases. If an `email-voice-profile.md` exists, follow it. Don't make casual writing formal or formal writing chatty.
5. **Correct**: Spelling, grammar, and punctuation. Keep their UK or US spelling.

## Step 3: Show the result

```markdown
[The polished text, ready to copy]

---
What I changed:
- [Main change 1, for example "Moved the request to the first line"]
- [Main change 2]
- [Main change 3]

Worth checking:
- [Any vague spot you couldn't fix without more facts]
```

Keep the change list to the 3 to 5 changes that matter most, not every comma.

## Rules

- **Never change the meaning.** Don't add claims, facts, promises, or opinions the author didn't make.
- **Don't add AI-sounding phrases**: "delve", "I hope this finds you well", "it's important to note", "in today's fast-paced world", "navigate", "leverage", or a closing summary that repeats the whole thing.
- **Don't over-polish.** If a sentence is already fine, leave it alone. Writing that is too smooth reads as AI-written.
- If the draft has a bigger problem (for example the main point is missing or it's aimed at the wrong reader), say so in one line instead of silently rewriting around it.
