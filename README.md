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
- `readback {prompt}`: Restate my prompt clearly to ensure we are aligned.
- `facts`: List the critical facts I should know before or after an implementation.
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
