# Module 02 — Section Loop

**Change Log:**  
- Added `summary_level` variable  
- Added conditional logic for short vs. detailed summary modes  

**Purpose:**  
Iterate through each paper section and generate structured summaries based on the user’s selected detail level.

**Inputs:**  
- Section text  
- Summary level (`short` or `detailed`)

**Steps:**  
1. Extract section text.
2. If section text is missing:
   - Output: “Section skipped: no usable text was provided.”
   - Continue to the next section.
3. If section text is fewer than 50 words:
   - Output: “Section very short: summary may be incomplete.”

**Conditional Logic:**
- If `summary_level = "short"`:
  - Generate a **1–2 sentence** summary of key information.
- If `summary_level = "detailed"`:
  - Provide:
    1. A brief paragraph summary
    2. A **bullet list with 3–5 key points**

**Output:**  
Pass structured summary sections + any warning messages to Module 03.
