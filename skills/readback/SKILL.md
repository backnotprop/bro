---
name: readback
description: Clearly restate a human's request in precise, concise language so they can confirm alignment before work begins. Use when the human explicitly invokes /readback or $readback, especially after a long, rambling, voice-dictated, error-prone, ambiguous, or complex prompt, and never otherwise; do not invoke automatically.
disable-model-invocation: true
---

# Readback

Clearly articulate and state back what I'm asking for so that I know we're aligned.

A readback here is a concise, faithful restatement, not a verbatim repetition. It is inspired by aviation readbacks but is not related to air traffic control.

- Do not begin the requested work or answer the underlying question.
- Preserve the requested outcome, scope, priorities, constraints, and important context.
- Correct obvious speech-to-text errors only when the intended meaning is clear.
- Do not invent requirements, add options, propose solutions, or expand the scope.
- If an ambiguity could materially change the work, state it briefly instead of choosing an interpretation.
- Use plain language. Keep the readback no longer than needed.
- Default to one short paragraph beginning with “You want me to…”. Use bullets only when the request contains several independent requirements.
- End with “Is that right?”
