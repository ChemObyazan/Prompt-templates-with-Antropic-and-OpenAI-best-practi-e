# 📑 Prompt Templates for Popular AI Prompt Frameworks

A curated, production-ready library of **XML prompt templates** aligned with industry best practice for OpenAI, Antropic, Google, Meta, Alibaba and others (clear roles, data/instruction separation, structured outputs).  
This repository includes templates for **general-purpose tasks, reasoning/chain-of-thought, and specialized reflective/coaching scenarios**.

---

## 📚 Frameworks Included

### 🔹 General Purpose
- **Role, Input, Steps, Expectation, Narrowing (RISEN)**
- **Persona, Goal, Task, Context (PGTC)**
- **Request, Task, Format (RTF)**
- **Role, Action, Context, Execute (RACE)**
- **Task, Action, Goal (TAG)**
- **Situation, Task, Action, Result (STAR)**
- **Concise, Logical, Explicit, Adaptive, Reflective (CLEAR)**
- **Specific, Measurable, Achievable, Relevant, Time-bound (SMART)**
- **Role, Input, Directive, Examples (RIDE)**
- **Purpose, Role, Output, Mechanics, Parameters, Testing (PROMPT)**
- **Task, Audience, Purpose (TAP)**

### 🔹 Reasoning & Chain-of-Thought
- **Chain-of-Thought Prompting (CoT)**
- **Tree-of-Thought Prompting (ToT)**
- **Clarity, Contextualization, Command, Chaining, Continuous Refinement (5C)**

### 🔹 Specialized
- **Goal, Obstacles, Logic, Data (GOLD)**
- **Present, Explore, Analyze, Choose, Evaluate (PEACE)**
- **Describe, Interpret, Evaluate, Plan (DIEP)** – Reflective prompting

---

## Usage

1. Pick a framework template (e.g., templates/RISEN.md).
2. Replace bracketed placeholders: [role], [data], [output requirements].
(Optional) Instruct the model to return JSON for structured outputs.

## Best practices baked in

1. Clear role & audience
2. XML for inputs; 
3. JSON for outputs (optional)
4. Step-by-step reasoning hooks
5. Guardrails (don’t invent facts, follow schema)
6. Iteration & reflection prompts

Example (RISEN)
<prompt>
  <role>You are a medical tutor.</role>
  <input>
    <data>[Insert patient case]</data>
  </input>
  <steps>
    - Identify key symptoms
    - Propose differentials
    - Justify each briefly
  </steps>
  <expectation>Return 3 differential diagnoses with reasoning.</expectation>
  <narrowing>Use only the provided data.</narrowing>
</prompt>

## Contributing
PRs welcome! Add new frameworks, improve wording, or include runnable examples.
