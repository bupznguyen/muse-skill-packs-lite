# seedance-debugger

Input: a problematic prompt + the symptoms the user describes (or a video screenshot).
Output: a diagnosis (root cause) + the fixed prompt + an explanation of why it was changed this way.

*Source: https://github.com/cclank/lanshu-awesome-ai-video-kit (MIT)*

## When not to use this skill

If no prompt has been written at all and the user just wants a new prompt, use the Seedance prompter; if the user wants to break down a complex story, use the Seedance storyboard skill.

## Diagnostic manual for the 12 problem categories

The full version is a diagnostic manual for 12 problem categories — character ID drift, subtitles, logo / watermark, style drift, extension jumps, twins, quality degradation, wrong effects, too many reference characters, end noise, Chinese pronunciation, and inaccurate voice — each with its root cause and fix strategy, plus a symptom-identification table that routes a described symptom to the right category.

## Workflow

Collect the symptoms first (asking the symptom, the original prompt, and the reference assets used when the report is vague), diagnose against the 12 categories, and output a diagnostic report with the fixed prompt, a table of what changed and why, and other possible root causes. When a problem is a known model limitation that a prompt cannot solve 100%, say so clearly and recommend a specific post-production remedy.

## Worked examples

The full version works through three fixes in detail: the twins problem (four identical people instead of two), style drift (an anime target coming out as a real person), and subtitles and a watermark appearing together.

## Reference resources

The full version links a masterclass synthesis expanding the practical pitfalls, the full 12-questions methodology, a constraint-word checklist, and the special character conventions.

## Full version
This is a free lite preview. The full version — with the complete workflow, prompt libraries, references and any scripts — is part of the paid pack on Agensi: https://www.agensi.io/users/bupz-nguyen
