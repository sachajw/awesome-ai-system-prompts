# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Repository Purpose

This is a curated collection of AI system prompts from various AI tools and agents, along with analysis documentation. It serves as a research resource for understanding how different AI products architect their system prompts.

## Structure

Each AI product has its own directory containing:
- System prompt files (`.md`, `.txt`, `.js`, `.ts`, `.py`, `.json`)
- README files with context/explanations where applicable
- Supporting schemas (tool definitions, function schemas)

```
ProductName/
├── README.md          # Context about the product/prompt
├── system.md          # Main system prompt
├── tools.json         # Tool/function schemas (if separate)
└── extraction-scripts/ # Any extraction utilities
```

## Key Files

- `README.md` — Comprehensive analysis of prompt patterns across all products
- `security/AI-SYSTEM-HARDENING.md` — Attack vectors and mitigations for AI agents
- `Clawdbot/` — Modular prompt architecture example (SOUL.md, AGENTS.md, IDENTITY.md)

## Contributing New Prompts

1. Create a directory with the product name (use proper capitalization: `ProductName`)
2. Add the system prompt file(s) with descriptive names (include dates for versioned prompts: `system-2025-04-16.md`)
3. Include a brief README.md explaining the source and any relevant context
4. If the prompt references external schemas (tools, functions), include those files
5. Update the main README.md if your addition reveals new patterns worth documenting

## Naming Conventions

- **Directories**: Product name as used officially (`ChatGPT`, `Claude-Code`, `same.new`)
- **Prompt files**: Descriptive names with dates when versioned (`4-5.md`, `system-2025-04-16.md`)
- **Supporting files**: Match the original format (`tools.json`, `functions-schema.json`, `AgentLoop.txt`)

## Analysis Approach

When analyzing prompts, focus on:
- **Role definition**: How the AI's identity and scope are established
- **Tool integration**: How tools are defined and when to use them
- **Planning mechanisms**: Explicit loops, thinking tags, or iterative rules
- **Safety protocols**: Refusal handling and content policies
- **Domain specificity**: Embedded expertise and constraints
