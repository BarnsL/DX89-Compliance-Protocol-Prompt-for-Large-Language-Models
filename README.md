# DX89 Compliance Protocol Prompt for Large Language Models

A structured system prompt that enforces strict compliance, self-auditing, and hallucination reduction in LLM outputs.

> Paste it into any LLM. Every response gets a preflight check, evidence anchoring, confidence scoring, and a release gate.

---

## What It Does

DX89 is a portable system/developer prompt that forces any LLM (ChatGPT, Claude, Gemini, etc.) to:

- **Anchor every response in time** with millisecond-precision timestamps
- **Declare evidence mode** (none, internal file, web, mixed) so you know what backs each claim
- **Self-audit** with an observation ? interpretation ? response ? confidence skeleton
- **Score confidence** on a per-claim basis and flag uncertainty explicitly
- **Gate release** — responses are PASSED, BLOCKED, or QUARANTINED before delivery
- **Learn from failures** — generates safeguards based on prior errors and applies them going forward
- **Refuse async cop-outs** — no "I'll do that later" or "please wait" stalling

---

## Usage

1. Copy the contents of the prompt (in this repo's README or the variant files).
2. Paste it as a **System Prompt** or **Developer Message** in your LLM of choice.
3. Every response from the model will now follow the DX89 skeleton.

---

## Variants

| File | Target |
|------|--------|
| `README.md` | Universal portable prompt (any LLM) |
| `DX89 for Amazon Quicksight Q` | Tuned for QuickSight Q analytics |
| `Gemini Personal Intelligence Entry` | Tuned for Google Gemini |

---

## Sample Outputs

| File | Demonstrates |
|------|-------------|
| `Sample Output` | Basic DX89-compliant response (Beef Wellington recipe) |
| `Sample Audit Output` | Self-audit and safeguard generation |
| `Sample Lotus Health AI Output` | Health/wellness domain compliance |

---

## Why

LLMs hallucinate. They present guesses as facts. They say "I'll look into that" and never do. DX89 eliminates these failure modes by making the model prove its work on every turn — time-anchored, evidence-declared, confidence-scored, and gated.

---

## License

LGPL-2.1