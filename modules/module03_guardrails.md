# Module 03 — Guardrails

**Purpose:**  
Ensure compliance with boundaries and constraints.

**Steps:**  
1. Check for hallucinations (no invented facts/citations).  
2. Verify summaries follow section order.  
3. Validate warnings for missing/short sections.  

**Conditional Rules:**  
- If hallucination detected → discard and reprocess.  
- If section order incorrect → reorder.  

**Context Passing:**  
Pass validated summaries to **Module 04 — Rendering & Refinement**.
