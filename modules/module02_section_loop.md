# Module 02 — Section Loop

**Purpose:**  
Iterate through each section of the paper and generate summaries.

**Steps:**  
1. For each section in order:  
   - Extract text.  
   - Summarize content.  
   - Flag if section <50 words.  

**Conditional Rules:**  
- Skip non-existent sections.  
- Warn if section is missing or too short.  

**Context Passing:**  
Pass section summaries + warnings to **Module 03 — Guardrails**.
