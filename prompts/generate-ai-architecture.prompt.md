---
name: "Generate AI Architecture"
description: "One-click AI system architecture generation for LLM apps, agent systems, RAG platforms, copilots, and AI-enabled products. Use when you want a structured architecture proposal with technology choices, Mermaid UML diagrams, delivery phases, and key risks."
agent: "Software & AI Architect"
model: "GPT-5 (copilot)"
argument-hint: "Describe the AI product, system, or business scenario you want architected"
---
Design a complete AI system architecture for the user's request.

Requirements for the response:
- Clarify the target users, business goal, and key operational constraints from the given input.
- Propose a practical architecture that can be implemented by a real engineering team.
- Make major component boundaries, data flow, model flow, and external dependencies explicit.
- Choose frameworks and infrastructure deliberately, with brief rationale.
- Include Mermaid diagrams when they improve clarity.
- Cover AI-specific concerns such as orchestration, prompts, retrieval, memory, evaluation, safety guardrails, observability, and fallback strategies when relevant.
- End with phased implementation guidance, major risks, and open assumptions.

Use this output structure:
1. Intent
2. Assumptions
3. Architecture
4. Key Decisions
5. UML
6. Delivery Plan
7. Risks

If the user's input is underspecified, make reasonable assumptions and label them explicitly instead of blocking.