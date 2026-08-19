---
name: clean-room
description: >-
  Get an independent decision from a fresh agent that receives a neutral brief
  and none of the current conversation. Use when the human explicitly invokes
  /clean-room or $clean-room. Never invoke this skill automatically.
disable-model-invocation: true
---

# Clean room

Launch a smart, independent agent to give us an unbiased third-party decision analysis. Give it only neutral facts and context.

Do not frame the brief toward the user's preferred answer or any alternative. We want a fair opinion from an agent with no access to this conversation.

You are the biased party. You carry this conversation's context, opinions, and momentum.

Get a verdict from a fresh agent that carries none of it. Give the fresh agent only the neutral brief.

Do not steer it afterward or reshape its verdict.

1. Frame one decision per run. Separate “should we” from “how should we.”
2. Start a new agent, task, thread, pane, or session with no inherited conversation.
   - Use the most capable isolated option at your disposal.
   - Prefer a smarter agent when the decision is complex, consequential, or difficult to reverse.
   - Never use a fork, continuation, or handoff that copies this conversation.
   - Block access to the current workspace if your tools allow it.
   - Otherwise, tell the agent not to inspect the workspace or read any local file that the brief does not name.
   - Start every rerun fresh. Do not include a previous clean-room verdict.
3. Write a neutral brief:
   - State only the decision, options, verified facts, fixed constraints, open questions, and allowed sources.
   - Name every local file, if any, that the agent may read.
   - Omit background that is not required to understand the decision.
   - Define the key objects and terms. A missing or incorrect premise can invalidate the verdict.
   - Give equal weight to the strongest facts that support each option.
   - Remove opinions, prior conclusions, leading language, and clues about any preferred answer.
   - Do not include the user's sentiment, preferred outcome, or prior reactions. Do not include your own.
   - Present each option without saying who proposed or prefers it.
   - Do not frame the task to make the agent infer or deliver the answer that the user wants.
   - If an allowed source is a proposal or design, tell the agent to treat it as mechanics, not evidence of value.
   - Allow “recommend against” or “no action” as equal choices.
   - Before you launch the agent, ask whether a reader can guess the hoped-for answer from the brief.
   - If a reader can guess it, rewrite the brief.
4. Let the agent reason freely, but limit the evidence it can gather.
   - It may read only the materials named in the brief.
   - Do not let it search the workspace, repository, commit history, issues, plans, notes, ADRs, or other local files.
   - Allow web research only for checkable facts from official documentation, specifications, pricing pages, and provider limits.
   - Do not use blogs, opinion pieces, forums, social posts, reviews, summaries, or third-party comparisons.
   - Let it challenge the premise, find other options, and gather missing facts within these limits.
   - Tell it to search the allowed sources for evidence against its answer.
   - Require one answer. Do not accept “it depends.”
5. Require its reasons, the strongest opposing case, why that case loses, and the evidence required to change its verdict.
6. Return the response unchanged, even when it contradicts you or the user.
   - Put any commentary after the verdict. Label it as your view.
7. Audit the verdict for important assumptions that were not in your brief.
   - If an assumption is factually wrong, tell the user, correct the brief, and rerun with a fresh agent.
   - If the verdict survives, state what must change before the decision changes.

If you cannot create a fresh context, do not simulate one. Give the user the neutral brief to paste into another session.

When you deliver the verdict, state that you selected the facts in the brief. This process reduces bias but cannot remove it.
