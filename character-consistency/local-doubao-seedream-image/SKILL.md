# Doubao Seedream Image

Use this skill for Doubao Seedream image generation through Volcano Ark. It supports Seedream 5.0 Pro, 5.0 Lite, 4.5, and 4.0. It is especially useful before Seedance video work: create character portraits or role sheets with Seedream first, then pass the saved image into the Seedance skill as a reference image.

For long-video, multi-role, storyboard, or multi-reference workflows, avoid polluting the main thread with image base64. For each visual QA pass, use a fresh disposable subagent given only the local image path(s), intended use, and a checklist, and accept only a short text verdict.

## Tool

Run the bundled CLI for all generation; it reads the Ark key from the shared fallback file or the documented environment variables, and can show the active configuration with the key masked. Never print full API keys.

## Model Choice

Choose by capability: 5.0 Pro for the highest-quality single-image generation or editing with multiple references; 5.0 Lite for image sets, storyboards, web-search-enhanced visuals, streaming, and larger output; 4.5 when 2K/4K sets or editing are needed with jpeg output; and 4.0 when 1K output or fast prompt optimization is needed. The full version lists exact model IDs, aliases, and per-model restrictions.

## Configuration

Configuration comes from the Seedream, Ark, and Seedance environment variables in a documented priority order, with defaults for the Ark base URL, model, and image path. Use a Volcano Ark API key — not the separate Volcano Speech key.

## Common Commands

The CLI covers text-to-image, high-quality single-image generation, reusable character references, image-to-image and multi-reference generation, image sets, local prompt optimization, storyboards from scenes, web-search generation, streaming, exact raw JSON payloads, and dry-runs without spending tokens. The full version gives the complete command for each case.

## Workflow

Preserve the user's creative intent and apply the prompt guide before paid generation, optimizing only the expression. Use the character route for reusable Seedance references, the Pro route for high-quality single images, the standard generate route for one-off and multi-reference calls, and the set and storyboard routes for sequential image groups. Save outputs immediately, verify complex work through fresh disposable QA subagents, and pass saved images into Seedance as reference or first-frame inputs.

## Prompt Optimization Rules

Rewrite loose requests into one concise, coherent natural-language paragraph — subject, action or change, environment, purpose, style, color, lighting, composition, exact quoted text, and what must stay unchanged or be avoided. For edits, name the exact object, region, and operation; for references, state what to extract and preserve and refer to images by ordinal; for sets, request consistency of character, style, color, and camera language.

## Notes

The full version records model IDs and aliases, supported input formats, reference-image limits, response and output formats, size presets and pixel constraints, and the conditions for web search, prompt-optimization modes, and raw payloads.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
