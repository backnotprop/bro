---
name: clean-room
description: Get an independent decision from a fresh agent that receives a neutral brief and none of the current conversation. Use when the user asks for a clean-room review, unbiased decision, independent opinion, fresh eyes, or a decision made away from the current chat.
---

# Clean room

1. Start a new agent, task, thread, pane, or session with no inherited conversation.
2. Never use a fork, continuation, or handoff that copies this conversation.
3. Give the new agent a neutral brief:
   - State the decision, options, verified facts, fixed constraints, open questions, and primary sources.
   - Give equal weight to the strongest facts that support each option.
   - Remove opinions, earlier conclusions, leading language, and clues about the preferred answer.
   - Allow the agent to reject the premise or recommend no action.
4. Ask the new agent to inspect the primary sources and choose one answer.
5. Do not accept “it depends” as the verdict.
6. Require its reasons, the strongest opposing case, and why that case does not win.
7. Return its response unchanged, even when it conflicts with the current conversation.

If the product cannot create a fresh context, do not simulate one. Give the user the neutral brief to paste elsewhere.

This process reduces bias but cannot remove it. The brief writer still chooses which facts to include.
