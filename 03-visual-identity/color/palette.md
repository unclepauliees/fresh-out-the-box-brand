# Fresh Out The Box — Color Palette

The palette is warm without being soft, sophisticated without being cold. It lives in the world of fashion editorial — think a well-shot lookbook, not a wellness app or a medical pamphlet. Every color has a role and a constraint.

---

## Primary Colors

These two colors do the heaviest structural work. They appear on everything.

### Espresso
```
Hex:  #1E1510
RGB:  30, 21, 16
CMYK: 0, 30, 47, 88
HSL:  22°, 31%, 9%
```
Use for: logotype, all body text, headings, primary dark backgrounds, footers.
Character: A warm near-black with a brown undertone. Does not read as corporate graphite or flat black — it has heat. Pairs with everything in the palette.

### Crème
```
Hex:  #F5EDE3
RGB:  245, 237, 227
CMYK: 0, 3, 7, 4
HSL:  30°, 47%, 93%
```
Use for: primary background, white-equivalent in all contexts, email backgrounds, card surfaces.
Character: A warm ivory. Clean enough to carry text and imagery; warm enough to feel like paper rather than screen. Never use true white (#FFFFFF) as a brand background — it reads cold and clinical.

---

## Secondary Colors

Supporting color with specific roles. None of these should dominate — they accent.

### Cognac
```
Hex:  #B8713F
RGB:  184, 113, 63
CMYK: 0, 39, 66, 28
HSL:  26°, 49%, 48%
```
Use for: decorative elements, large headlines on Crème backgrounds (≥18.66px bold or 24px regular), large badges, icon fills, photography prop color.
**Accessibility note:** Cognac text on Crème = 3.42:1 — passes WCAG AA for large text only. Do NOT use for body copy or small UI labels.
Espresso text on Cognac background = 4.70:1 — passes AA for normal text. This is the correct pairing when Cognac is a background.

### Cognac Deep
```
Hex:  #8B5230
RGB:  139, 82, 48
CMYK: 0, 41, 65, 45
HSL:  25°, 49%, 37%
```
Use for: CTA button backgrounds (with Crème or white text), hover state for Cognac elements, links over light backgrounds.
**Accessibility note:** White/Crème on Cognac Deep = 5.97:1 ✓ — passes AA for normal text. This is the text-safe CTA pairing.

### Blush
```
Hex:  #D4A59E
RGB:  212, 165, 158
CMYK: 0, 22, 25, 17
HSL:  6°, 37%, 73%
```
Use for: soft background panels, quote callout backgrounds, subtle illustration fills, warmth accents.
**Accessibility note:** Espresso on Blush = 8.49:1 ✓✓ — passes AA for all text sizes. Blush can carry body copy if Espresso is used.

### Sage
```
Hex:  #7A8E6E
RGB:  122, 142, 110
CMYK: 14, 0, 23, 44
HSL:  103°, 13%, 49%
```
Use for: badge backgrounds (with Espresso text), subtle borders, supportive accents, sustainability/material callouts.
**Accessibility note:** Espresso on Sage = 5.29:1 ✓ — passes AA for normal text. White on Sage = 3.48:1 — fails normal text; use Espresso only.

### Warm Sand
```
Hex:  #C9B49A
RGB:  201, 180, 154
CMYK: 0, 10, 23, 21
HSL:  32°, 28%, 70%
```
Use for: section dividers, input field borders, illustration mid-tones.
**Accessibility note:** Mid-tone only. Warm Stone text over Warm Sand fails normal text. Use Espresso for any text over Sand backgrounds.

---

## Functional Neutrals

### Off-Black
```
Hex:  #2C2420
RGB:  44, 36, 32
CMYK: 0, 18, 27, 83
HSL:  18°, 16%, 15%
```
Use for: body text (primary), long-form copy. Slightly softer than Espresso for extended reading.
**Accessibility note:** Off-Black on Crème = 13.8:1 ✓✓ — excellent for all body text.

### Parchment
```
Hex:  #E8DDD0
RGB:  232, 221, 208
CMYK: 0, 5, 10, 9
HSL:  31°, 28%, 86%
```
Use for: card backgrounds, product tile backgrounds, subtle section differentiation from Crème.

### Warm Stone
```
Hex:  #8C7E74
RGB:  140, 126, 116
CMYK: 0, 10, 17, 45
HSL:  22°, 10%, 50%
```
Use for: secondary labels, captions (large size ≥14px), inactive states. 
**Accessibility note:** Warm Stone on Crème = 3.32:1 — fails normal text AA. For captions smaller than 18.66px bold or 24px regular, use Off-Black instead. Warm Stone is approved only for decorative labels, large-type captions, and secondary metadata.

---

## Text-Safe Pairings (Computed Contrast Ratios)

| Text Color | Background | Contrast Ratio | Normal Text | Large Text |
|---|---|---|---|---|
| Espresso #1E1510 | Crème #F5EDE3 | **16.1:1** | ✓ AAA | ✓ AAA |
| Off-Black #2C2420 | Crème #F5EDE3 | **13.8:1** | ✓ AAA | ✓ AAA |
| Crème #F5EDE3 | Espresso #1E1510 | **16.1:1** | ✓ AAA | ✓ AAA |
| Espresso #1E1510 | Cognac #B8713F | **4.70:1** | ✓ AA | ✓ AA |
| Crème #F5EDE3 | Cognac Deep #8B5230 | **5.97:1** | ✓ AA | ✓ AA |
| Espresso #1E1510 | Sage #7A8E6E | **5.29:1** | ✓ AA | ✓ AA |
| Espresso #1E1510 | Blush #D4A59E | **8.49:1** | ✓ AA | ✓ AA |
| Espresso #1E1510 | Parchment #E8DDD0 | **11.9:1** | ✓ AAA | ✓ AAA |
| Cognac #B8713F | Crème #F5EDE3 | **3.42:1** | ✗ | ✓ AA |
| White #FFFFFF | Cognac #B8713F | **3.92:1** | ✗ | ✓ AA |
| Warm Stone #8C7E74 | Crème #F5EDE3 | **3.32:1** | ✗ | ✓ AA |

**Rule:** Body copy = Espresso or Off-Black on Crème/Parchment/Blush. Mid-tones (Cognac, Sage, Warm Stone) are decorative or large-text-only unless paired with Espresso as text.

---

## Color Usage Ratios

For brand consistency across touchpoints, target these rough usage ratios:

| Color | Approximate Usage |
|---|---|
| Crème | 50–60% (backgrounds, white space) |
| Espresso | 15–20% (text, marks, dark accents) |
| Cognac / Cognac Deep | 8–12% (key accents, CTAs) |
| Blush | 8–10% (warmth fills, secondary panels) |
| Sage | 4–6% (badges, grounding) |
| Warm Sand + Parchment | 8–12% (supporting neutrals) |

If you find Cognac taking up more than 15% of a surface, reassess — it risks looking like a different, warmer brand.

---

## Colors to Avoid

- **True white (#FFFFFF):** Too cold for this brand. Use Crème.
- **True black (#000000):** Slightly harsh. Use Espresso (with a rare exception for one-color print production where pure black is required).
- **Pink in any register:** Pink ribbon associations are category wallpaper. Blush is the closest we get, and it reads as a warm neutral, not a breast cancer awareness color.
- **Hospital/medical blues or teals:** These read as clinical and undermine the fashion positioning in every context.
- **Saturated purples:** Often read as oncology-adjacent in American visual culture.
