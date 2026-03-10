# Learning Accelerator

A system of Claude Code skills that turns Claude into a senior dev mentor — teaching as you work, not just doing the work for you.

## What It Does

### Always-On Mentor (CLAUDE.md)
Every session, Claude proactively:
- Surfaces **insights** on every code interaction (the why, alternatives, CS fundamentals, industry context)
- Asks **senior dev questions** at natural breakpoints ("What happens if this service goes down?")
- Evaluates your answers and fills knowledge gaps

### Deep Dive (`/deep-dive`)
Say "go deeper" or `/deep-dive` on any topic to get:
- **Level 1** — What it is
- **Level 2** — How it really works under the hood
- **Level 3** — Edge cases, trade-offs, what breaks at scale
- **Industry context** — How Netflix, Google, etc. handle it
- **Socratic check** — Questions to verify you actually understood

### Mock Interview (`/mock-interview`)
Say "quiz me" or `/mock-interview` to enter interview mode:
- Choose a focus: system design, infrastructure, code reasoning, general CS, or mixed
- Answer questions as stream-of-consciousness (like you're speaking)
- Get per-answer evaluation: accuracy, clarity, depth, gaps
- See how a senior dev would have answered
- Get a session summary with strengths and weak spots

## Installation

Copy the skill files to your Claude Code config:

```bash
# Mentor behavior (always-on)
cp config/CLAUDE-mentor-config.md ~/.claude/CLAUDE.md

# Skills (on-demand)
mkdir -p ~/.claude/skills/deep-dive ~/.claude/skills/mock-interview
cp skills/deep-dive/SKILL.md ~/.claude/skills/deep-dive/SKILL.md
cp skills/mock-interview/SKILL.md ~/.claude/skills/mock-interview/SKILL.md
```

## Usage

Just open Claude Code in any project. The mentor behavior is automatic.

| Command | What it does |
|---------|-------------|
| *(just code)* | Proactive insights + questions |
| "go deeper" / `/deep-dive` | Layered explanation on any topic |
| "quiz me" / `/mock-interview` | Mock interview with evaluation |
| "simpler" | Adjust explanation level down |
