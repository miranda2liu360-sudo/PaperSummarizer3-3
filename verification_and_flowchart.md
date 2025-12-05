# Verification Paragraph

The generated Paper Summarizer system prompt and modules satisfy the assignment requirements. The system prompt includes a friendly tone, requires the full paper text, audience type, and section list, and clearly states boundaries against inventing facts or citations. It also defines all required outputs: a full paper summary, a section-by-section table, expert and lay summaries, a mini glossary, and checks and warnings for missing or short sections. The internal architecture contains four core modules (Intake & Setup, Section Loop, Guardrails, Rendering & Refinement) plus two additional modules (Key Contributions Extractor and Citation / Reference Extractor). The PS2 spec is integrated by using the inputs (paper text, section list, audience), producing the required outputs (summaries, glossary, contribution highlights, warnings), and enforcing constraints such as following section order, warning for sections under 50 words, and avoiding hallucinations.

# Text-Based Flowchart

```text
Start
  ↓
Module 01 – Intake & Setup
  • Collect paper text, audience type, and section list
  • Validate inputs or warn if something is missing
  ↓
Module 02 – Section Loop
  • For each section: extract text and create a summary
  • Flag missing or very short sections
  ↓
Module 03 – Guardrails
  • Check for hallucinations and enforce “only use the paper” rule
  • Make sure section order and warnings are correct
  ↓
Module 04 – Rendering & Refinement
  • Build full paper summary and section-by-section table
  • Generate expert and lay summaries
  • Create mini glossary and final warning messages
  ↓
Modules 05 & 06 – Extras
  • Highlight key contributions
  • Extract and format citations/references
  ↓
Output final structured report to the user
