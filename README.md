# Fresh Out The Box — Brand Identity Kit

Complete, production-ready brand identity. Every file is usable today. This README explains what's here, how to use it, what needs a human designer's pass, and the three decisions most worth pressure-testing with the founder.

---

## What's Here

```
fresh-out-the-box-brand/
├── 01-strategy/
│   ├── brand-platform.md          Purpose, vision, mission, values, positioning,
│   │                              promise, personality sliders, tagline options
│   ├── audience-personas.md       5 detailed personas with mindsets, trigger moments,
│   │                              and messages that land vs. wound
│   └── messaging-architecture.md  Brand idea → 3 pillars → proof points → sample
│                                  copy per pillar per audience
│
├── 02-verbal-identity/
│   ├── voice-and-tone.md          4 voice principles + tone flexed across 5 contexts
│   │                              (product page, first-shed email, social, clinic,
│   │                              customer service)
│   ├── copy-bank.md               20 headlines, 10 product descriptions, 5 founder
│   │                              story excerpts, packaging copy, unboxing insert
│   └── lexicon.md                 Words we use / words we never use, with rationale
│
├── 03-visual-identity/
│   ├── logos/
│   │   ├── fotb-primary.svg           Horizontal lockup (full color)
│   │   ├── fotb-primary-black.svg     One-color black
│   │   ├── fotb-primary-white.svg     Reverse on dark background
│   │   ├── fotb-stacked.svg           Stacked lockup (full color)
│   │   ├── fotb-stacked-black.svg     Stacked one-color black
│   │   ├── fotb-stacked-white.svg     Stacked reverse
│   │   ├── fotb-mark.svg              Halo mark (full color)
│   │   ├── fotb-mark-black.svg        Halo mark (black)
│   │   └── fotb-mark-white.svg        Halo mark (reverse)
│   ├── color/
│   │   ├── palette.md             All hex/RGB/CMYK values, usage ratios, computed
│   │   │                          WCAG contrast ratios, text-safe pairing matrix
│   │   └── swatches.svg           Visual swatch reference sheet
│   ├── typography/
│   │   └── type-system.md         Playfair Display + DM Sans specs, full type scale
│   │                              (Display → Caption), CSS custom properties, print
│   │                              equivalents, Google Fonts load strings
│   ├── photography-art-direction.md  5 shot briefs with explicit representation
│   │                                 requirements, editing direction, what never appears
│   └── iconography/
│       ├── icon-comfort.svg
│       ├── icon-breathable.svg
│       ├── icon-remy-hair.svg
│       ├── icon-modular.svg
│       ├── icon-put-on-go.svg
│       ├── icon-hsa-fsa.svg           Labeled "may be eligible" — never promissory
│       ├── icon-bamboo-lining.svg
│       ├── icon-adjustable.svg
│       ├── icon-washable.svg
│       └── icon-scalp-safe.svg
│
├── 04-applications/
│   ├── packaging-direction.md     Full unboxing spec: box construction, interior lid
│   │                              copy, tissue, insert card, gift box, shipping carton
│   │                              (with discreet-default shipping direction)
│   ├── social-templates/
│   │   ├── quote-card.html        1:1 Instagram format (edit blockquote + attribution)
│   │   ├── product-card.html      4:5 product showcase (replace placeholder image)
│   │   └── founder-story-card.html  1:1 Blush ground (see inline compliance warnings)
│   ├── email-header.svg           600×160px email header, Espresso ground
│   └── clinic-one-pager.html      Print-ready letter-size, for patient navigators
│                                  and boutique partners — includes hedged reimbursement
│                                  language and wholesale contact
│
├── 05-guidelines/
│   └── index.html                 THE FLAGSHIP — complete brand guidelines as a
│                                  polished single-page microsite. All logos embedded
│                                  inline. Live swatches. Computed contrast ratios.
│                                  Real do/don't copy pairs. Photography direction.
│                                  Compliance guardrails with review checklist.
│
└── README.md                      This file
```

---

## How to Use This Kit

### Viewing the Guidelines
Open `05-guidelines/index.html` in any modern browser. All fonts load from Google Fonts — requires an internet connection. This is the single source of truth for any designer, writer, or agency partner working on this brand.

### Using the Logos
The SVG logos use `font-family` references to Playfair Display (loaded from Google Fonts). They render correctly:
- When embedded **inline** in HTML (recommended for all web uses)
- When opened directly in Chrome, Firefox, or Safari (fonts load via `@import` in the SVG style block)
- When placed as `<img src>` tags — fonts will **not** load; only the geometric halo arc will render

For print, embroidery, laser engraving, or any non-browser use: the wordmark letterforms must be **outlined to paths** by a production designer before delivery. See the guidelines for the specification.

