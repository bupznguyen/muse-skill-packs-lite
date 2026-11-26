# Character Consistency

Keep the user's character identical across every generated shot. The method: expand a short Brief into ultra-detailed prompts, turn the prompts into a character sheet, and ride the sheet on every generation the character appears in.

The core job of this skill is **expansion**. Every one-line field in the Brief becomes a paragraph of specifics in the prompt. Vague prompts produce generic faces — and a generic face cannot stay consistent. Detail is what consistency is made of.

## What it does

**Input:** a filled Character Brief (a freeform description is fine — it gets mapped into the Brief and shown back first). **Output:** an ultra-detailed close-up prompt, a three-panel sheet prompt (bust-up / full body front / full body rear), and the role line for every later prompt where the character appears. This skill writes prompts only — the user runs the generations.

## Step 0. Fill the Character Brief

Collect name, age/build, face, hair, outfit (item by item: garment, material, color, wear), any existing close-up, and notes on vibe and visual style. Fill blanks with conservative proposals and show the completed Brief; ask only when two readings would produce different people.

## Step 1. Lock the close-up

Expand the Brief into an ultra-detailed close-up prompt structured around eyes (highest priority), skin, hair, expression, visible clothing and technical style. The user generates several candidates and picks one — the picked image becomes the character.

## Step 2. Generate the three-panel sheet

Run a sheet prompt with the close-up attached as reference: one 16:9 sheet, three panels on a seamless cool grey background, restating the full identity and outfit, since the close-up shows nothing below the chest. Also deliver the role line: the sheet defines the character's features, hairstyle and clothing — not its background or layout.

## Self-check

Confirm the Brief is complete (especially the outfit), every field was expanded into specifics, all three panels read as the same person on plain grey, and the role line was delivered.

## What this skill does not do

It does not write full video prompts, call any generation API, or make generation deterministic — it supplies the identity assets video prompts ride on.

Based on the character-consistency skill from https://github.com/nigo-studio/ai-film-skills (MIT License).

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
