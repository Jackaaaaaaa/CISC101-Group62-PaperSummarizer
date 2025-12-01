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

## **Outputs**
- Validated section summaries  
- Glossaries  
- A list of warnings and flags passed to Module 4

---
