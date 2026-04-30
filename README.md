# Throw Rock 🪨

**Efficient model-to-model delegation for AI agents.** Free. Open source. MIT licensed.

Compressed machine-language protocol that reduces token usage by 40-60%.

Skills compound. Prompts don't.

## Install

### Hermes Agent
```bash
git clone https://github.com/wizzleweasel/throw-rock.git ~/.hermes/skills/throw-rock
```

### OpenClaw
```bash
git clone https://github.com/wizzleweasel/throw-rock.git ~/.openclaw/skills/throw-rock
```

### Other Claw Agents
```bash
git clone https://github.com/wizzleweasel/throw-rock.git
# Copy skills/ directory to your agent's skills path
```

## What It Does

| Concept | Natural Language | Machine Language | Compact Tier1 | Savings |
|---------|-----------------|------------------|---------------|---------|
| Code analysis | ~800 tokens | ~300 tokens | ~100 tokens | **87%** |
| File operations | ~400 tokens | ~150 tokens | ~50 tokens | **87%** |
| Terminal commands | ~300 tokens | ~100 tokens | ~35 tokens | **88%** |

**New:** Supports 3 compressed formats (Tier 1-3) cutting tokens by 60-90% additional savings over standard JSON.

## When to Use

Triggers automatically when:
- Delegating subtasks to helper models (Groq, etc.)
- Need to reduce token costs
- Batch processing multiple operations
- Repetitive tool calls

## How It Works

Main model translates tasks to JSON, helper model works in structured format, no verbose English in delegation layer.

Each skill is a `SKILL.md` file following the [Agent Skills](https://agentskills.io) open standard:

```yaml
---
name: throw-rock
description: "Efficient model delegation using compressed protocol. Use when: delegating to helper models; need to reduce token costs; batch processing"
---
```

The description tells agents **when** to use the skill. The body provides full protocol — task format, response format, examples.

Works across **Hermes Agent, OpenClaw, Claude, ChatGPT, Copilot, Cursor, Windsurf** — any tool that supports the Agent Skills standard or MCP.

## Quality

Reviewed against agent skill best practices:

- **Clear triggers** — "Use when:" terms for reliable discovery
- **Agent-first** — Protocol only, no explanations agents already know
- **Concise** — Machine language only, no fluff
- **Output contracts** — Declared JSON format for composability

## Catalog

1 skill for model delegation:

| Skill | Description |
|-------|-------------|
| throw-rock | Compressed machine-language delegation protocol (40-60% token savings) |

## Token Savings

| Scenario | Natural | Machine | Savings |
|----------|----------|----------|---------|
| Code analysis | ~800 | ~300 | **62%** |
| File operations | ~400 | ~150 | **62%** |
| Terminal commands | ~300 | ~100 | **67%** |
| Search results | ~600 | ~200 | **67%** |

## Test

```bash
# Test
python scripts/throw_rock.py "read file main.py"

# Hermes Agent
hermes --test-skill throw-rock

# OpenClaw
openclaw --test-skill throw-rock
```

---

**Skills compound. Prompts don't.** Use throw-rock to reduce token costs by 40-60%.