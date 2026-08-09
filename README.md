# bro

Practical skills for daily work with AI.

Use them to simplify AI output, identify the facts that matter, and confirm requests before work starts.

No jargon. No bullshit. Straight to the point.

## Skills

- `bro`: Restates the last AI response in plain language.
- `facts`: Lists only the facts that can affect the work, related systems, or the people who use it.
- `readback`: Restates your request before work starts so that you can confirm it.

### Readback

`/readback [long prompt, often voice prompt]`

Use `readback` after a long, dictated, or complex request. The AI states the request clearly and waits for your confirmation.

## Install

```bash
npx skills add backnotprop/bro
```

### Claude Code plugin

```text
/plugin marketplace add backnotprop/bro
/plugin install bro@bro
```

### Codex plugin

```bash
codex plugin marketplace add backnotprop/bro
codex plugin add bro@bro
```
