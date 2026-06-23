# Balajitechlabs Illustrations

> A Codex skill for generating absurd, hand-drawn Chinese article illustrations with the Xiaohei visual IP.
>
> 16:9 horizontal | white background | black sketch lines | sparse red/orange/blue notes

---

## What this repository is

This repository contains the `balajitechlabs-illustrations` Codex skill. It is designed to guide AI agents to generate inline illustrations for Chinese articles, blog posts, Notion content, workflow documentation, and methodology content.

The goal is not to produce commercial illustration, PPT diagrams, or cute cartoon art. Instead, it turns a key idea, flow, structure, state, or metaphor from the article into a clean, absurd, readable hand-drawn sketch.

The default visual identity is "Xiaohei": a solid black figure with white dot eyes, thin legs, and a blank serious expression. Xiaohei participates in the core action of the illustration, not just decorates it.

---

## What this project produces

Default output:

- 16:9 horizontal article illustrations
- a shot list of 4-8 illustration ideas for one article
- per-image theme, core idea, structure type, Xiaohei action, and Chinese label suggestions
- final PNG assets saved to `assets/<article-slug>-illustrations/`

Not intended for:

- PPT / PDF / Keynote
- SVG / HTML / Canvas editable art
- brand hero posters or polished flat illustration
- dense text-heavy infographics

---

## Key design principles

- pure white background with no texture, gradient, shadow, or noise
- black hand-drawn line art with thin, slightly wobbly strokes
- large whitespace, with the subject occupying about 40%-60% of the canvas
- sparse Chinese handwritten annotations in red/orange/blue
- one illustration should convey only one core action, structure, state, or metaphor
- Xiaohei must be the active protagonist in the image

---

## Repository structure

```text
.
├── README.md
├── LICENSE
├── NOTICE.md
├── assets/
│   └── ian-wechat-qr.jpg
├── examples/
│   ├── images/
│   │   ├── 01-two-breakpoints.png
│   │   ├── 02-sort-by-purpose.png
│   │   └── ...
│   └── prompts.md
└── balajitechlabs-illustrations/
    ├── SKILL.md
    ├── agents/
    │   └── openai.yaml
    ├── assets/
    │   └── examples/
    └── references/
        ├── style-dna.md
        ├── xiaohei-ip.md
        ├── composition-patterns.md
        ├── prompt-template.md
        └── qa-checklist.md
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/Balajitechlabs/balajitechlabs-illustrations.git
cd balajitechlabs-illustrations
```

Copy the skill into your Codex skills directory:

```bash
mkdir -p "${CODEX_HOME:-$HOME/.codex}/skills"
cp -R ./balajitechlabs-illustrations "${CODEX_HOME:-$HOME/.codex}/skills/"
```

---

## Usage examples

### Plan illustrations only

```text
Use $balajitechlabs-illustrations to plan only, do not generate images yet.
Analyze this article and output about 5 shot list items.
Each item should include the placement, theme, core idea, structure type, Xiaohei action, suggested elements, and suggested Chinese labels.

<insert article>
```

### Generate article illustrations

```text
Use $balajitechlabs-illustrations to generate 4 Xiaohei-style article illustrations for this article.
Requirements: 16:9 horizontal, pure white background, black hand-drawn line art, sparse red/orange/blue Chinese handwritten annotations.
Each image should explain only one core structure. Do not make a PPT-style infographic.

<insert article>
```

### Single concept illustration

```text
Use $balajitechlabs-illustrations to generate one 16:9 article illustration for the concept:

Trust is not shouted. It is laid down piece by piece as evidence.

Make the image absurd but clean. Xiaohei must perform the core action.
Use at most 5 short Chinese labels.
```

---

## Notes

- Example images in `examples/images/` are for style calibration only.
- Do not directly copy the old examples' compositions.
- After generation, check the image for white background, whitespace, Xiaohei action, and readable Chinese labels.
- If many Chinese label errors appear, reduce labels and regenerate.
