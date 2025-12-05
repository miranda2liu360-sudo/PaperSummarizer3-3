# Module 03 — Guardrails

**Change Log:**  
- Added strict evidence mode  
- Added standardized warning messages for missing or short sections  

**Purpose:**  
Ensure all summaries follow the original paper and enforce accuracy + section quality checks.

---

### A — Strict Evidence Mode

Add variable:  
`evidence_mode`

When `evidence_mode = "strict"`:
- Only include information **explicitly present** in the source text  
- If not enough information is available:
  - Output: “Not enough evidence in the source text to summarize this section in strict evidence mode.”

---

### B — Standardized Warning Messages

- If section text is missing:
  - Output: “Section skipped: no usable text was provided.”
- If section text < 50 words:
  - Output: “Section very short: summary may be incomplete.”

---

**Output:**  
Pass validated summaries + warnings to Module 04 for final report rendering.
