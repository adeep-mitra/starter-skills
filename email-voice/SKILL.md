---
name: email-voice
description: Learns how the user writes emails from their own sent emails, saves it as a voice profile, and drafts new emails and replies that sound like the user wrote them. Use when the user asks to write, draft, or reply to an email, or says "make it sound like me", "in my voice", or "learn how I write".
---

# Email Voice

Draft emails that sound like the user, not like an AI. The voice always comes from the user's own writing, never from a generic template.

## Step 1: Find or build the voice profile

Look for an existing `email-voice-profile.md` (ask the user where they keep it if it isn't obvious). If it exists, read it and skip to Step 3.

If there is no profile, build one:

1. Ask the user for 5 to 15 emails **they wrote themselves**. Sent emails are best. Pasting them into the chat is fine.
   - If the tool has access to the user's mailbox, offer to read their Sent folder, and only do it with their permission.
   - Ignore forwarded text, quoted replies, auto-signatures, and emails written by other people.
2. Ask for a mix if possible: to their boss, to colleagues, to clients or outsiders, and a few quick replies. People write differently to different audiences.
3. If they have fewer than 5, work with what they have and mark the profile as low confidence.

## Step 2: Extract the voice

Study the samples and note only what is actually there:

- **Openings**: how they greet ("Hi Sam," / "Hey," / no greeting) and their first line
- **Sign-offs**: exact closing words and name format ("Cheers, A" / "Thanks, Anna")
- **Length**: typical number of sentences; how short their quick replies are
- **Sentences**: short and punchy, or long and flowing
- **Formality**: contractions, slang, emoji, exclamation marks
- **Asking for things**: direct ("Can you send X by Friday?") or softened ("Would it be possible to...")
- **Saying no or pushing back**: how blunt or cushioned
- **Pet phrases**: words and phrases they reuse
- **Never does**: things absent from every sample (for example, never uses emoji, never writes more than one paragraph)
- **Spelling**: UK or US English

If the user writes very differently to different people, record each style separately instead of averaging them.

Write the profile in this format and show it to the user:

```markdown
# Email Voice Profile
Confidence: high / medium / low (based on N samples)

## Default style
- Greeting:
- Sign-off:
- Length:
- Sentences:
- Formality:
- Spelling:

## How they ask for things
## How they say no
## Phrases they use
## Things they never do

## Variations by audience
- Boss / leadership:
- Colleagues:
- Clients / outsiders:
- Quick replies:
```

Ask the user: "Does this sound like you? Anything to change?" Then offer to save it as `email-voice-profile.md` so it can be reused next time.

## Step 3: Draft the email

1. Work out who the recipient is and which audience variation applies.
2. If replying, read the whole thread and answer what was actually asked.
3. Use only facts the user gave you. Put anything unknown in brackets, for example `[date]` or `[price]`. Never invent commitments, deadlines, numbers, or promises.
4. Write in the profile's voice: same greeting, sign-off, length, and directness.
5. Offer a subject line when it's a new email.

## Step 4: Check before showing

Reread the draft and fix it if:

- It is longer than the user's usual emails of this type
- It uses phrases the user never uses. Common AI giveaways to remove unless they appear in the user's samples: "I hope this email finds you well", "I wanted to reach out", "delve", "I'd be happy to", "Please don't hesitate to", "Thank you for your patience", a stack of exclamation marks
- It sounds more formal or more cheerful than the user
- It contains a claim or commitment the user didn't give you

The test: would the recipient believe the user wrote this themselves?

## Rules

- Draft only. Never send an email on the user's behalf unless they explicitly ask.
- The voice is the user's. Never copy the style of this skill's author or anyone else.
- When the user edits a draft, notice what they changed and offer to update the profile.
