---
name: local-flow-prompting
description: >
  Write professional AI video generation prompts for Google Flow (powered by Veo 3.1/Veo 2).
  Use this skill whenever the user needs to create footage prompts, video generation prompts,
  visual scene descriptions, or B-roll prompts targeting Google Flow or Veo models. Also trigger
  when the user mentions "Flow", "Veo", "Google video generation", "footage prompt", "AI footage",
  or asks to generate cinematic scene descriptions for AI video tools. Covers the full prompting
  formula (cinematography + subject + action + context + style), camera movement vocabulary,
  lighting descriptors, audio prompting for Veo 3.1, credit optimization on Google AI Ultra,
  and known model strengths/weaknesses from community production testing. Essential for any
  YouTube production workflow that uses Google Flow for B-roll, establishing shots, or
  narrative footage generation.
---

# Google Flow Footage Prompting Skill

This skill enables Claude to write production-quality video generation prompts
for Google Flow (Veo 3.1 / Veo 2) within a YouTube content production pipeline.

## When to Read Reference Files

Before writing prompts, consult the reference files in the full version: the prompt formula reference (always first), the Ultra pricing reference for budget planning, and the community insights reference for model selection and failure modes.

## Core Prompt Architecture

Every Flow prompt follows a five-part formula — cinematography + subject + action + context/environment + style & ambiance — in that order, at a target length of 3–6 sentences (100–150 words).

## Model Selection Matrix

The full version tabulates which Veo model to use per production phase — fast models for iteration and drafts, quality models for final hero footage — and warns that credit cost is per output, not per request.

## Prompt Writing Workflow

For each scene: determine the shot requirements from the script, check the model strength matrix to confirm Flow is the right tool, write the prompt with the five-part formula, add the audio layer (Veo 3.1 only), set generation parameters, and iterate before the final render.

## Output Format

Each footage prompt is delivered as a structured block with shot type, movement, model, aspect ratio, duration, outputs, and credit estimate, followed by the prompt text and any audio, negative prompt, and fallback model with its rationale.

## Extension and Chaining

Scenes longer than 8 seconds use the Extend feature, with coherence limits after a few extensions; longer scenes are planned as multiple separate generations joined by match cuts or dissolves.

## Advanced Techniques

The full version covers timestamp prompting for multi-shot sequences in one generation, the First + Last Frame workflow for controlled motion, and Ingredients to Video for keeping specific characters, objects, or styles consistent across clips.

## What NOT to Prompt

Key avoidances include instructive negatives, more dialogue than fits in ~8 seconds, re-describing a reference image in image-to-video mode, and quotes around dialogue — plus the limits of character consistency and of audio outside text-to-video mode.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
