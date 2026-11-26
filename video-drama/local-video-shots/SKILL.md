## video-shots

**Shot breakdown** for a finished film — break one video down into a shot-by-shot analysis table: **duration, size, category, camera move, frame**.

**The premise is baked in: shot boundaries are measured, not eyeballed.** So there is a hard line down the middle: code measures cuts, durations, film length, frame rate and each shot's motion, and checks the result against 15 quality gates; the model judges only size, category, camera, frame and rhythm from keyframes. The hardest gate is camera vs. measured motion — claiming a large camera move while the measured frame-to-frame change is near zero is blocked outright.

**Boundaries (what this does not do)**: no speech transcription, no face recognition or automatic character merging, no judgement of whether the film is good, no editing or clip export, and no object detection inside shots.

### Step 0 — Fix the input and the scope

All you need is one video file. Fix two things first — the whole film or one section, and what the breakdown is for (imitation reference, edit-rhythm analysis, or delivery-asset inventory) — or go with the stated defaults and say so in the report.

### Step 1 — Seed the working draft

A zero-dependency script uses ffmpeg scene detection to seed a draft with measured start, end, duration and motion per shot; the size, category, camera and frame cells are left empty as the model's job. Read the detection summary and re-run with an adjusted threshold rather than making do with a bad draft.

### Step 2 — Extract keyframes and contact sheets

Extract an opening and a closing frame per shot and tile them into contact sheets — one set for content, one for camera work — reading the sheets first and single frames only for shots that cannot be called from the sheet.

### Step 3 — Fill in the four fields, batch by batch

Working one contact sheet at a time against the bundled taxonomy, fill in size, category, camera, frame and optional rhythm, judging camera from the opening/closing framing difference plus the measured motion — and trusting the measurement when the two disagree. Machine-measured fields are never edited by hand.

### Step 4 — Add missed cuts and merge invented ones

Scene detection misses cuts on dissolves and dark-on-dark cuts and invents them on handheld shake and flashes; a recut command splits and merges shots, renumbers, recomputes durations and motion, and clears annotations on changed shots so they are judged again.

### Step 5 — Validate

Run validation and fix every violation one by one until it passes: all 15 gates are code, covering timeline continuity, duration self-consistency, vocabularies, checkable frame descriptions, category evidence, camera vs. measured motion, declared manual cuts, keyframes and rhythm annotation. A skipped gate is not a pass, and the report must say so.

### Step 6 — Produce the report and report back

Render a Markdown table and a single interactive HTML report — embedded player with shot highlighting, a shot pace strip, searchable and filterable shot lists, distributions, cast and quality gates — then report back the shot count, average shot length, cuts per minute, dominant sizes and camera moves, and the report path.

## Boundaries

The full version details the limits: dialogue comes only from subtitles burned into the picture, measured motion cannot distinguish camera movement from subject movement, dissolves need a declared midpoint cut, long films are broken down in sections, and bilingual Chinese/English operation switches labels and gate criteria together.

## Self-test

A bundled self-test exercises every quality gate with a breaking test case; it calls no model and spends no tokens, and is run first after changing the script.

## Bundled example

The full version includes a complete worked breakdown of an AI short film — shots data and motion track — that serves as both the quality benchmark and the self-test fixture.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
