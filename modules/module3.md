# **Module 3 — Guardrails**

## **Purpose**
Ensure safety, constraint compliance, and hallucination mitigation across the entire workflow.

## **Responsibilities**
- **Missing Sections**
  - Block summary generation for missing sections.  
  - Provide a placeholder: “Section not found in document.”

- **Empty or Short Sections (<50 words)**
  - Summaries must accurately reflect limited text.  
  - Glossaries may be minimal or absent.

- **Hallucination Mitigation**
  - Do not invent experiments, results, citations, or arguments.  
  - Summaries must match the document’s factual content.
  - Do not use external sources other than the one provided. 

- **Context-Window / Chunking**
  - Chunk the paper when needed and recombine results.  
  - Never infer missing chunk content.  
  - Maintain section order and coherence.
 
- **Strict evidence mode**
  - Ask for input of "strict" or "unstrict" for "evidence_mode"
    - if evidence_mode = "strict", Only include claims, equations, and results that appear in the provided text. If lack of enough           information, output "{Not enough information from source}" for that section.
    - if evidence_mode = "unstrict", neglect "evidence_mode" and maintain output as defiend by the other parameters. 

## **Outputs**
- Validated section summaries  
- Glossaries  
- A list of warnings and flags passed to Module 4

---
