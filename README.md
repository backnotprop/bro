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

Practical, QoL skills for daily work with AI.

**Align & clarify**
- `bro`: Restates the last AI response in plain language.
- `readback {prompt}`: Restate my prompt clearly to ensure we are aligned.
- `sharpen`: Sharpens the goal, approach, and scope before doing the work.
- `facts`: List the critical facts I should know before or after an implementation.

**Track & refocus**
- `recap`: Gives a two- or three-sentence recap of recent work, with focus on what happened last.
- `converge`: Pulls a sprawling session back into focus: names the goal, sorts open threads, and picks the one next thing.
- `status`: Renders the work in flight as an ASCII status board in the terminal.
- `ladder`: Renders one lane of work as a vertical progress ladder, done on top and todo below.

**Show it in HTML**
- `big-pics-little-words`: Explains the discussion in HTML with big visuals and few words.
- `one-pager`: Makes one HTML page that shares an idea with teammates early, or recaps work, with big pictures and little words.
- `storyboard`: Shows an end-to-end user and system flow in HTML using cropped UI snippets, automated steps in between, and minimal words.

**Stress-test decisions**
- `clean-room`: Gets an independent verdict from a fresh agent with no access to the current conversation.
- `regret-minimization`: Launches one or more agents to simulate the future with deterministic scripts and cited factual data, then reports back the regrets of today's choices.


### (latest ✨): Storyboard

- `/storyboard [flow or feature]`: Walks through the full lifecycle in HTML using cropped UI snippets, automated steps in between, and minimal words.

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

### Examples

**/status** 

_🔈 btw, want a UI for status?? try [Inbox by Plannotator](https://plannotator.ai/inbox)_

<img width="1168" height="1366" alt="image" src="https://github.com/user-attachments/assets/557b3889-f593-438e-9b76-023b28a7378d" />
