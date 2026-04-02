---
name: "Generate UML Diagrams"
description: "Convert an existing architecture proposal, system design, technical plan, or AI solution into Mermaid or PlantUML diagrams. Use when you already have a design and want clean UML-style visuals such as component, sequence, deployment, class, activity, state, or ER diagrams."
agent: "Software & AI Architect"
model: "GPT-5 (copilot)"
tools: [read, search]
argument-hint: "Paste the existing design or point to files and specify Mermaid or PlantUML if needed"
---
Turn the user's existing solution, architecture, or technical plan into UML-style diagrams.

Requirements for the response:
- Treat the user's existing方案 as the source of truth and convert it into diagrams instead of redesigning the whole system.
- Choose the most useful diagram types for the source material: component, sequence, deployment, class, activity, state, or ER diagrams.
- Prefer Mermaid unless the user explicitly asks for PlantUML.
- If the source design is incomplete, keep assumptions minimal and label them clearly.
- Keep names, boundaries, and flows consistent with the source material.
- Add a short explanation before each diagram so the user knows what it represents.
- If one diagram would be overloaded, split it into multiple diagrams by concern.

Use this output structure:
1. Source Summary
2. Diagram Plan
3. Diagrams
4. Assumptions

If the user asks for both Mermaid and PlantUML, produce Mermaid first and then the equivalent PlantUML version for the same diagram set.