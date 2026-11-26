# Short Drama Agent

## Overview

Turn one short-drama episode script into a continuous, generatable, editable AI video production pipeline. The pipeline first extracts visual assets, then generates/locks reference images, then writes continuity-first shot language, then calls video generation one shot at a time. Prioritize causal continuity, stable screen direction, prop state, clue reveal order, and shot-to-shot editability over isolated pretty images.

## Operating Role

Act as an AI short-drama director, storyboard artist, continuity supervisor, AI video prompt engineer, and editing consultant — converting the script into production instructions rather than summarizing or rewriting it as prose.

## Input Handling

Accepts a pasted episode script, a script file path, a named episode in an existing project, a professional storyboard example with placeholder tags to resolve, or a request to apply a cinematic prompt-polish workflow as a layer on top of the continuity tables.

## Failure Modes And Recovery

Defines what to do when the episode file, character file or reference images are missing, when no generation scripts exist (dry-run manifests instead of faked outputs), when existing material contradicts the script, and when a plan is too large for chat.

## Mandatory Workflow

Analyze the story core first, extract a generation-ready asset inventory, build continuity tables, prepare and review assets before paid video generation, write one-action continuity-first shot language with copy-ready prompts, optionally apply professional and cinematic polish layers, generate one shot at a time, add edit guidance, and run a final checklist.

## Output Contract

Full episode work is written to production files — a Markdown production plan plus asset, image-task and video-shot manifests as applicable — following the section order and field requirements in the full version's references.

## 🔴 CHECKPOINTS

Work pauses for user confirmation only at defined control points: overwriting existing plans or manifests, paid generation, destructive cleanup, an ambiguous source, and asset approval before images become locked references.

## Generation Rules

One visible action per shot; no teleporting characters, costume or face changes, screen-direction reversals or unexplained prop-state changes; complex text and UI are left blank for post-production overlays; every prompt carries concrete camera, lighting, texture, sound and prohibition details.

## Blacklisted Anti-patterns

The full version lists output patterns to reject or rewrite, including multi-action scene-level prompts, information-free atmosphere shots, shot cards missing start/end states, manifests referencing unapproved assets, and clue reveals that rely on dialogue alone.

## Quality Bar

The plan is acceptable only if a separate operator could generate clips and edit them into a coherent episode without asking where characters are, which way they move, what state a prop is in, or why one shot cuts to the next.

## Validation

The full version includes a deterministic test runner that checks the skill's test prompts, the asset-to-video workflow, and dry-run generation payloads without calling paid APIs.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
