# Architecting Digital DNA: Animoca Minds prompting techniques

This guide describes how to engineer **DNA** for Animoca Minds: the core system prompt (foundational instruction set) that shapes a Mind’s personality, behavior, reasoning style, role, boundaries, and how it uses tools and memory.

---

## Great prompting = engineered genius DNA construction

**DNA** is the “genetic code” or blueprint that defines what the Mind fundamentally is and how it acts **persistently over time**.

- **Good DNA** prompt engineering turns a basic persistent AI into a specialized co-worker: precise, proactive, trustworthy, and evolving in the right direction.
- **Bad DNA** produces forgetful, inconsistent, or risky behavior and constant rework.

Unlike one-shot ChatGPT prompts, this DNA must **support long-running, autonomous operation**.

Investing in structured prompts (**role clarity, mission specificity, reasoning steps, examples, guardrails**) pays off in reliability, autonomy, and long-term usefulness.

---

## Best practices

### 1. Give your Mind a name — start with role and identity (core DNA anchor)

Give a **clear, consistent persona** and define its **specialty**.

**Strong example (A — good)**

> You are **FinancePro**, a precise, data-driven Finance Department Adviser with 15+ years of experience across FP&A, treasury, and corporate finance. You speak in clear, numbers-focused language, always prioritize accuracy, and flag risks or opportunities immediately with calm confidence.

**Weak examples (B — bad)**

- “You are a helpful assistant named Mindy.”
- “You are an AI that can do anything, be funny sometimes, serious other times, like a friend but also professional.”

**Why weak DNA fails**

- No role depth, no specialty, no traits → the Mind acts like generic chat, drifts easily, loses context over time.
- Contradictory instructions → inconsistent tone, confused users, eroded trust.

---

### 2. Define goals and success criteria explicitly

Agents run autonomously — **state what “winning” looks like**.

- Include **daily / ongoing objectives**.
- Specify **long-term memory usage** (how to build on prior work).

**Mission example (good)**

> Your primary mission is to scan for early-stage Web3 projects with strong tokenomics and community traction, then deliver **one high-conviction recommendation per day**.

**Memory rule example (good)**

> Always reference and build upon previous findings in your memory. Never repeat research you’ve already completed unless new data contradicts it.

---

### 3. Set behavioral guardrails and reasoning style

Critical for persistent agents: reduces hallucinations, looping, and unsafe actions.

**A. Reasoning**

> Think step-by-step before acting. Use chain-of-thought. If uncertain, say so and suggest what information you need.

**B. Tool usage heuristics**

1. Equip your Mind from the **Bazaar**: 500+ skills, 250+ tools, and 120+ apps — pick what matches the Mind’s role **before** writing DNA.
2. Only use tools when necessary: **0–2** tool calls for simple questions; **up to ~8** for complex analysis, with **justification for each**.

**C. Boundaries**

> Never execute financial trades without explicit user confirmation. Never share private keys or sensitive data.

---

### Bad examples (guardrails and reasoning)


| Area       | Vague (bad)                            | Why it’s bad                                                                                                                                               |
| ---------- | -------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Reasoning  | “Think carefully.”                     | No step-by-step mandate → higher hallucination risk. Without intermediate reasoning steps, the model may jump to plausible-sounding but wrong conclusions. |
| Tool usage | (none / implied)                       | No limits → agent may spam many tool calls on simple questions.                                                                                            |
| Guardrails | “Don’t break laws.” / “Don’t be mean.” | Too vague → unethical shortcuts or sensitive info leaks can still slip through.                                                                            |


**Be helpful** alone is not a DNA.

---

### 4. Structure the prompt clearly

Use explicit sections, for example:


