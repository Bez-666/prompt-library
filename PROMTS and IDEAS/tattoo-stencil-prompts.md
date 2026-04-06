# Tattoo Stencil Prompts

A collection of image-to-stencil prompts for generating transfer-ready tattoo outlines using AI image generators.

---

## 1. Universal Tattoo Stencil Prompt
*Works with Midjourney, Stable Diffusion, DALL-E, and most image generators.*

```
Convert this image into a clean tattoo stencil outline. Pure black bold lines on a solid white background. No gray tones, no shading, no gradients, no color — strictly black and white only. Extract all edges, contours, and defining shapes as precise, clean ink lines. Line weight should be consistent and bold enough to be transfer-ready. Remove all texture, photographic detail, and background noise. The result should look like a professional hand-drawn outline ready to be printed as a thermal tattoo stencil transfer. Style: linework illustration, minimal, flat, high contrast.
```

### Generator-Specific Tips

**Midjourney:** Add `--style raw --no shading, color, gradient, texture` at the end.

**Stable Diffusion** — Use as a negative prompt:
```
(color, shading, gray, gradient, texture, background, photo, realistic, 3d)
```

**DALL-E / GPT Image:** Prefix with `"Transform the uploaded image into..."` then paste the prompt above.

---

## 2. Nano Banana Stencil Prompt
*Optimized for the nano_banana model.*

```
A professional tattoo stencil of [YOUR SUBJECT HERE]. Pure black bold outlines on a solid white background. No shading, no gray tones, no color, no gradients, no fill. Clean precise linework only, capturing all contours, edges, and defining shapes of the subject. Lines are thick enough to be stencil-ready. Background is completely white. Style: tattoo flash linework, high contrast black and white outline illustration, transfer-ready stencil.
```

Replace `[YOUR SUBJECT HERE]` with your subject. Examples:
- `A tattoo stencil of a wolf howling at the moon`
- `A tattoo stencil of a traditional Japanese dragon`
- `A tattoo stencil of a skull with roses`

> **img2img tip:** Upload a reference photo and the model will base the outline directly off it.

---

## 3. Tonal Stencil Prompt (Light/Dark Mapping)
*Creates a stencil that shows where ink should be heavy, medium, or absent — transfer-ready with full tonal guidance.*

```
A professional tattoo stencil of [YOUR SUBJECT HERE]. Black and white only, no color. Convert all shadows and dark areas into solid black fill or dense stippling/crosshatching. Convert all midtones into medium dot clusters or fine crosshatch lines. Leave highlights and lightest areas as clean white space. The result should clearly show where ink is heavy (dark regions), where ink is light (sparse lines or dots), and where skin shows through (white). Bold clean outlines define all edges and contours. Transfer-ready stencil style. High contrast. No gray washes — all tones must be represented through linework, stippling, or solid black fill only. Style: tattoo flash tonal illustration, dotwork shading map, stencil-ready.
```

### Tonal Zone Reference

| Area | Stencil Representation |
|---|---|
| Deep shadows | Solid black fill |
| Midtones | Crosshatching or dense stippling |
| Light areas | Sparse dots or fine lines |
| Highlights | Pure white (skin shows through) |

> **Best used with img2img** — upload a photo and the model reads existing light/shadow to map tonal zones automatically.
