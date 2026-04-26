---
name: moment-notes
description: Create emotional hand-drawn annotations on photos with scene understanding, emotion mapping, and orientation-aware text layout. Use when generating lightweight image notes for daily sharing, especially when the user wants meaningful mood expression from a single moment photo.
---

# Moment Notes

Generate image annotations with three layers:
1. Visible elements in the photo
2. Scene understanding behind those elements
3. Emotional response that the viewer can feel

## Workflow

1. Read the photo and list key elements.
2. Infer the scene context and one dominant emotional line.
3. Decide whether the main viewing orientation is landscape or portrait.
4. Keep all annotation text direction aligned with that orientation.
5. Produce local notes plus one final summary line.

## Prompt Source

Use [references/prompts.md](references/prompts.md) as the prompt base.

## Output Requirements

- Keep line style lightweight and hand-drawn in white.
- Keep language short, conversational, and emotional.
- Keep all local notes aligned with one emotional direction.
- Keep text layout consistent with landscape or portrait viewing.
- End with one summary sentence that emotionally responds to the image.
