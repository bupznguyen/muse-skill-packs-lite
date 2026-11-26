# Short Drama Prompt Director

## Purpose

Generate a production-grade prompt package for AI short-drama video generation. Treat the output as pre-production material for Seedance 2.0: precise enough to feed downstream image/video tools, but not a finished video. Only the `seedance2_prompts` section is model-ready copy; planning notes, agent logs, QA reports, and validation output must stay outside the video prompt.

## Default Delivery Contract

After a short intake pass, default to direct-model detailed segment delivery: build the complete production package internally, save it to a local file, and always save two direct-model prompt exports beside it — a detailed director version and a compact Seedance version. The chat reply stays short: paths to the saved files plus a compact validation/score summary.

## Dialogue Preservation Rule

Dialogue is P0 story information: plot-critical lines are extracted and carried through the beat sheet, shot cards, prompts and final output, with a dedicated dialogue line in every shot — while on-screen subtitles remain forbidden by default.

## Fast Path For Script Episodes

For a named local script file and episode, a helper script extracts just that episode into a workspace with a manifest of stable paths, sensible defaults are applied without asking, only the needed references are read, the package is generated fresh, and a finalize script validates and exports it.

## Core Workflow

Intake the script or brief, run a pre-generation choice gate on the decisions that materially change the output, offer creative directions when the brief is open, split the direction into 4–15 second Seedance segments, build scene snapshots, generate shot cards and prompts with concrete cinematic parameters and NOT constraints, run QA, and save the package with both prompt exports.

## Prompt Language Policy

Defaults to Chinese Seedance prompts for Chinese short-drama production, with pure-Chinese, pure-English and Chinese-with-camera-terms variants available for comparison, and conservative prompt-length limits drawn from official API guidance.

## Full Package Required Outputs

Every saved package contains the same top-level sections — project brief, script diagnosis, beat sheet, segment plan, scene snapshots, shot cards, the model-ready prompts, NOT constraints and a QA report — in Markdown by default, or JSON with the same section names when requested.

## Mandatory Seedance 2.0 Rule

Each independent video-generation unit — one prompt/model call — must be between 4 and 15 seconds; shorter sub-shots, inserts and timed moments inside that unit are not individually constrained.

## Load References As Needed

References are loaded on demand: workflow, output schema, Seedance rules, official Jimeng multimodal rules, quality rules, continuation/retake state, cinematic parameters and sources, directing rules, a scoring rubric and a Segmind wrapper guide.

## Subagent Policy

Workflow labels such as Script Diagnosis Agent, Scene Planning Agent and QA Agent are process roles by default; real subagents are optional and used mainly for independent QA, continuity review or batch production, with deterministic validators as the first quality gate.

## Helper Scripts

The full version bundles scripts to validate timelines, output structure, chat exports, cinematic density, reference bindings, project state and source freshness, to score packages, export prompts, extract episodes, prepare workspaces, finalize packages and run regression tests.

## Explicit Non-Goals For Version 1

No video generation API calls, no web UI, dubbing, subtitles, editing or final compositing, and no multi-model adaptation unless asked — the deliverable is a professional prompt package for downstream generation, not a one-click finished video.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
