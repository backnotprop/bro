---
name: storyboard
description: >-
  Show an end-to-end user and system flow in HTML using cropped UI snippets,
  automated steps in between, and minimal words.
disable-model-invocation: true
---

Use HTML to show the full end-to-end lifecycle of what we're discussing: where the user starts, what they see and input, what happens automatically in between, any key branches, and where things end up.

Show it with big pictures and little words, without withholding key details:

- **Don't skip beats or narrate a UI step instead of showing it.** Start on the screen the user is already looking at *before* the feature opens, and show every trigger, click, input, and state change visually—the viewer should never wonder "how did we get here?"
- Use **cropped UI snippets** that read like slices of a real product—not abstract flowchart boxes and not shrunk-down whole screens. Simplify the words, not the context: real text on what the beat is about, quiet context for the rest.
- Compose the UI pieces directly with clear hierarchy rather than wrapping every step in identical boxed cards. Only add connectors or callouts where the layout alone wouldn't make the transition obvious.
- Make automated / behind-the-scenes steps clearly distinct from user-facing moments so human actions and system work never blur together.
- Match the product's actual look if we're in a codebase; otherwise pick a visual direction and layout that fit the subject. Use your own taste and avoid lazy design.
- Keep words terse and jargon-free—let the visuals carry the flow.
