<p align="center">
  <img src="https://em-content.zobj.net/source/apple/391/rock_1faa8.png" width="120" />
</p>

<h1 align="center">throw-rock</h1>

<p align="center">
  <strong>why use many token when few token do trick</strong>
</p>

<p align="center">
  <a href="https://github.com/wizzleweasel/throw-rock/stargazers"><img src="https://img.shields.io/github/stars/wizzleweasel/throw-rock?style=flat&color=yellow" alt="Stars"></a>
  <a href="https://github.com/wizzleweasel/throw-rock/commits/main"><img src="https://img.shields.io/github/last-commit/wizzleweasel/throw-rock?style=flat" alt="Last Commit"></a>
  <a href="LICENSE"><img src="https://img.shields.io/github/license/wizzleweasel/throw-rock?style=flat" alt="License"></a>
</p>

<p align="center">
  <a href="#before--after">Before/After</a> •
  <a href="#install">Install</a> •
  <a href="#compression-levels">Levels</a> •
  <a href="#required-skills">Dependencies</a> •
  <a href="#benchmarks">Benchmarks</a>
</p>

<p align="center">
  <strong>🪨 Throw Rock Ecosystem</strong> &nbsp;·&nbsp;
  <strong>throw-rock</strong> <em>throw compressed rock</em> <sub>(you are here)</sub> &nbsp;·&nbsp;
  <a href="https://github.com/wizzleweasel/pierced-tongue">pierced-tongue</a> <em>transport layer</em> &nbsp;·&nbsp;
  <a href="https://github.com/juliusbrussee/caveman">caveman</a> <em>talk less</em>
</p>

---

Efficient model-to-model delegation protocol that uses **compressed machine language** to cut tokens by 40-75% while keeping full technical accuracy.

