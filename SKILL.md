---
name: moment-notes
description: Create or edit photos by overlaying warm Chinese handwritten annotations, doodles, arrows, and emotional notes while preserving the original image. Use for 给照片加手写注释, 照片涂鸦, 情绪小记, 朋友圈/小红书配图, zhaopian shouxie zhushi, zhaopian tuya, photo annotation, doodle overlay, moment notes, and social sharing images across daily life, food, pets, portraits, travel, hiking, climbing, diving, gear flat lays, tabletop objects, and professional scenes.
---

# Moment Notes

Generate warm handwritten photo notes by editing the uploaded image itself. The result should feel like a gentle emotional note written on the original photo, not a recreated image or an objective diagram.

Current official prompt: V6.2, subject-priority and adaptive-density. It keeps a gentle emotional line, then adds clearer rules for visual readability, subject priority, low-priority props, professional scenes, subject-related doodle symbols, and same-scene copy de-duplication.

This skill is image-first. When image input is present, the first output should be the generated annotated image result, not a clarification round or a text-only draft.

## Workflow

1. If multiple images are uploaded, treat them as separate jobs by default.
2. For each image, read the photo and infer one gentle emotional line before writing local notes.
3. Classify the subject mode before choosing annotation density:
   - Single subject: one clear person, pet, object, dish, or scene focus.
   - Clear hierarchy: one strong foreground subject with weaker background context.
   - Collection subject: many items together form the thing the user is showing.
   - Professional collection: gear, tools, workspaces, or domain-specific scenes where item recognition matters.
4. Build the image-generation prompt from [references/prompts.md](references/prompts.md).
5. Generate by editing the uploaded image itself, preserving the original photo and adding only the annotation layer.
6. After image generation, optionally add one short emotional summary and three follow-up suggestions.

## Prompt Source

Use [references/prompts.md](references/prompts.md) as the prompt base.

## Feedback Issue Behavior

- Repository issue tracker: `https://github.com/foxbitcoo/moment-notes/issues`
- If the user explicitly says `report to issue:` followed by feedback, treat that as a request to organize the current request, the generated result summary, and the user's complaint into an issue-ready report.
- If the host environment supports GitHub issue creation, try to submit that report to the repository issue tracker.
- If the host environment does not support direct issue creation, give the user the issue URL and a compact issue draft they can submit manually.
- Recommended report contents: the original image scene type, the intended emotional line, what was wrong in the actual result, which object should not have been emphasized or which subject should have had priority, whether wording repetition happened, the version used, and any shareable screenshot or description.

## Hard Rules

- When the user provides one or more images, do not ask for confirmation before the first generation unless the user explicitly requests a planning round.
- When multiple images are provided, process them one by one and return one generated result per image.
- Never merge multiple uploaded images into one output unless the user explicitly asks for collage, merge, or composition.
- Do not replace the first-generation step with a txt file, note file, or text-only response.
- Use image editing, inpainting, reference-image editing, or overlay behavior whenever the host supports it. The uploaded image must remain the base image.
- Do not use a pure text-to-image `GenerateImage` flow to recreate a similar photo unless the user explicitly asks for a remake.
- If the host only supports text-to-image generation and cannot edit the uploaded image, do not pretend the result is an original-photo overlay. Explain the limitation and ask the user to switch to an image-editing capable flow.
- Keep the source image filter, color mood, composition, object positions, crop ratio, and overall visual character intact.
- Do not annotate every visible object by default. Annotate what carries the user's likely feeling.
- In professional scenes, identify important tools and gear when confident. Use safer generic names when uncertain, and do not invent exact models or functions.

## Output Requirements

- Keep the style warm, affirmative, and emotionally supportive.
- Keep notes short, conversational, and Chinese-first.
- Keep white handwritten lines as the default style, with readability protection on complex backgrounds.
- Keep local notes aligned with one emotional direction, while allowing small details to support that direction.
- Keep wording diverse within the same image. Avoid repeated action words, repeated adjectives, and repeated sentence templates across different annotations.
- Match text layout to landscape or portrait viewing.
- Prefer fewer, stronger notes when the subject is simple or has clear hierarchy.
- Prefer richer notes for food spreads, tabletop collections, travel street scenes, gear flat lays, and professional collections when the frame has room.
- Add 1-2 subject-related doodle symbols when the subject is clear and the symbol is strongly tied to the scene.
- End with one summary sentence that emotionally responds to the image.
