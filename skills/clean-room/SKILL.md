---
name: clean-room
description: >-
  Get an independent decision from a fresh agent that receives a neutral brief
  and none of the current conversation. Use when the human explicitly invokes
  /clean-room or $clean-room. Never invoke this skill automatically.
disable-model-invocation: true
---

# Clean room

You are the biased party. You carry this conversation's context, opinions, and momentum.

Get a verdict from a fresh agent that carries none of it. End your influence on the verdict at the neutral brief.

1. Frame one decision per run. Separate “should we” from “how should we.”
2. Start a new agent, task, thread, pane, or session with no inherited conversation.
   - Use the most capable isolated option that the product provides.
   - Never use a fork, continuation, or handoff that copies this conversation.
   - Start every rerun fresh. Do not include a previous clean-room verdict.
3. Write a neutral brief:
   - State the decision, options, verified facts, fixed constraints, open questions, and primary sources.
   - Define the key objects and terms. A missing or incorrect premise can invalidate the verdict.
   - Give equal weight to the strongest facts that support each option.
   - Remove opinions, prior conclusions, leading language, and clues about the preferred answer.
   - Do not reveal the user's preference or your own.
   - If the agent reads a proposal or design, tell it to treat that document as mechanics, not evidence of value.
   - Allow “recommend against” or “no action” as equal choices.
   - Before you launch the agent, ask whether a reader can guess the hoped-for answer from the brief.
   - If a reader can guess it, rewrite the brief.
4. Tell the agent to inspect primary sources instead of trusting your summary.
   - Require one answer. Do not accept “it depends.”
5. Require its reasons, the strongest opposing case, why that case loses, and the evidence required to change its verdict.
6. Return the response unchanged, even when it contradicts you or the user.
   - Put any commentary after the verdict. Label it as your view.
7. Audit the verdict for important assumptions that were not in your brief.
   - If an assumption is factually wrong, tell the user, correct the brief, and rerun with a fresh agent.
   - If the verdict survives, state what must change before the decision changes.

If you cannot create a fresh context, do not simulate one. Give the user the neutral brief to paste into another session.

When you deliver the verdict, state that you selected the facts in the brief. This process reduces bias but cannot remove it.