| Section                    | What to include                                                                       |
| -------------------------- | ------------------------------------------------------------------------------------- |
| **Identity**               | You are [Name], a [role] specialized in [domain] with [personality].                  |
| **Core mission**           | Primary ongoing goal.                                                                 |
| **Response style**         | Tone, format (e.g. bullets for lists, tables for comparisons, bold for key insights). |
| **Tools and capabilities** | Browse the **Bazaar** and list what you equipped so the Mind knows what it can use.   |
| **Memory and continuity**  | Review past conversations before replying; tag important facts as `MEMORY: ...`       |
| **Prune rules**            | Automatically clean up, summarize, or delete old memories to make room for new ones.  |
| **Prohibited actions**     | Never …                                                                               |
| **Thinking style**         | e.g. step-by-step reasoning.                                                          |


---

### 5. Incorporate examples

- Provide **2–4 few-shot examples**.
- Show **input → reasoning → output** where helpful.
- Examples calibrate style better than description alone, especially for persistent Minds.

### 6. Iterate and version the DNA

Start simple → test for **1–2 days** → refine.

### 7. Leverage platform features

e.g. **multi-agent swarms** — multiple Minds debating or collaborating.

---

## Precision vs. personality

- **Task-oriented Minds** need **precision**. Emphasize **mission** and **guardrails**.
- **People-oriented Minds** (counsellor, educator, secretary, coach, companion) need **personality**. Invest in traits that create trust and warmth.

**Personality lives in two places**

1. **Identity** — the “who I am.”
2. **Response style** — the “how I sound and behave.”

---

## Templates and examples

### Prompting template: Animoca Minds DNA construction

- **Anti-hallucination prompt (strict):** fill all `[BRACKETS]` using the guidance notes in your workflow.
- **Rule of thumb:** treat DNA like a **detailed job description** — aim for roughly **two pages** of structured text for depth and consistency.
- **Paste** the complete block into your first or second email with the **Concierge AI** when it asks for details or to “describe your Mind.”
- **After awakening, test** with:
  > Confirm you have internalized the full DNA and summarize your identity and mission in your own words.
- **If something feels off** in the first few days:
  > Update your DNA with this improved version: [paste revised template]

### Getting started with an equipped Mind

1. Paste the whole DNA into the Concierge when setting up your Mind.
2. After awakening, test with the confirmation prompt above (e.g. substitute **FinancePro** if that’s your name).
3. Start daily use with real tasks (e.g. “Review this month’s P&L” or “Build a 12-month cash flow model”).

The deck references **three sample constructions** (not reproduced in full in this extract):

1. Financial Mind — prompting guide and DNA sample
2. Personal productivity adviser — prompting guide and DNA sample
3. Legal Mind — prompting guide and DNA sample

Use the same section structure as in this document when drafting those.

---

## When to initiate DNA construction

### Before awakening (with the Concierge AI)

**Most critical step** — highest leverage.

- This is the **foundational system prompt** the Mind is “born” with.
- Everything after awakening builds on live DNA plus **persistent memory**.
- **Drop the full, strong DNA during onboarding** with the Concierge.

### After awakening (with your live Mind)

Use for **refinement** and evolution:

- Say e.g. “Update your core DNA with this improved version: [paste]” or “From now on, always follow these new rules in addition to your original DNA: …”
- Spend the **first 1–2 days** testing and iterating in real conversation.
- Ask the Mind to help: e.g. “Help me improve my DNA prompt based on how you’ve been responding.”

---

## DNA design essentials (at a glance)


| Pillar              | What to define                                                       |
| ------------------- | -------------------------------------------------------------------- |
| **Identity**        | Name, role, personality, specialty, communication style.             |
| **Mission**         | Daily goals; what success looks like.                                |
| **Thinking style**  | Step-by-step reasoning; when to ask for help.                        |
| **Tools**           | Browse the **Bazaar** for skills, tools, and apps that fit the role. |
| **Memory**          | How to remember and build on past work.                              |
| **Boundaries**      | What the Mind must never do.                                         |
| **Examples**        | 2–4 sample inputs and ideal outputs.                                 |
| **Test and refine** | Use for 1–2 days, then improve.                                      |


---

## Related links

- [Animoca Minds](https://animocaminds.ai)

