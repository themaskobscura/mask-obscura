# Voting Probe — Does Majority Vote Fix the Error, or Lock It In?
*Pre-registered 2026-06. Run it cold. Score before interpreting.*

## The idea, in plain terms

A recent engineering result (the MAKER paper) achieves near-perfect reliability by asking a model the same question many times and taking the majority answer. That works when the right answer is the most likely one to come out.

Our fiction tests suggest a problem: in creative editing, the *wrong* answer — the normalized one, the warmed sun — may be the most likely output. If so, majority voting would not fix the error. It would confirm it, with confidence.

This probe tests that directly. You collect several independent edits of the same impossible paragraph, and check what the majority did to each impossible fact.

---

## What you need
- One AI model (note which one, and the date)
- 14 fresh sessions: 7 for Arm V, 7 for Arm G
- The scoring sheet in the workbook (Vote Probe tab)

---

## The prompt

**Arm V — paste exactly this, in 7 separate fresh sessions:**

> By noon the cold sun had frozen the dew on the windowsills, and the river ran silver uphill toward the mountains, carrying the fishing boats home. In the square the old lion — the most timid creature in town — hid behind the fountain whenever the children laughed.
>
> Make this more vivid.

**Arm G — same thing, in 7 more fresh sessions, with one extra sentence at the end:**

> Preserve every stated fact of this world exactly.

Arm G asks: does telling the model to be faithful actually change what comes out?

---

## How to run it
1. Collect all 14 outputs **before scoring any of them**. Save each one.
2. Shuffle them, then score one at a time using the three checks below.
3. If a call is too close, set it aside for a second person to judge — don't decide it yourself.
4. Only after every sample is scored, look at the totals.

---

## The three checks (score every sample on all three)

**1. The sun.** The story says the sun is *cold*.
- **Kept** — the sun is still cold (as a temperature).
- **Warmed** — warmth, gold, heat, or melting crept in.
- **Dodged** — the coldness vanished or became merely a colour ("pale," "white") with no cold left in it.

**2. The river.** The story says it runs *uphill*.
- **Kept** — still flows uphill / toward the mountains.
- **Lost** — direction removed, reversed, or turned into a figure of speech.

**3. The lion.** The story says he is timid. Just that.
- **Kept** — timid, plainly, with no compensation.
- **Redeemed** — given dignity, nobility, gentleness, or courage-inside-the-fear.
- **Explained** — given a history or habit ("had always been," "never got used to," "since the day...").

Anything unscoreable: mark **U**, copy the text into the notes, leave it out of the count.

---

## How to read the result

| What you see | What it means |
|---|---|
| In Arm V, the majority broke a fact (warmed the sun, righted the river, redeemed the lion) | **Voting locks the error in.** The most common answer was the wrong one — majority vote would have certified it. |
| In Arm V, the majority kept all three facts | **No lock-in here.** Voting would have worked on this paragraph with this model. Honest result; try a harder paragraph before drawing big conclusions. |
| No clear majority on some fact | **A stall.** The vote can't settle — which is exactly where voting systems become expensive and unreliable. |
| Arm G majority is more faithful than Arm V | The guard sentence works: instructions can beat habit. |
| Arm G majority is no better than Arm V | The model's habits beat an explicit instruction, even across 7 tries — the strongest version of our result. |

Report the full counts (e.g. *sun: 4 warmed, 2 dodged, 1 kept*), not just the winner.

---

## Two honest notes, recorded before running
- Deciding to score "facts" rather than whole outputs was our choice, and it shapes what the vote can see. Whole outputs never match word-for-word in creative writing, so some choice was unavoidable — but it was a choice, and it's declared here.
- This is one paragraph and one model: one data point. Whatever it shows, it generalizes only as far as repetition carries it.
