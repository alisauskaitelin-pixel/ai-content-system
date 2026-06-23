# AI content system

A weekly content operating system. It turns a week of events into a finished content calendar, full copy across six channels, run through a quality gate and an algorithm-fitness gate, then shipped into a project tool. It runs with an AI assistant (built in Claude Code), and there is a human approval gate at every step, so the system never gets ahead of the person who owns it.

I built it to run the marketing function for two products on a one-and-a-half-person team without the quality sliding. The goal was never more posts. It was to take the volume off one operator while holding the bar, so nothing ships that I would not put my name on.

> Channels here: X, Medium, Email, YouTube, Instagram, TikTok. Configurable.
> To run it yourself you supply: memory files (product facts, past performance, audience), a per-channel voice rule set, a quality threshold, and your project tool.

---

## What makes it more than a prompt

→ Memory files. Product facts, channel performance history, audience definition, a bank of evergreen filler. Read on every run, so planning starts from what is true and what has worked, not from generic knowledge.
→ A rules layer. Banned words, banned patterns, a platform contract per channel, and a golden-examples file holding every piece of copy a human has approved. Copy has to clear it.
→ A skill per channel. Each channel carries its own format contract: opener spec, structure, length, voice anchor. The right one loads before drafting for that channel.
→ A learnings loop. Every correction and every win is written back to memory, so mistakes do not repeat and approved copy becomes next week's reference. The system drifts toward its owner's taste over time, not away from it.

---

## The workflow

Every step has a defined output and a human approval gate. Steps are not skipped or combined. Complete each, show the output, wait, move on.

**1. Intake.** Listen. What is happening this week, what is launching, any constraints. Confirm back what was heard. No drafting yet.

**2. Context read.** Load the memory files silently: product facts, performance history (last period's top post and why), audience, filler bank. Confirm what is loaded.

**3. Performance review.** If last period's analytics are in, read them. Top and bottom posts, which content types worked, one recommendation for this week. Save the insight back to memory.

**4. Weekly narrative.** Place this week's events in an engagement hierarchy, which event type earns the lead. Write the week's story in two or three sentences: what it is, who it is for, what the audience should feel by Sunday. Approve before moving.

**5. Channel map.** Map every day across six channels. Which days post, what type, what feeds what. Flag reuse ("the trailer cuts into a Reel," "the article feeds a thread"). Tag each post's audience segment and whether it needs a visual. No copy yet.

**5.5. Angle pass.** Before a single word of copy, write the one angle each piece leads with. The angle is the most charged thing in it: a human truth, a tension, a withheld turn. Not the topic, not a summary. This is the gate that kills the descriptive recap, and it has to happen in planning, because by drafting time the lazy default has already won. No piece proceeds without an angle that passes.

**6. Copy draft.** Write full copy for every post, each through its channel's format contract. Apply the framing rules per platform (what is right on X is wrong on TikTok). One idea per post. Mark each post's visual need and audience segment.

**6.5. Visual briefs.** For every post that needs a visual, generate a paste-ready brief for the design tool: concept, composition, the actual brand asset paths, and an algorithm-fitness checklist.

**7. Copy check.** Run the AI-detection scorer on every piece. Anything below the human-quality threshold is revised before it is shown. The scorer is its own tool (see the copy-check gist).

**7.5. Algorithm-fitness pass.** Audit every post against current platform ranking mechanics: shape variation across the week (no two posts the same shape in a day), a cadence cap (repeated posts from one account decay within a session), and a quality pre-screen (would the platform's own quality model read this as real and high-signal, not press-release or AI-slop). Fix before shipping, not after it underperforms.

**8. Review.** A human reads, flags specific pieces with reasoning. Apply, re-score the changed items. If feedback conflicts with a rule, surface the conflict instead of silently overriding it. Save the correction pattern to memory.

**9. Approval.** Owner approves. All posts move to Ready.

**10. Build.** Write the approved calendar into the project tool: one campaign record (the week's narrative, channels, key dates, decisions) and one record per post (copy, visual brief, channel, type, segment, publish date), plus a local backup.

**11. Filler check.** Check the evergreen bank. If a channel is running low, flag it.

**12. Save learnings.** Write back everything learned this session: corrections and why, new patterns, approved copy promoted to golden examples, performance insights. This is the loop that makes next week sharper.

---

## Why it holds

→ The angle pass (5.5) beats the failure mode of every content system, which is describing what happened. It forces one charged idea per piece, in planning, where the default can still be beaten.
→ The copy-check gate (7) keeps anything below human quality off the owner's desk. The volume comes off without the bar dropping.
→ The algorithm-fitness pass (7.5) catches structural reach problems before they ship, not after.
→ The learnings loop (12) compounds. Every week the system sounds a little more like the person who owns it.
