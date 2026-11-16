# Tinkomi Geometric Flow

Reusable visual system for blog hero illustrations and supporting product screenshots.

## Hero image standard

- Master canvas: 1600 × 900 px, landscape 16:9.
- Preferred web format: WebP, target under 250 KB when practical.
- Palette: ink navy `#091630`, cobalt `#1769FF`, warm mint `#76EBC8`, soft blue `#DCE9FF`.
- Use one restrained, abstract geometric motif that represents the article topic.
- Keep the essential motif within the central 55% of the canvas and leave crop-safe outer margins.
- No title, text, letters, numbers, logos, watermarks, people, device mockups, charts with invented values, or simulated product UI.
- Keep the article title as HTML text, not embedded in the image.

## Product evidence

AI-generated images are concept illustrations only. When a post needs to demonstrate a real feature, capture a genuine screenshot from the public demo and label it as a product screenshot. Never present generated UI as the actual application.

## File naming

- Hero illustration: `[post-slug]-hero.webp`
- Genuine UI screenshot: `[post-slug]-ui-01.png`

## Accessible descriptions

- Concept illustration: describe the abstract idea briefly.
- Product screenshot: describe only the visible feature and state.
- Pure decoration that repeats nearby text may use empty alt text (`alt=""`).
- Add a caption only when useful; clearly distinguish a concept illustration from an application screenshot.

## Reusable image prompt

Replace only `[TOPIC]` and `[MOTIF]`:

```text
Create one premium editorial cover illustration for
Tinkomi | Practical Software Tools.

Topic: [TOPIC]
Central abstract motif: [MOTIF]

Use the established Tinkomi Geometric Flow visual identity:
- Landscape 16:9 composition, target 1600x900
- Deep ink navy background (#091630)
- Bold cobalt blue (#1769FF)
- Warm mint accents (#76EBC8)
- Occasional soft blue highlights (#DCE9FF)
- Refined 2D vector-style geometric illustration
- Clean modular shapes, subtle pixel motifs,
  carefully balanced negative space
- One coherent central geometric composition
- Keep essential artwork in the central 55% width
- Keep generous margins for mobile center crops
- High contrast and consistent visual hierarchy
- Professional, friendly indie software-tool aesthetic
- Minimal, timeless, not flashy

Strict exclusions:
No text, words, letters, numbers, labels, typography,
logos, watermarks, photographs, people, device mockups,
charts with fake values, browser windows, fake screenshots,
invented UI, code text, decorative clutter, or visual noise.

The artwork must communicate the topic through abstract
forms only. It must not pretend to show the actual product
interface.
```
