# **Module 2 — Section Loop**

## **Purpose**
Summarize each section independently using a reliable, repeatable workflow.

## **Workflow**
Start loop for each section in order:
1. Extract section text or mark missing.
2. If present but <50 words → flag as {short}.  
3. The summarizer should support two summary levels for each section:
   - summary_level = "number of words in the section"
      - If summary_level < "300" words, generate only a compact summary.
      - If summary_level > "300" words, generate summary + bullet list.
5. Generate summary using only the section text.  
6. Generate **3–8 glossary terms** with definitions grounded in that section.  
7. Apply hallucination controls:
   - No invented claims, results, or content  
   - No invented terminology  
   - No summarizing absent content
End loop once all sections were summerized. 

## **Outputs**
For each section:
- Section summary (20–80 words)  
- Per-section glossary  
- Flags: missing / empty / short

---
