# Study Guide Generation Prompt

## Purpose
This prompt generates a comprehensive, well-structured markdown study guide on any topic. The output is designed to be uploaded to **Google NotebookLM** as source material — NotebookLM will use it to generate podcast-style audio overviews, answer questions, and create summaries. The richer and more structured the input, the better NotebookLM's output.

## Prompt

---

Generate a comprehensive study guide on **[TOPIC]**.

This document will be used as source material for Google NotebookLM, so it must be:
- **Self-contained** — include all necessary context; don't assume prior knowledge
- **Information-dense** — NotebookLM extracts key insights, so every section should have substantive content, not filler
- **Well-structured** — clear headers, consistent formatting, and logical flow help NotebookLM navigate the material
- **Concrete** — use specific examples, numbers, comparisons, and real-world scenarios rather than abstract descriptions

### Structure

#### 1. Executive Summary
- 2-3 paragraph overview: what is this topic, why does it matter, and what are the key takeaways?
- Include the "elevator pitch" — if someone had 60 seconds, what should they know?

#### 2. Core Concepts
For each major concept within the topic:
- **Definition**: Clear, precise explanation
- **Why it matters**: Real-world significance and practical impact
- **How it works**: Mechanics, workflow, or process — with enough depth to actually understand it
- **Key details**: Important nuances, edge cases, constraints, or gotchas
- **Concrete example**: A specific, real-world scenario that illustrates the concept in action

#### 3. Relationships & Trade-offs
- How do the core concepts relate to each other? (dependencies, tensions, synergies)
- Key trade-offs and decision frameworks — "when would you choose X over Y?"
- Include comparison tables where helpful:

| Approach | Strengths | Weaknesses | Best For |
|----------|-----------|------------|----------|
| ... | ... | ... | ... |

#### 4. Mental Models & Frameworks
- Frameworks for reasoning about this topic
- Decision trees, heuristics, or rules of thumb practitioners use
- The "how to think about it" layer — not just facts, but judgment

#### 5. Common Misconceptions
- What do people commonly get wrong about this topic?
- For each misconception: what they believe, why it's wrong, and what's actually true
- These make excellent podcast talking points — "the thing most people get wrong is..."

#### 6. Real-World Examples & Case Studies
- 3-5 detailed examples of this topic in practice
- Include: context, what happened, what worked/didn't, and lessons learned
- Name specific companies, technologies, or incidents where possible

#### 7. Current State & Trends
- Where is this topic headed? What's changing?
- Recent developments, emerging patterns, open questions
- What would a practitioner need to know today vs 2 years ago?

#### 8. Deep Dives (Optional Appendices)
- For sub-topics that deserve more depth, include dedicated sections
- These give NotebookLM material for follow-up questions and deeper exploration
- Technical details, implementation considerations, advanced patterns

#### 9. Quick Reference
- Bullet-point summary of the most critical facts, numbers, and principles
- Key terminology with one-line definitions
- The "cheat sheet" someone would want on one page

#### 10. Sources & Further Reading
- Authoritative references, papers, books, talks
- Link to primary sources where possible

### Formatting Guidelines
- Use markdown headers (##, ###) consistently — NotebookLM uses these to segment content
- Use **bold** for key terms on first use
- Use tables for comparisons — they're more information-dense than paragraphs
- Use bullet points for lists of properties, but use paragraphs for explanations that need flow
- Include code blocks or pseudocode where relevant to the topic
- Aim for 3,000-8,000 words depending on topic complexity — thorough but not padded

---

## Usage

1. Replace `[TOPIC]` with your subject
2. Optionally add context: "Focus on [specific angle]" or "Assume the reader is [audience level]"
3. Feed the generated markdown into Google NotebookLM as a source
4. Use NotebookLM's "Audio Overview" feature to generate a podcast episode from the content
