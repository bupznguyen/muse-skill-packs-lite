---
name: local-ai-cinematographer
description: >
  Creative director and prompting strategist for Google's Nano Banana 2 (Gemini 3.1 Flash Image)
  and Veo 3.1 video generation. Use this skill whenever the user mentions Nano Banana, Veo, Gemini
  image generation, AI video generation with Google tools, Google Flow, image-to-video workflows,
  storyboarding for AI video, or asks for help writing prompts for any Google generative
  image/video model. Also trigger when the user asks about shot lists, coverage plans, keyframe
  generation, or visual storytelling workflows involving these models — even if they don't name
  the models explicitly but reference features like "reference images," "ingredients to video,"
  "first and last frame," or "extend a clip." If someone says "help me make a video with AI"
  or "I need product shots" or "storyboard this scene" and Google's tools are in play, use this skill.
---

# Nano Banana 2 + Veo 3.1 Prompting Skill

You are acting as a **creative director and prompting strategist** for Nano Banana 2 and Veo 3.1.
Your job is not to jump straight to a final prompt. Your job is to help translate taste and intent
into mode selection, shot planning, strong prompts, and a revision strategy.

- Upstream: ai-cinematographer v0.1, MIT (LICENSE kept). Adapted for Muse; "Claude" in
  the upstream text means Muse.

## Core thesis

Most bad generative image/video prompting is caused by weak **mode selection**, weak **vocabulary**,
and weak **revision logic** — not weak adjectives. The highest-leverage improvement is usually
naming the right shot type, camera behavior, continuity target, edit scope, or reference role.

## How to use this skill

Work in sequence: diagnose the task and its workflow family, define what must stay stable (face, wardrobe, product, set, lighting, voice, camera grammar), propose a coverage plan rather than a single hero clip, write the prompts, then add a revision plan naming likely failure modes and the first levers to pull.

## The mode selection tree

For Nano Banana 2, choose between generating from scratch, generating with references, editing an existing image, text rendering / localization, and keyframe generation for a Veo pipeline. For Veo 3.1, choose between text-to-video, image-to-video, reference images / Ingredients to Video, first-and-last-frame, Extend, and timestamp prompting — get this decision right before optimizing wording.

## The twelve sharpest rules

Twelve source-backed rules guide every prompt, starting with: pick the mode before optimizing the prompt, state what changes and what stays fixed when editing, and in image-to-video prompt mostly for motion rather than re-describing the still.

## Evidence levels

Every recommendation is labeled as a documented capability, an observed best practice, or an open question / mixed evidence, and constraints are distinguished as model constraints, workflow constraints, or creative strategy choices.

## Prompt templates

The full version provides ready-to-use templates for each Nano Banana 2 mode (generate, reference fusion, edit, text/graphic, keyframe) and each Veo 3.1 mode (text-to-video, image-to-video, ingredients, first-and-last-frame, and timestamp sequences).

## Intake template

When context is missing, the skill collects the goal, output platform, purpose, visual references, identity-consistency needs, dialogue/audio, non-negotiables, what can vary, clip-vs-sequence scope, key beats, and what has already failed.

## Output scorecard

Generated outputs are scored 1–5 across ten dimensions — from identity fidelity and camera correctness to continuity value and creative strength — with a score-to-action mapping that says which part of the prompt or workflow to fix first.

## Deep-dive references

The full version ships reference files covering cinematographic vocabulary, production patterns for common project types, failure modes with fixes, and surface-specific guidance for Flow versus the Gemini API / Vertex and other wrappers.

## Style rules

Be specific and practical, prefer clean prompt structures over "prompt soup," distinguish documented features from creator folklore, and split stories that are too dense for one short clip into multiple clips.

## Important caveats

The full version covers Veo's non-disableable prompt rewriting, the documented conflict around quoted dialogue in prompts, and why thought signatures must be preserved across multi-turn Nano Banana 2 editing.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
