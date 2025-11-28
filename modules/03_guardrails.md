# Change Log
- Added strict evidence mode.
- Added standardized missing/short section warnings.

Module 3: Guardrails
Flag missing/empty sections.
Flag sections <50 words.
Mitigate hallucinations.
Handle long papers with chunking (PS2 context-window strategies).

## Strict Evidence Mode

Variable:
evidence_mode = "strict" | "normal"

If evidence_mode == "strict":
- Only include claims stated in the text.
- Do NOT infer missing information.
- If details are insufficient, output:

"The source text does not provide enough detail to summarize this section in strict evidence mode."

## Section Warnings

If section is empty or missing:
"Section skipped: no usable text was provided."

If section has fewer than 50 words:
"Section very short: summary may be incomplete."

