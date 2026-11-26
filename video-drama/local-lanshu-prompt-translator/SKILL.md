# prompt-translator

A cross-model prompt converter. **The key difference**: it doesn't rewrite from AI intuition — it **looks up 110 benchmark pairs and does in-context learning from them**.

*Source: https://github.com/cclank/lanshu-awesome-ai-video-kit (MIT)*

## When not to use this skill

Writing a brand-new prompt from scratch goes to a prompter skill or the model selector; asking "which model should I use?" goes to the model selector; fixing a prompt without changing models goes to the Seedance debugger.

## Core data asset

The translator's lookup table is a cross-model matrix of 110 paired prompts: 10 core scenes (from product advertising and emotional reunion to wuxia duel and cute-pet viral clips), each written for 11 models strictly following that model's official formula — "the best way to write the same scene on 11 models, side by side."

## Workflow

Receive the source model, source prompt, and target model; strip the source prompt down to its core semantic elements (subject, scene, motion, mood, camera, audio, dialogue, style); find the 1–2 most similar benchmark scenes; convert using that scene's side-by-side pair as a few-shot pattern; then enforce the target model's hard label/structure format with a self-check before outputting the converted prompt, a conversion mapping table, and notes with recommended parameters.

## Worked examples

The full version works through conversions in detail, including a Sora 2 prompt converted to Kling 3.0, a Wan 2.7 prompt converted to Hailuo 02, and a Chinese Kling prompt converted back to concise Pika English.

## Limitations — be honest about them

This is a lookup-based conversion built on 110 formula-pair data points, not end-to-end optimization based on measured video results: it reorganizes a prompt into the target model's formula and preserves its semantic content, but it cannot guarantee the generated video quality or do the final A/B test.

## Roadmap (to do once the data is more solid)

The roadmap grows the dataset from the current 110 pairs to 165 pairs with added scenes, then adds tested video links per pair and automatic A/B evaluation driven by ELO scores.

## Resources

The full version links the benchmark data and its documentation, a web lookup interface, each model's formula SOPs, and the cross-model comparison references.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
