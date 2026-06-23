---
name: ian-xiaohei-illustrations
description: Generate Ian-style Chinese article illustrations. For users asking to create illustrations for Chinese articles, posts, blogs, Notion docs, workflow docs, methodologies, flows, structures, states, metaphors, or ideas. Includes tasks like "absurd", "Xiaohei", "hand-drawn", "article illustration", "illustration suggestions", "shot list", "remove title/edit image". Default style uses Xiaohei IP, pure white hand-drawn art, sparse red/orange/blue annotations, and a clean yet imaginative visual approach.
---

# Ian Xiaohei Absurd Article Illustrations

## Core positioning

Design and generate 16:9 horizontal article illustrations for Chinese articles. The goal is not commercial illustration, PPT infographics, or cute cartoons. Instead, turn the article's key judgment, flow, structure, state, or metaphor into a clean, absurd, creative, readable hand-drawn explanation image that does not feel like a manual.

The default visual IP is "Xiaohei": a solid black shape with white dot eyes, thin legs, and a blank expression, seriously doing a bizarre but coherent task. Xiaohei must perform the core action in the image, not just stand beside it as decoration.

## Read these references first

Read them as needed. Do not overload context at once:

- `references/style-dna.md`: style DNA, colors, text, no-go items.
- `references/xiaohei-ip.md`: Xiaohei IP appearance, personality, action library, and restrictions.
- `references/composition-patterns.md`: structure types, original metaphor methods, and repetition rules.
- `references/prompt-template.md`: single-image generation prompt template.
- `references/qa-checklist.md`: post-generation checks and iteration rules.
- `assets/examples/`: low-frequency style calibration only. Do not use these cases as default composition, object, or label templates.

## Workflow

### 1. Digest the article

First read the user's article text, link, Notion page, Markdown file, or screenshot content. Extract:

- the core point
- which paragraphs carry cognitive turns
- which ideas are worth illustrating
- which parts are better left as text

Do not illustrate everything evenly. Prioritize "cognitive anchors," such as: core judgment, dual breakpoints, input-output loops, branch paths, before/after contrast, one-fish-many-uses, handoff path, common pitfalls, role state changes.

### 2. Produce an illustration strategy first

If the user only asks "analyze how to illustrate / think about what should be illustrated," output a shot list first. Each image should clearly state:

- where it belongs in the article
- the theme
- the core idea
- the structure type
- what Xiaohei does in the image
- suggested elements
- suggested Chinese label wording

Default 4-8 images. For short articles, 1-3 images; for long articles, do not exceed 9 unless absolutely necessary. Use just enough illustrations, and avoid turning the article into an artbook.

### 3. Generate images one by one

If the user explicitly asks to "generate / output / create images / help me generate," do not pause for confirmation. Use the built-in `image_gen` tool to generate each image separately. Do not put multiple images into one.

Each image should illustrate only one core structure. Prompts must include:

- 16:9 horizontal Chinese article illustration
- pure white background
- black hand-drawn line art
- sparse red/orange/blue Chinese handwritten annotations
- lots of white space
- Xiaohei as the core action subject
- no PPT, commercial illustration, cute cartoon, complex architecture, or top-left title label

Do not copy prior cases. The examples only show style density and Xiaohei participation. Do not directly reuse compositions like "two conveyor breakpoints / Xiaohei pulling a line / material fish / stamp toolbox / common pit path" unless the user explicitly requests a direct remake. Invent a fresh metaphor for the current article every time.

### 4. Check and iterate

After generation, review `references/qa-checklist.md`. If any of these issues occur, prioritize regeneration or local editing:

- Xiaohei is only decoration
- the image is too crowded
- it looks like a flowchart / PPT
- too much Chinese text or severe typos
- a top-left title appears, such as "common pitfalls / workflow / system architecture / route map"
- the style is too cute, childish, or stiff
- the background is not clean white

### 5. Save and deliver

If the user is working inside this workspace, copy the final images to:

```text
assets/<article-slug>-illustrations/
```

Name them in order:

```text
01-topic-name.png
02-topic-name.png
```

Keep the original generated files. Do not overwrite existing assets unless the user explicitly asks to replace them.

## Output expectations

Before generation, keep the strategy output short and precise. After delivery, include:

- how many images were generated
- the purpose of each image
- save paths
- which images are the safest, and which are optional

Do not write long essays about style theory. Let the images speak for themselves.
