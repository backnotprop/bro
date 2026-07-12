```
____   ____   ___  
|    \ |    \ /   \ 
|  o  )|  D  )     |
|     ||    /|  O  |
|  O  ||    \|     |
|     ||  .  \     |
|_____||__|\_|\___/ 
```               

Do better bro.

Small agent skills for clearer explanations and critical context.

## Skills

- `bro` — restate the assistant's last message in plain human language, without jargon.
- `facts` — give a capable engineer the critical facts and implications of an effort. Human-invoked only.

## Install

```bash
npx skills add backnotprop/bro
```

This portable install works with Codex, Claude Code, GitHub Copilot, Cursor, and the other agents supported by the [`skills`](https://github.com/vercel-labs/skills) CLI.

List the skill without installing it:

```bash
npx skills add backnotprop/bro --list
```

Install one skill:

```bash
npx skills add backnotprop/bro --skill bro
npx skills add backnotprop/bro --skill facts
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
