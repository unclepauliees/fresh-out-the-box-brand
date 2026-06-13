# Fresh Out The Box — Typography System

Both typefaces are available on Google Fonts. Everything in this repo renders without licensing.

---

## Typefaces

### Display / Editorial: Syne

**Google Fonts:** `Syne` — [fonts.google.com/specimen/Syne](https://fonts.google.com/specimen/Syne)
**Load string:** `?family=Syne:wght@400;500;600;700;800&display=swap`

Syne is a geometric display sans-serif designed by Bonjour Monde. It has a distinctive optical character that reads as contemporary fashion without defaulting to cold minimalism. Its unusual but legible letterforms occupy the same territory as typefaces used by Acne Studios, Toteme, and The Row — recognisably fashion, without the overuse that now follows Playfair Display. No italic variant exists in the family; see Manrope below for italic uses.

**Weights in use:**
- Regular (400) — navigation labels, kickers, metadata at display size
- Medium (500) — H3 sub-headings, component headers
- SemiBold (600) — H2 section headings, product names
- Bold (700) — H1 page headings, logotype
- ExtraBold (800) — hero display, campaign headlines only

### Body / UI: Manrope

**Google Fonts:** `Manrope` — [fonts.google.com/specimen/Manrope](https://fonts.google.com/specimen/Manrope)
**Load string:** `?family=Manrope:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,500&display=swap`

Manrope is a humanist geometric sans-serif with a genuinely warm character. Its rounded letterforms and open apertures make it readable for women in fatigue — a practical accessibility concern for this audience, not merely an aesthetic one. Manrope has true italic variants (not browser-obliqued), which makes it the correct choice for all italic uses — pull quotes, editorial taglines, and emphasis — where Syne cannot serve.

**Weights in use:**
- Light (300) — taglines, small captions, metadata, packaging secondary text
- Regular (400) — body copy, UI labels, navigation
- Medium (500) — sub-headers, emphasis within body
- SemiBold (600) — CTAs, button labels, short product claims

---

## Type Scale

All sizes given in pixels for digital / rem equivalents noted. Print specs in points.

| Level | Element | Typeface | Weight | Size (px) | Line Height | Letter Spacing | Notes |
|---|---|---|---|---|---|---|---|
| Display | Hero headline | Syne | 800 | 64–72 | 1.05 | 0 | Homepage, campaign hero only |
| H1 | Page title | Syne | 700 | 48 | 1.1 | 0 | One per page |
| H2 | Section heading | Syne | 600 | 36 | 1.15 | 0 | |
| H3 | Sub-section | Syne | 500 | 26 | 1.2 | 0 | |
| H4 | Component title | Manrope | 600 | 18 | 1.3 | 0.02em | Uppercase option: letter-spacing 0.1em |
| Body Large | Intro copy | Manrope | 400 | 18 | 1.6 | 0 | First paragraph of any long-form section |
| Body | Standard copy | Manrope | 400 | 16 | 1.65 | 0 | Primary reading size |
| Body Small | Supporting copy | Manrope | 400 | 14 | 1.6 | 0 | Use sparingly; check contrast at this size |
| Label | UI labels, badges | Manrope | 500 | 12 | 1.4 | 0.08em | Uppercase only at this size; always use Medium+ |
| Caption | Photo captions, metadata | Manrope | 300 | 11–12 | 1.5 | 0.04em | Off-Black only; Warm Stone fails AA at this size |
| Quote | Featured testimonials | Manrope | 400 Italic | 24–28 | 1.4 | 0 | Manrope italic; Syne has no native italic |
| Wordmark | Logo text | Syne | 700 | — | — | 0.15em | Logo: fixed — do not rescale letters independently |

---

## Typographic Rules

### Hierarchy
Use Syne only for display/editorial moments and structural headings. The split between Syne (geometric, fashion-coded) and Manrope (warm, readable) creates the brand's visual tension — contemporary and forward-facing, but never cold. Mixing them in the same paragraph is wrong.

### Italic Uses
Syne has no italic variant. All italic text — pull quotes, taglines, editorial callouts — uses Manrope italic. Do not rely on browser-generated oblique for any italic context; always load the Manrope italic weights explicitly.

### Tracking (Letter Spacing)
Syne at large sizes (H1–H2): no tracking. The letterforms already have natural visual rhythm.
Manrope at small sizes (Label, Caption): positive tracking (0.06–0.1em). This is the standard rule for humanist sans at small sizes — tracking prevents crowding.
Manrope UPPERCASE: always add tracking ≥ 0.08em. Uppercase without tracking reads as shouting.

### Line Length
Body copy: 65–75 characters per line (approximately 550–640px at 16px / 400). Wider than this causes eye fatigue — a real concern for this audience.

### Font Loading
Use `font-display: swap` on all Google Fonts loads. This prevents invisible text during load — particularly important for older browsers and slow connections that may affect the primary audience (40–65 demographic).

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Syne:wght@400;500;600;700;800&family=Manrope:ital,wght@0,300;0,400;0,500;0,600;1,300;1,400;1,500&display=swap" rel="stylesheet">
```

### CSS Custom Properties

```css
:root {
  /* Typefaces */
  --font-display: 'Syne', 'Helvetica Neue', Arial, sans-serif;
  --font-body: 'Manrope', 'Helvetica Neue', Arial, sans-serif;

  /* Scale */
  --type-display: clamp(48px, 7vw, 72px);
  --type-h1: clamp(36px, 5vw, 48px);
  --type-h2: clamp(26px, 3.5vw, 36px);
  --type-h3: clamp(20px, 2.5vw, 26px);
  --type-h4: 18px;
  --type-body-lg: 18px;
  --type-body: 16px;
  --type-body-sm: 14px;
  --type-label: 12px;
  --type-caption: 11px;

  /* Line heights */
  --leading-tight: 1.1;
  --leading-editorial: 1.2;
  --leading-body: 1.65;
  --leading-loose: 1.8;
}
```

---

## Do Not Use

- **Helvetica, Arial, or any system geometric sans as primary display font** — fallback only
- **Fake oblique Syne** — Syne has no italic; if italic is needed, use Manrope italic
- **Syne below 16px** — this is a display face; do not use it for body text
- **All-caps Manrope below 12px** — legibility degrades for the 40–65 audience
- **More than two weights of either typeface on one surface** — keep hierarchy legible

---

## Print Specifications

For clinic one-pagers, packaging inserts, and any offset/digital print:

| Digital | Print equivalent |
|---|---|
| 72px | 54pt |
| 48px | 36pt |
| 36px | 27pt |
| 18px | 13.5pt |
| 16px | 12pt |
| 14px | 10.5pt |
| 11px | 8pt (minimum) |

Minimum body text for print: 10pt (Manrope Regular). Below this, legibility fails for the 40–65 primary audience, many of whom may be experiencing treatment-related visual fatigue.
