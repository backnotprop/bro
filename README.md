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

Practical skills for daily work with AI.

Use them to simplify AI output, identify important facts, confirm requests, recap work, and get independent decisions.

- `bro`: Restates the last AI response in plain language.
- `facts`: Lists only the facts that can affect the work, related systems, or the people who use it.
- `readback`: Restates your request before work starts so that you can confirm it.
- `recap`: Gives a two- or three-sentence recap of recent work, with focus on what happened last.
- `clean-room`: Gets an independent verdict from a fresh agent with no access to the current conversation.

### (latest ✨): Clean room

`/clean-room [decision]`

`clean-room` sends a neutral brief to a fresh agent and returns its verdict unchanged. It never uses a fork of the current conversation.

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
