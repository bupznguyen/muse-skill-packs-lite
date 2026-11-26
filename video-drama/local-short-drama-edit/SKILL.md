# Short-Drama Editing and Final Film

Assemble the per-shot material of one episode into a finished film, and record the choices in an edit sheet. Each edit-sheet section binds one storyboard shot ID and one real media file.

Choose the usable clips from the actual material and check the narrative against the screenplay and storyboard. When material and intent disagree, record the choices and the gaps.

## Quick Start

Invoke the skill on an episode whose produced shots already exist, and it cuts them into a finished film with an accompanying edit sheet.

## Entry

The entry condition is that the material already exists and is readable — finished prompts or a successful generation job do not count as usable material. Incomplete material can be cut as a marked fragment with the gaps listed, and input clips must share one aspect ratio and frame rate for the built-in renderer.

## Workflow

Watch every clip in full and mark its usable band, locate spoken spans for dialogue shots, choose narrative in- and out-points inside the usable range, order shots and check adjacent relationships, compare picture consistency across joins, handle sound joins and loudness, write subtitles from the screenplay text, write the edit sheet, render, and verify the finished film.

## Edit sheet requirements

The edit sheet opens with the delivery spec (target duration, aspect ratio and frame rate, delivery loudness, subtitles) and one section per segment recording its source shot and file, self-consistent in-point, out-point and duration, the reasons for both points, sound handling, any join correction, and its subtitle text. Unused shots are listed with reasons that distinguish missing files from unusable quality.

## Boundaries

No new material is generated at this stage, upstream screenplay and storyboard semantics are not changed, the screenplay's sound design is followed, and a technically successful render is never written up as a quality conclusion.

## Commands

The bundled tool provides check, render and verify commands: check validates the edit sheet against the material without rendering, render cuts and splices the segments, burns subtitles and unifies loudness, and verify measures the finished film and reports numbers only.

## Knowledge on demand

The full version links references on stage boundaries, usable bands in generated footage, cut craft, sound and subtitles, delivery verification, a finished edit-sheet example, and an optional subtitle-overlay route with adjustable typography.

## Revisions

Unaffected segment IDs are kept; the edit sheet is updated before re-rendering, and when a segment is deleted the report states which segment takes over its information or that the information no longer appears.

## Completion

Work is complete when every segment is bound to real material with a self-consistent range, dialogue is complete and audible, subtitles match the screenplay character for character, edit points have no audible hard cuts, loudness lands on the delivery target, and every unused shot has a stated reason.

## Installation and maintenance

A self-test script is run only when installing, upgrading or troubleshooting the skill.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
