# Module 3: Guardrails
    - identifying missing or empty sections
    - flagging very short sections (less than 50 words)
    - enforcing hallucination mitigation
        no invented citations/made up section titles
    - applying long paper chunking

# New Requirement B: Strengthened Evidence & Hallucination Guardrails

The Guardrails Module must enforce stronger transparency and stricter evidence-based behavior.

# 1. Strict Evidence Mode

mode variable: evidence_mode = "strict"

# When evidence_mode is set to "strict": 

Only include claims, equations, and results that appear in the provided text.
If it cannot find enough information, it must say so explicitly (e.g., “The source text does not provide enough detail to summarize this section in strict evidence mode.”).

# 2. Standardized Section Warning Messages

For sections that are:
- missing/empty
- too short (< 50 words)

The module must instruct the system to output a **standardized warning**, such as:

- "Section skipped: no usable text was provided.”
- "Section very short: summary may be incomplete.”

You decide the exact wording.
