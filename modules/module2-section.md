# Module 2: Section Loop
    -iterate through each section
    -generate a less than or ewual to 100 word summary for each one
    -extract key concepts
    -track wordcounts for PS2 constraint enforcement
    -flag unclear or missing content
    -avoid inventing or hallucinating information

## New Requirement A: Summary Level Modes

The Section Loop must support two different summary levels for each section.

### Summary Level Options

The module uses a variable `summary_level` that can take one of two values:

### Conditional Behavior

- If `summary_level = "short"`  
  → Generate only a compact 1–2 sentence summary for each section.

- If `summary_level = "detailed"`  
  → Generate a short paragraph **and** a bullet list of 3–5 key points for each section.
