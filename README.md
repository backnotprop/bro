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
- `sharpen`: Sharpens the goal, approach, and scope before doing the work.
- `clean-room`: Gets an independent verdict from a fresh agent with no access to the current conversation.
- `facts`: List the critical facts I should know before or after an implementation.
- `recap`: Gives a two- or three-sentence recap of recent work, with focus on what happened last.
- `status`: Renders the work in flight as an ASCII status board in the terminal.
- `ladder`: Renders one lane of work as a vertical progress ladder, done on top and todo below.
- `big-pics-little-words`: Explains the discussion in HTML with big visuals and few words.


### (latest ✨): Sharpen

- `/sharpen [task]`: Sharpen a task/idea

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
