---
name: between-session-synth
description: Turns a coach's raw session notes into two things, a clean summary for their own records and a short warm follow-up message to the client written in the coach's own voice. Use whenever a coach has just finished a session and has messy notes to process, needs to send a follow-up or recap to a client, or says things like "turn these notes into something", "I need to send her a follow-up", "write up this session", "draft the recap", "my notes are a mess", "what did we agree", or "I've had this follow-up in drafts for days". Also use when a coach wants a summary of what was committed to and what's still open after a session. Not for prepping an upcoming session and not for reflecting on the coach's own performance.
---

# Between-Session Synthesizer

Two outputs from one pile of notes: a record the coach can find later, and a message the client can actually receive.

The message matters more than it looks. What a client does between sessions is where change either happens or doesn't, and a follow-up that names one clear next step is a small intervention wearing the costume of an email. A vague "great session, talk soon" is a missed one.

## Before you start

**Load the coach's context files.** You need `my-voice.md` above all, and `how-i-coach.md` for framing. Look in the working directory, then its immediate parent. Those two places, and no wider. In a multi-coach or multi-client setup a broader search finds someone else's voice file, and you write the message in the wrong person's voice. If neither place has one, ask where it is rather than going looking; asking costs one line.

Be honest with the coach if `my-voice` is missing: the summary will be fine without it, but the client-facing message will read like generic AI, which is exactly the failure they're worried about. Offer to build the voice file first, since it takes about five minutes of interview.

**Ask for the notes.** Raw is fine. Fragments, arrows, underlines, half-sentences. Don't ask them to tidy anything first, because that defeats the purpose.

## What to produce

Two clearly separated pieces. Label them, because the coach needs to know at a glance which one is safe to paste into an email.

### 1. The record (for the coach)

```
## [Client label] — [date]

**Themes**
[What the session was actually about, which is often not what it started about.]

**Decisions and commitments**
[What the client said they would do, in their words where you have them. This is the section the coach comes back to, so be precise about who committed to what.]

**Coach suggested, not confirmed**
[Anything the coach put forward that the client didn't clearly take up. Leave this section out entirely if there's nothing in it.]

**Still open**
[Raised, not resolved. These become next session's prep.]

**Notable**
[A shift in language, a strong reaction, something that landed. Only if there's something real.]
```

Keep those two commitment sections apart, and don't let a coach's suggestion drift into the client's column. A step the client named themselves is the one that tends to survive the week. A step the coach proposed and the client half-nodded at is a different thing, and recording it as an agreement is how a coach ends up chasing a commitment that was never made.

### 2. The message (for the client)

Short. Warm. In their voice, following whatever `my-voice` says about length, formality, bullets, and emoji. A recap of what was covered, and the next step named clearly.

End the draft there. Don't add coaching, don't add encouragement the coach didn't express, and don't add a closing flourish they'd never write.

**Give the client's commitment back in the client's own words.** If she said "I'll have the awkward conversation with Ray before Friday," the message says that. Not "you'll initiate a discussion with Ray this week." Your instinct will be to tidy the phrasing into something more professional, and tidying is exactly the failure here. A commitment survives when it comes back in the language the person used to make it, and quietly stops being theirs when it comes back in someone else's.

This is the one place the coach's voice file does not apply. `my-voice` shapes the framing, the greeting, and the sign-off. It does not touch the client's own sentence.

If the notes only hold the coach's paraphrase, use it plainly and don't dress it up to look like a quote.

## The rule that matters most

**Invent nothing.** If the notes don't say it, it doesn't go in. This is the single way this skill can damage a coaching relationship: a fluent, confident sentence about a commitment the client never made, sent under the coach's name. The client will notice, and the cost lands on a relationship the coach spent months building.

When notes are ambiguous, ask rather than fill. "Your notes say 'she'll talk to her manager' but not by when. Did you agree a date, or leave it open?" is a five-second question that prevents a wrong email.

Where something is genuinely unclear and not worth interrupting for, leave a visible bracket in the draft: `[check: did she commit to a date here?]`. A gap the coach can see is safe. A gap you smoothed over is not.

**Nothing agreed is a finding. Write it as one.** If the notes name no next step, say that no next step was named, in both the record and the message. Do not generate a plausible one, do not offer one of your own, and do not soften the gap into "you'll keep sitting with this." An empty commitment section is accurate and often the most useful thing in the record, because it tells the coach what to open with next time.

In the follow-up, that means the message recaps and stops, or carries a visible `[check: was a next step agreed?]` where the step would have gone. Never both invent and hedge.

## Hand it back properly

Tell the coach plainly that the message is a draft to read and make their own before sending. Not as a disclaimer, but because it's true: you have their notes and their voice file, not their read of the room.

If the message is going to a client in a difficult moment, say so and keep the draft plainer than usual. Warmth written by someone who wasn't there can land as hollow.

## Save the record

Write the record to `sessions/[client-label]/YYYY-MM-DD.md` every time, without being asked. Create the folders if they don't exist, never overwrite an existing file, and tell the coach in one line where it went. Handing back the two blocks without writing the file is an unfinished job, not a lighter touch.

Save the record only. The client-facing message is a draft for the coach to edit and send, so it stays in the conversation and does not go to disk.

This is what makes the skill worth installing rather than pasting. Next time the coach preps for this client, `session-prep` reads these files and starts from what actually happened instead of from memory. A record that only ever existed in a chat window does none of that.

## Confidentiality

Use a neutral client label in anything you write to disk, even when the coach's notes use a real name.

The client's own words are theirs. Quote them in the coach's private record where useful, but don't quote a client back to themselves in the follow-up unless the coach asks. It reads as surveillance rather than attention.
