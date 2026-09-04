```
____   ____   ___  
|    \ |    \ /   \ 
|  o  )|  D  )     |
|     ||    /|  O  |
|  O  ||    \|     |
|     ||  .  \     |
|_____||__|\_|\___/ 
```               
Alignment shouldn't be so hard.

## Skills

Practical, QoL, skills for daily work with AI.

- `bro`: Restates the last AI response in plain language.
- `facts`: Lists only the facts that can affect the work, related systems, or the people who use it.
- `readback`: Restates your request before work starts so that you can confirm it.
- `recap`: Gives a two- or three-sentence recap of recent work, with focus on what happened last.
- `clean-room`: Gets an independent verdict from a fresh agent with no access to the current conversation.
- `status`: Renders the work in flight as an ASCII status board in the terminal.

### (latest ✨): Status

- `/status`: Renders the current work as an ASCII board, grouped by phase, one row per item, instead of a status paragraph.

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
