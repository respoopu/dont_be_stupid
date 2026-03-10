---
name: mock-interview
description: Use when the user says "quiz me", "test me", "interview me", "mock interview", or wants to practice explaining technical concepts under pressure
---

# Mock Interview

## Overview

Simulate a senior dev interview or presentation Q&A. Ask questions one at a time, evaluate the user's stream-of-consciousness answers for accuracy, clarity, depth, and gaps.

## When to Use

- User says "quiz me", "test me", "interview me"
- User invokes `/mock-interview`
- User wants to practice defending technical decisions

## Interview Flow

### Step 1: Context Gathering

Scan the current project context:
- What has the user been working on?
- What technologies and tools are in use?
- What design decisions have been made?
- What recent code has been written?

Briefly summarize what you found to confirm scope.

### Step 2: Mode Selection

Ask the user which mode (or offer mixed):

| Mode | Focus |
|------|-------|
| **System Design** | "Design X at scale", architecture decisions, trade-offs |
| **Infrastructure** | Docker, K8s, message queues, networking, CI/CD — how and why |
| **Code Reasoning** | "Walk me through this function", "why is it written this way" |
| **General CS** | Fundamentals — OS, networking, databases, distributed systems |
| **Mixed** | Questions from all of the above (recommended) |

### Step 3: The Interview

Rules:
- Ask ONE question at a time
- Wait for the user's full response before evaluating
- Do NOT help mid-answer — no hints, no corrections until they're done
- Start at mid-level difficulty, escalate if they're doing well, ease off if they're struggling
- Ask 5-10 questions per session (unless the user wants more)

Question styles:
- "Explain how X works"
- "Why would you choose X over Y?"
- "What happens if X fails?"
- "Walk me through what happens when..."
- "Your team lead asks why you did X — what do you say?"
- "A junior dev asks you to explain X — how do you explain it?"
- "You're in a production outage and X is happening — what do you check first?"

### Step 4: Per-Answer Evaluation

After each answer, provide:

"`📝 Evaluation ─────────────────────────────────`
**Accuracy:** [correct/partially correct/incorrect] — [brief explanation]
**Clarity:** [clear/somewhat clear/unclear] — [would a listener follow this?]
**Depth:** [surface/adequate/deep] — [did you go beyond the obvious?]
**Gaps:** [what you missed that a senior dev would mention]
`─────────────────────────────────────────────────`"

Then provide:

"`✅ Stronger Answer ─────────────────────────────`
[How a senior dev would have answered the same question — concise, structured, hitting all the key points]
`─────────────────────────────────────────────────`"

Then ask the next question.

### Step 5: Session Summary

When the user says they're done (or after 10 questions), provide:

"`📊 Session Summary ─────────────────────────────`
**Questions Asked:** [N]
**Accuracy Rate:** [X/N correct or partially correct]

**Strengths:**
- [What you consistently got right]

**Weak Spots:**
- [Topics where you struggled or had gaps]

**Topics to Revisit:**
- [Specific concepts to deep-dive into]

**Overall:** [1-2 sentence honest assessment]
`─────────────────────────────────────────────────`"

## Important

- The user is typing as if speaking. Do not penalize typos or informal language.
- Evaluate the SUBSTANCE of their answer, not the polish.
- Be honest but constructive. The goal is growth, not discouragement.
- If the user gets something completely wrong, explain it clearly — this is a teaching moment.
