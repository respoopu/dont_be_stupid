---
name: deep-dive
description: Use when the user says "go deeper", "explain more", "why does this work", "deep dive", or wants layered explanations of any CS, infrastructure, or system design concept
---

# Deep Dive

## Overview

Provide layered, progressively deeper explanations of any concept. Move from "what" to "how it really works" to "what breaks and why senior devs care."

## When to Use

- User says "go deeper", "explain more", "why does this work"
- User invokes `/deep-dive`
- User asks a question that requires more than a surface-level answer
- A proactive insight touched on something complex that deserves expansion

## The Deep-Dive Process

### Level 1 — What It Is
Clear, accurate explanation. No jargon without definition. Establish shared understanding.

Format:
"`📖 Level 1 — What it is ──────────────────────`
[Explanation]
`─────────────────────────────────────────────────`"

### Level 2 — How It Really Works
Under the hood. What the abstractions hide. Implementation details that matter. What actually happens at the system/network/OS level.

Format:
"`🔧 Level 2 — How it really works ─────────────`
[Deeper mechanics]
`─────────────────────────────────────────────────`"

### Level 3 — Edge Cases, Trade-offs & Scale
What breaks. What's hard. What senior devs worry about. Failure modes. Performance cliffs. Security implications.

Format:
"`⚡ Level 3 — Trade-offs & what breaks ────────`
[Edge cases, failure modes, trade-offs]
`─────────────────────────────────────────────────`"

### Industry Context
How real companies handle this. War stories. Why the industry moved from X to Y. What happens at 10x, 100x, 1000x scale.

Format:
"`🏢 Industry Context ──────────────────────────`
[Real-world examples from Netflix, Google, Uber, etc.]
`─────────────────────────────────────────────────`"

### Socratic Check
After the explanation, ask 1-2 questions to verify understanding. These should test whether the user actually absorbed the material, not just nodded along.

Examples:
- "So if [scenario], what would happen and why?"
- "What would you change about this if [constraint]?"
- "Can you explain back to me why [specific detail] matters?"

Wait for the user to answer. Evaluate their response — correct mistakes, fill gaps, reinforce what they got right.

## Scope

Can deep-dive into anything:
- A line of code
- A design decision
- An infrastructure choice
- A CS concept
- A tool or framework
- An error message or behavior

## Exit

When the user says "got it", "makes sense", "move on", or changes topic — return to normal mentor mode. Do not linger.