### Using the Social Templates
Open any template in a browser. Edit the clearly marked `<!-- EDIT HERE -->` sections. Screenshot or export via headless browser (Puppeteer, Playwright) at 1080×1080px for Instagram square or 1080×1350px for 4:5 format. Read the inline instructions panel in each template before publishing.

### Using the Clinic One-Pager
Open `clinic-one-pager.html` in a browser. File → Print (or Cmd/Ctrl+P) → Save as PDF → Letter size, no margins. The `@media print` styles activate automatically. The reimbursement language is pre-hedged to the correct standard.

### Icons
All icons are 24×24 SVGs. Change `stroke="#1E1510"` to any brand color. Scale by changing `width` and `height` attributes while keeping the `viewBox`. Do not use these icons as standalone imagery without label text — they support copy, not replace it.

---

## Three Decisions Most Worth Pressure-Testing With the Founder

### 1. The tagline alternatives
The kit proposes two alternatives alongside the incumbent:
- **Current:** "Restoring confidence, one hat at a time."
- **Option B:** "The hat. The hair. The you." (recommended for testing)

Option B compresses the brand promise into a form with stronger recall and word-of-mouth potential. But it's a departure from the incumbent, and that decision belongs to the founder. Recommendation: run both in an A/B on the website hero for one quarter and measure time-on-page, social share rate, and direct quotes in customer reviews.

### 2. The halo mark vs. a wordmark-only approach
The halo mark (the 320° arc) is the brand's most distinctive visual asset — it works as a favicon, a branded seal, an embroidery patch, a foil stamp. But any mark requires consistency and protection to build recognition. The question for the founder: is the brand at a scale where it can commit to building mark recognition, or should it lean wordmark-only for now and introduce the mark gradually? The kit is built for both paths; this is a resourcing and timeline decision, not a design quality question.

### 3. The discreet shipping default
The packaging direction recommends that **discreet exterior packaging (no brand name on the shipping box) be the default**, with opt-in for branded exterior. This is a privacy-first decision built around the primary customer's reality: many women receiving these orders are at workplaces or in shared households and may not have disclosed their medical situation. This recommendation is correct for the audience but should be confirmed by the founder — some brands build equity from visible shipping; others protect customers first. There is no wrong answer, but it's a deliberate choice.

---

## What Needs a Human Designer's Pass Before Production

### Priority 1: Outline the logotype letterforms
The SVG logos use live text references. Before the logotype is used in print, embroidery, packaging dielines, or any non-browser context, a type designer or production designer must:
1. Confirm Playfair Display is appropriate (no foundry conflicts with the specific version used)
2. Optically space the wordmark letterforms for the brand's specific use case (letter-spacing in CSS/SVG is uniform; optical spacing is not)
3. Convert all text to outlined paths

### Priority 2: Trademark screening of the wordmark
"FRESH OUT THE BOX" as a wordmark should be screened by a trademark attorney before filing or committing to the name at scale. The phrase is a common idiom — screening for likelihood of confusion in Class 25 (clothing/headwear) and Class 44 (medical services/products) is essential. Budget approximately $800–1,500 for a clearance search.

### Priority 3: A custom photography shoot with the specific representation brief
The photography direction in this kit is specific enough to brief a photographer today. The brand's visual credibility depends entirely on executing it well — particularly the coily/curly texture representation and the active-treatment lifestyle shots. A poorly shot set of images will undermine every other quality decision in this kit. A day rate of $2,500–5,000 for a brand photographer plus a half-day rate for a stylist is the minimum investment for this to land. Stock photography is not an acceptable substitute.

---

## On Voice and Compliance

Every piece of copy in this kit has been cleared against the banned-language list in `02-verbal-identity/lexicon.md`. When writing new content, run it against that list before publishing. The self-critique checklist in `05-guidelines/index.html` (Sensitivity & Compliance section) is a one-minute review process — use it every time.

HSA/FSA language in this kit is consistently hedged: "may be eligible," "verify with your plan administrator." Do not alter this language to be more promissory. It is not a marketing conservatism — it is an accuracy requirement.

---

## Technical Notes

- All fonts: Google Fonts (Playfair Display, DM Sans). No licensing required for web and screen use. For print production, confirm font license covers commercial print via the SIL Open Font License under which both are distributed.
- All colors are specified in hex, RGB, and CMYK in `03-visual-identity/color/palette.md`. CMYK values are approximate conversions — a production designer should pull Pantone equivalents for spot-color print applications.
- All SVG icons are `fill="none"` stroke-based, `stroke="#1E1510"`, `stroke-width="1.5"`, `viewBox="0 0 24 24"`. They are accessible: each includes a `<title>` element and `role="img"` `aria-label`.
- The clinic one-pager uses CSS Grid — it renders correctly in Chrome, Firefox, Safari, and Edge. It does not require any external dependencies. Print output has been designed for standard US Letter at zero margins.
