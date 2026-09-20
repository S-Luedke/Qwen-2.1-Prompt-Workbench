# Qwen 2.1 Prompt Workbench

69 fill-in prompt templates for **Qwen-Image-2.1**, grouped by task, as a single self-contained page.

**→ [Open the workbench](https://s-luedke.github.io/Qwen-2.1-Prompt-Workbench/)**

Edit any field and the finished prompt below it recomposes live, then copy it straight into your UI.
Search, filter by reference-image count, and a category rail. Your edits are remembered in your
browser. No build step, no dependencies, no server — one 83 KB HTML file that also works offline.

## Categories

Text to Image · Text & Typography · Transparent/RGBA · Single-Image Edit · Editing Text In An Image ·
Portrait & People · Style & Medium · Local/Marked-Region Edit · **Multi-Image Composition** ·
Panorama, Infographic & Storyboard

## Working with reference images

`<image1>`, `<image2>` … are literal tags the model reads. They map to reference images in the order
you add them, up to 10, and `<image1>` is the edit target — the output follows its framing.

Three things that matter more than any setting:

- **Name every reference you rely on.** An unmentioned `<image2>` conditions far more weakly.
- **Say what must not change.** "keep the face, hair and pose unchanged" is the single most useful
  clause in edit prompts.
- **Match the output aspect ratio to `<image1>`**, or the edit drifts out of frame.

## Settings

The official ComfyUI templates ship 25 steps, CFG 1, euler / simple. Qwen's own repository uses
about 40–50 steps with euler instead; more advanced solvers need fewer. CFG stays at 1 on the
official path, which means the negative prompt is unused. Resolution is 1 MP by default and the
model supports up to native 2K — prefer multiples of 32.

## Files

| File | What it is |
|---|---|
| `index.html` | the workbench, self-contained |
| `templates.json` | the same 69 templates as data, with fields, defaults and reference counts |

## Note on licensing

Qwen-Image-2.1 is released under the **Qwen Research License Agreement**, which permits research and
evaluation only. Commercial use needs a separate licence from the model's authors. The template text
in this repository is original and freely usable; the model it targets is not.

## Sources

[Qwen-Image-2.1 Space](https://huggingface.co/spaces/Qwen/Qwen-Image-2.1) ·
[QwenLM/Qwen-Image-2.1](https://github.com/QwenLM/Qwen-Image-2.1) ·
[ComfyUI docs](https://docs.comfy.org/tutorials/image/qwen/qwen-image-2-1)
