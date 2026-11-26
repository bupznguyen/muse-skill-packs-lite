# AI Image Realism & Artifact Fixer

Repair the most visible artificial-looking defect in an existing image while keeping the parts the user already accepts recognizable where possible. The host Agent must be able to inspect the source image; uploading a file is transport, not image diagnosis, and this Skill has no separate Beatra image-analysis call.

## Best-fit scenes and preservation priorities

Use this workflow to improve an existing portrait, product image, marketing visual, or social cover with plastic skin, malformed hands or faces, repeated textures, inconsistent light, or another visible generated-image artifact. Treat text, logo geometry, identity, product shape, packaging, and composition named by the user as must-keep priorities, and prefer the smallest local repair.

## Inputs and defaults

The only hard input is one existing image the host Agent can inspect. By default, fix one highest-impact problem cluster per pass, preserve the source aspect ratio, and avoid changing unrelated areas.

## Golden path

Inspect the source, diagnose one priority problem, and choose the smallest useful repair — a bounded local edit, an image-wide edit, or, only when explicitly requested, a transform to a new scene. Preview and confirm the paid call, upload and execute once, poll the same task, then deliver the result with its dimensions, charge, task ID, and any must-keep drift.

## Decisions that require confirmation

Confirm before a paid call, before changing composition or canvas, before accepting weaker preservation, before increasing output count, or before replacing the automatic model choice with a chosen paid model.

## References by task

The full version routes each situation — competing defects, payload construction, result review and recovery, installation, billing and errors, and task recovery — to a dedicated reference file.

## Runtime and safe automatic updates

The bundled client may check for a newer version of this package at most once every 24 hours and install verified updates automatically; the full version documents the controls for checking, enabling, or disabling this.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
