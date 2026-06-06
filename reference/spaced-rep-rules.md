# Spaced-Repetition Rules

After each Feynman + Quiz, rate the learner's confidence and schedule the next review based on recall performance. The whole point of spacing is to surface forgetting *before* the exam.

## Confidence ratings

| Rating | When to assign | Next interval |
|--------|----------------|---------------|
| **Weak** | Couldn't explain key parts of the Feynman; got the quiz wrong | 1 day |
| **Hesitant** | Right but shaky; missed details on Feynman or mis-tagged distractors; quiz correct but slow | 3 days |
| **Confident (first pass)** | Clean Feynman + correct quiz + accurate distractor tagging | 7 days |
| **Confident (subsequent)** | Cleanly cleared a review | Double the previous interval: 7 → 14 → 30 → 60 → 90 days |

## Confidence is set by performance, not self-report

You — Claude — rate it based on what you observed:

- Did they recall key mechanism names cleanly? (Feynman)
- Did they pick the right letter? (Quiz)
- Did they tag distractors with precise named patterns? (Quiz bonus)

The learner does NOT get to override the rating with "I knew that, I just didn't say it." If they didn't say it, they didn't have it on tap.

## At-review-time scoring

When a concept is due for review:

- Pose 1–2 targeted MCQs (review-style — short scenario, four options)
- If they pass cleanly → **double** the interval (per Confident-subsequent)
- If they miss → drop to **Hesitant (3 days)** AND add a row to the watch list naming the specific gap
- If they completely blank → drop to **Weak (1 day)**

## Watch list

A separate list inside `learning-log.md` of specific gaps to re-drill. Examples of what belongs on it:

- "text-content-as-completion anti-pattern" (not just "Concept 1.1" — be precise)
- "parallel spawning ≠ context: fork confusion"
- "`tool_choice` values (auto / any / forced)"

Each watch-list item should:

- Name the specific gap precisely
- Reference the parent concept and which review the re-drill is scheduled for
- Be marked ✅ **CLEARED** once the learner gets it right two reviews in a row

## When a concept has been at Confident for ≥60 days

Optional: drop it from active rotation entirely. It's locked. Keep the row in the log for traceability but mark its Next Due as `archived`. If the learner ends up needing to renew the cert, archived concepts can be reactivated for a refresh round.

## Sanity floor

If you find yourself bumping the same concept down to Weak more than three times across separate reviews, the issue is the teaching, not the learner. Re-explain with a different analogy, change the example domain, or split the concept into two finer-grained pieces.