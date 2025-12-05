# Module 01 — Intake & Setup

**Purpose:**  
Collect inputs and prepare the summarization pipeline.

**Steps:**  
1. Accept full paper text (PDF or plain text).  
2. Accept audience type (expert or layperson).  
3. Accept or detect section list.  

**Conditional Rules:**  
- If section list is missing → auto-detect sections.  
- If paper text is missing → stop and warn user.  

**Context Passing:**  
Pass validated inputs to **Module 02 — Section Loop**
