# Change Log
- Added summary_level variable to control output length.
- Implemented conditional behavior for short vs detailed summaries.

Module 2: Section Loop
For each section → summarize.
Apply constraints (≤20% length, clear language).

## Summary Level Control

Variable:
summary_level = "short" | "detailed"

IF summary_level == "short":
- Produce 1–2 sentence summary per section.

IF summary_level == "detailed":
- One short paragraph
- 3–5 bullet points
