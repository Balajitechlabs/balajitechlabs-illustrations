# Raw Image Prompt Template

Generate each image separately. Replace the variables with content from the article. Do not combine multiple images into one.

```text
Generate one standalone 16:9 horizontal Chinese article illustration.

Visual DNA:
Pure white background. Minimalist black hand-drawn line art. Slightly wobbly pen strokes. Lots of empty white space. Sparse red/orange/blue handwritten Chinese annotations. Clean absurd product-sketch feeling. No gradients, no shadows, no paper texture, no complex background, no commercial vector style, no PPT infographic look, no cute mascot poster, no children's illustration, no realistic UI.

Recurring IP character required:
Xiaohei, a small solid-black absurd creature with white dot eyes, tiny thin legs, blank serious expression, and a slightly uneven hand-drawn body. Xiaohei must perform the core conceptual action, not decorate the scene. Make Xiaohei serious, deadpan, and slightly bizarre, not cute.

Theme:
{article illustration theme}

Structure type:
{structure type: Workflow / system segment / before-after contrast / role states / concept metaphor / layered method / route map / mini comic storyboard}

Core idea:
{the core meaning this image should convey}

Composition:
{specific scene: where Xiaohei is, what Xiaohei is doing, main objects, how information flows}

Suggested elements:
{element1} / {element2} / {element3} / {element4}

Chinese handwritten labels:
{label1} / {label2} / {label3} / {label4} / {optional label5}

Color use:
Black for the main line art and Xiaohei. Orange for the main flow/path/arrows. Red only for key warnings/problems/results. Blue only for secondary notes, feedback, or system state.

Constraints:
One image explains only one core structure. Keep the main subject around 40%-60% of the canvas. Preserve at least 35% blank white space. Use at most 5-8 short handwritten Chinese labels. Do not write a title in the top-left corner. Do not write the structure type on the image. Do not make it a formal diagram, course slide, or dense explainer. Do not copy prior examples or reuse known case compositions unless explicitly requested; invent a fresh visual metaphor for this specific article. It should be clear but not instructional, interesting but not childish, strange but clean.
```

## Image editing prompt

Remove the top-left title:

```text
Edit the provided image. Remove only the handwritten title "{text to remove}" and its underline from the top-left corner. Fill that area with the same clean white background, matching the surrounding blank paper. Preserve everything else exactly: characters, labels, paths, line style, composition, aspect ratio, and image quality. Do not add any new text or objects.
```

Enhance absurdness:

```text
Regenerate this illustration with the same core meaning and simple layout, but make Xiaohei more central to the conceptual action. Xiaohei should be doing the strange work that explains the idea, not standing beside the diagram. Keep it clean, sparse, hand-drawn, and not cute.
```
