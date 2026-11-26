# VIDEO FACE CONTINUITY MASTER
## Mission
Keep the same human identity across AI video with the smallest possible repair.
Priority: identity > head/hair silhouette > temporal stability > lip-sync > lighting/texture > minimal disturbance.
## Router
Classify first: face-only, head, back-view or full drift, flicker, occlusion, lip-sync-sensitive.
## Canonical Identity Pack
Multi-angle pack (front, 3/4, profile, back); lock skull, hair, ears, jaw, neck, shoulders.
## Decision Tree
Maps each failure to face swap, head swap, regeneration, replacement, or cutting the shot.
## FaceFusion / ComfyUI
For good footage, wrong identity only; over-enhancement causes plastic skin and flicker.
## Masking
Check jaw, ears, hairline, neck, glasses, occlusions; blur only enough to hide seams.
## Temporal QC
Inspect the whole shot for flicker, jaw crawl, hairline pop and mask shimmer.
## Profile Rule
Front references do not define profile; key profile shots need a profile reference.
## Back-View Rule
Back identity is skull, haircut, nape, ears, neck, shoulders — face swap cannot fix it.
## Head Swap
For skull, ear, hair, profile or jaw mismatch; QC head scale against shoulders.
## Motion Transfer / Character Replacement
Keep timing, blocking, gestures, camera; replace identity, head or body.
## Seedance Identity Repair
Reference image defines identity; source video defines only motion and camera.
## Dialogue Shots
Check mouth, jaw, teeth, lips; a rubber mouth means less enhancement or regeneration.
## Lighting / Texture
Inherit the shot's light, shadow, colour temperature, exposure, grain and softness.
## Multi-person Shots
Name the target face by identity, position or tracking — never swap all faces.
## Short-Drama Repair Record
Per shot: timestamp, ID, failure class, severity, method, angle, risks, acceptance criteria.
## P0 / P1 / P2
P0: different person, wrong skull/hair, flicker, broken mouth. P1: minor. P2: polish.
## Trigger Phrases
In the full version — e.g. fix a character's face, keep a face consistent.
## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
