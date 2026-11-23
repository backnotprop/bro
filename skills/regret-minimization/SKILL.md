---
name: regret-minimization
description: >-
  Launch one or more agents to simulate the future with deterministic scripts
  and cited factual data, then report back the regrets of today's choices.
disable-model-invocation: true
---

# Regret minimization

Launch an agent to play in the future, simulate how today's choices unfold, and come back with what we would regret.

1. Frame the decision and scenarios.
   - Identify the choice(s) being made today, the options or scenarios to test (including "do nothing" when relevant), and the time horizon(s) that matter.
   - Run this once for a single path, or `n` times with separate agents (subagents, tasks, or sessions)—one per decision option or scenario, in parallel when possible—so each future plays out independently.
2. Give each agent a clean brief of today's baseline.
   - Include the specific choice or scenario it is playing out, verified facts, fixed constraints, and pointers to primary sources.
   - Do not steer it toward defending or rejecting the choice.
3. Have each agent simulate the future with deterministic scripts and cited facts.
   - Gather factual data first (codebase measurements, logs, benchmarks, pricing, docs, or current external data) and cite every source inline throughout the analysis and inside the scripts.
   - Generate and run whatever deterministic scripts are needed to simulate the future—cost, capacity, latency, or growth models, failure or bottleneck checks, sensitivity sweeps, or fixed-seed simulations. Compute numbers with code, never mental math.
   - Keep generated scripts in a temporary or scratch directory so the repo stays clean unless the user asks to keep them.
   - Separate cited facts from assumptions, and test sensitivity when key assumptions move.
4. Return from the future with concrete regrets.
   - Report the specific regrets about today's choices: what compounded badly, broke, locked us in, or foreclosed better options—backed by script outputs and cited data.
   - Distinguish severe or irreversible regrets from cheap, reversible ones, and note what early signal would have caught each regret in time.
   - State what we would wish we had changed, hedged, or chosen differently today.
5. Synthesize across all `n` runs.
   - For a single run, return the agent's regrets, citations, and script results directly.
   - For multiple runs, preserve each agent's findings and citations, then compare the regret profiles side by side: highlight regrets that recur across futures and call out which choice minimizes severe or irreversible regret.