**Required skills:** [pierced-tongue](#required-skills) (transport) + [caveman](https://github.com/juliusbrussee/caveman) (language compression)

Based on the observation that compressed JSON/symbolic notation dramatically reduces LLM token usage without losing technical substance. So we made it a one-line install.

## Before / After

<table>
<tr>
<td width="50%">

### 🗣️ Normal Delegation (82 tokens)

> "Please analyze this codebase and tell me what it does, focusing on architecture and dependencies. I need a comprehensive overview."

</td>
<td width="50%">

### 🪨 Throw Rock (28 tokens — Tier 1)

> `{"a":"analyze","p":{"pa":"/app","f":"arch"},"o":"j"}`

</td>
</tr>
<tr>
<td>

### 🗣️ Normal Delegation

> "Can you please read the file main.py and then run the tests using pytest? Let me know the results."

</td>
<td>

### 🪨 Throw Rock (12 tokens — Tier 2)

> `→rf(pa:main.py)∴tr(cmd:pytest)∴`

</td>
</tr>
</table>

**Same task. 65% less tokens. Technical accuracy stay.**

**Pick your compression level:**

<table>
<tr>
<td width="33%">

#### 🪨 Tier 1: Compact JSON

> `{"a":"rf","p":{"pa":"main.py"},"o":"j"}`

- 27% savings vs standard JSON
- Still readable
- Easy to debug

</td>
<td width="33%">

#### 🪨 Tier 2: Symbolic (Default)

> `→rf(pa:main.py)∴`

- 56% savings vs natural
- Mathematical notation
- Best balance

</td>
<td width="33%">

#### 🔥 Ultra (Caveman + Symbolic)

> `rf(main.py)∴`

- 75% savings combined
- Caveman language + symbolic
- Maximum compression

</td>
</tr>
</table>

**Same delegation. You pick how many tokens.**

```
┌─────────────────────────────────────┐
│  TOKENS SAVED          ████████ 65% │
│  TECHNICAL ACCURACY    ████████ 100%│
│  SPEED INCREASE        ████████ ~2x │
│  REQUIRED SKILLS       pierced + caveman │
└─────────────────────────────────────┘
```

- **Faster delegation** — less tokens to generate = speed go brrr
- **Easier to parse** — structured formats, no wall of text
- **Same accuracy** — all technical info kept, only fluff removed
- **Save money** — 65% less tokens = less cost
- **Fun** — every delegation become efficient

## Install

Pick your agent. One command. Done.

| Agent | Install |
|-------|---------|
| **Hermes Agent** | `git clone https://github.com/wizzleweasel/throw-rock.git ~/.hermes/skills/throw-rock` |
| **OpenClaw** | `git clone https://github.com/wizzleweasel/throw-rock.git ~/.openclaw/skills/throw-rock` |
| **Claude Code** | `git clone https://github.com/wizzleweasel/throw-rock.git skills/` |
| **Any other** | `git clone https://github.com/wizzleweasel/throw-rock.git` |

Install once. Use in every session after that. One rock. That it.

### What You Get

Auto-activation is built in. Throw Rock auto-starts when:
- Delegating subtasks to helper models
- Need to reduce token costs
- Batch processing multiple operations

## Required Skills

Throw Rock needs these skills to work:

### 🗣️ pierced-tongue (Transport Layer)
**Required for:** Model-to-model communication transport  
**Install:** `git clone https://github.com/wizzleweasel/pierced-tongue.git`  
**Provides:** HTTP/stdio/ACP transport protocols

### 🪨 caveman (Language Compression)
**Required for:** Token-efficient natural language output  
**Install:** `git clone https://github.com/juliusbrussee/caveman.git`  
**Provides:** 75% token savings via caveman-speak

### Dependency Chain
```
throw-rock (delegation protocol)
    ↓ requires
pierced-tongue (transport) + caveman (compression)
    ↓ enables
Efficient model-to-model delegation (40-75% total savings)
```

## Benchmarks

| Scenario | Natural Language | Standard JSON | Tier 1 Compact | Tier 2 Symbolic |
|----------|-----------------|----------------|-----------------|------------------|
| Code analysis | ~800 tokens | ~300 | ~220 (27%) | ~120 (56%) |
| File operations | ~400 tokens | ~150 | ~110 (27%) | ~60 (56%) |
| Terminal commands | ~300 tokens | ~100 | ~73 (27%) | ~40 (56%) |
| **With Caveman** | **~200** (75%) | **~150** (50%) | **~110** (73%) | **~60** (80%) |

*Combined with caveman language compression*

## Compression Levels

| Level | What changes |
|-------|--------------|
| **Tier 1: Compact JSON** | Short keys (`a`=`action`, `p`=`params`). Remove whitespace. Still JSON. |
| **Tier 2: Symbolic** (default) | Math notation (`→`=delegate, `∴`=result). Best savings. |
| **Ultra: Caveman+Symbolic** | Caveman language + symbolic. Maximum compression. |

Example — "Read file main.py and run tests":
- Tier 1: `{"a":"rf","p":{"pa":"main.py"}}` → `{"a":"tr","p":{"cmd":"pytest"}}`
- Tier 2: `→rf(pa:main.py)∴→tr(cmd:pytest)∴`
- Ultra: `rf(main.py)∴tr(pytest)∴`

## Auto-Activation

ACTIVE EVERY DELEGATION. No revert after many turns. Still active if unsure. Off only: "stop throw-rock" / "normal mode".

Default: **Tier 2 (Symbolic)**. Switch: `/throw-rock tier1|tier2|ultra`.

## Rules

Drop: verbose English, greetings, explanations. Structured formats OK. Technical terms exact. Code blocks unchanged. Errors quoted exact.

Pattern: `[action]([param]:[value])∴`

Not: "Sure! I'd be happy to help you read that file and then run the tests..."  
Yes: `→rf(pa:main.py)∴→tr(cmd:pytest)∴`

## Integration

### With pierced-tongue (transport)
```python
from pierced_tongue import Transport

transport = Transport(config='pierced-tongue-config.yaml')
result = transport.send(target='groq-helper', message='→rf(pa:main.py)∴')
```

### With caveman (compression)
```
Normal: "The file contains 3 functions and 2 classes."
Caveman: "File have 3 func, 2 class."
Caveman+Symbolic: `rf→3 func,2 class∴`
```

## Testing

```bash
# Smoke test
python scripts/throw_rock.py --test

# Hermes Agent
hermes --test-skill throw-rock

# OpenClaw
openclaw --test-skill throw-rock
```

---

**Skills compound. Prompts don't.** Throw Rock with pierced-tongue + caveman = maximum efficiency. 🪨🗣️