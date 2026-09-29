---
name: meeting-recap
description: Turns meeting notes or a transcript into a short recap of decisions, action items with owners and due dates, and open questions, plus an optional follow-up email. Use when the user shares meeting notes, a transcript, or a recording summary, or asks to "summarize this meeting", "write up the notes", or "what are the action items".
---

# Meeting Recap

Turn messy meeting notes or a transcript into a recap people will actually read. Accuracy matters more than polish: a recap that invents an owner or a decision is worse than no recap.

## Step 1: Read the input

Accept anything: a full transcript, rough bullet points, or a mix. Note the quality honestly at the top of the recap:

- **Good**: full transcript with speaker names
- **Partial**: notes that miss parts of the meeting
- **Rough**: a few bullets from memory

Don't ask the user a list of questions first. Work with what you have, then flag gaps.

## Step 2: Group by topic

Organize by topic, not in the order things were said. If the user has the agenda, use its topics as the headings and add any topics that came up unplanned.

## Step 3: Pull out what matters

For each topic, capture:

- **What was discussed**: two or three sentences at most
- **Decisions**: what was agreed, in bold
- **Action items**: who will do what, by when
- **Open questions**: things raised but not resolved

## Step 4: Never make things up

- If an action has no clear owner, write **Owner: unassigned**. Don't guess.
- If no deadline was given, write **Due: not set**.
- If a decision sounds likely but wasn't stated clearly, write it as "Seems to have agreed X (please confirm)".
- If more than a third of the actions have no owner, put a warning at the top: "⚠ 4 of 9 actions have no owner. Agree owners before this goes out."

## Output format

```markdown
# [Meeting name]: recap
[Date] · Attendees: [names] · Notes quality: good / partial / rough

## In short
- [Most important decision]
- [Most important action]
- [Anything blocking]

## [Topic 1]
[What was discussed, 2-3 sentences.]
**Decided:** [decision]
- [ ] [Action]: [Owner], due [date]
Open: [question]

## [Topic 2]
...

## All actions by person
**[Name]**
- [ ] [Action], due [date]

**Unassigned**
- [ ] [Action]

## Next meeting
[What needs to happen before the group meets again.]
```

## Step 5: Offer a follow-up email

Offer to turn the recap into a short email to attendees: the "In short" section, then each person's actions. If an `email-voice-profile.md` exists, write it in the user's voice.

## Quality check

- [ ] Every action has an owner or says "unassigned"
- [ ] Every action has a date or says "not set"
- [ ] No decision is stated more firmly than it was made
- [ ] "In short" fits on a phone screen
- [ ] Someone who missed the meeting can tell what they need to do
