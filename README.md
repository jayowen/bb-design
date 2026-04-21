# Business Builders — Design System

> Marketing-agency brand system. StoryBrand-certified, HubSpot Platinum, Inc. 5000.
> Tagline: **"Clear message. Proven strategy. Real growth."**

This folder is the single source of truth for building branded Business Builders
artifacts: slides, landing pages, pitch decks, social posts, proposals, and
in-product UI. Every color, font, shadow, and component here comes from the
official 2025 Brand Guide and the live StoryBrand marketing site.

---

## Index

| File / folder | What it contains |
|---|---|
| `colors_and_type.css` | CSS variables for color, type, spacing, shadows, motion. Import this first. |
| `assets/` | Raw logos (primary lockup, mark, light/dark variants). |
| `preview/` | Small HTML cards that populate the Design System tab (type specimens, color swatches, component states). |
| `ui_kits/website/` | React/JSX recreation of the marketing site — hero, growth stack, industries grid, success stories, process, footer. Open `index.html` for the interactive demo. |
| `slides/` | 16:9 slide templates (title, section, big-quote, stat, comparison) in the BB visual language. |
| `SKILL.md` | Drop-in Agent Skill so Claude Code / any agent can use this system. |
| `README.md` | You are here. |

### Source materials
- `uploads/Brand Guide 2025 - Business Builders .pdf` — the official guide (logos, clear space, color, type, application mockups).
- `uploads/Marketing Agency Business Growth Experts StoryBrand Agency.pdf` — full scroll capture of the live marketing site (hero, 4-pillar growth stack, industries, success stories, process, footer).
- `uploads/Business-Builders-Logo-Versions (1)-01.png` — primary lockup.
- `uploads/IMG_0267.png` — alt logo capture.

No codebase or Figma was attached; all recreations below are rebuilt from the
brand guide + live-site screenshots. If you have access to the production repo
or Figma library, drop it in and regenerate the UI kit for pixel-perfect parity.

---

## Company context

Business Builders is a full-service marketing agency. They position themselves
around the **StoryBrand framework** (clear message → proven strategy → real
growth) and bundle services into a **four-pillar "Growth Stack"**:

1. **PLAN** — Messaging, Video, Website, Marketing, AI blueprints
2. **PRODUCE** — Website dev, video production, photography, brand identity
3. **PROMOTE** — SEO, PPC, Social, CRM/HubSpot
4. **PROTECT** — Managed hosting, maintenance, ADA compliance, security

**Products represented in this system:**
- The **marketing website** (primary surface — recreated in `ui_kits/website/`).
- A **slide template system** for internal decks and client-facing pitches (in `slides/`).

Trust signals that recur across the brand: *StoryBrand Certified Agency*,
*HubSpot Platinum Partner*, *Inc. 5000 (2×)*, *26+ years*, *1000+ clients*.

---

## Content fundamentals

The voice is **direct, punchy, and operator-focused** — the reader is a busy
business owner who is frustrated with marketing that doesn't work. Copy is
written to relieve that frustration: name the problem, promise a plan, show
proof.

### Tone
- **Plain-spoken authority.** Short sentences. No jargon. No "synergy."
- **Problem → plan → outcome.** Classic StoryBrand. Every section follows it.
- **Confident, not loud.** Big claims are backed with numbers ("532% increase in
  site traffic"), logos, and named client quotes.
- **Warm where it counts.** Headlines bark; subheads use *italic serif* to
  soften and invite.

### Person
- **"You" and "we"** — never "the client," never "our customers."
- "We help **you** grow." "When **you** have the right team around you…"
- Collective "our team," "our process."

### Casing
- **ALL-CAPS** for display headlines and section titles. It's a brand signature.
- Eyebrow tags ("SUCCESS STORIES", "HOW WE HELP YOU GROW") are uppercase with
  wide tracking, set inside a black pill or yellow box.
- Body copy is **sentence case**. Never use title case for running text.
- Category badges ("WEB", "CASE STUDY", "VIDEO") are uppercase, bold, yellow.

### Headline pattern (very specific — use it)
Every hero/section headline follows one of these shapes:

1. **Three-beat rhythm** with one italic middle:
   *CLEAR MESSAGE. **PROVEN STRATEGY**. REAL GROWTH.*
2. **Two-line with one yellow emphasis word:**
   *GET A PLAN THAT **WORKS*** / *& a team you can trust*
3. **Problem statement with the payoff in yellow:**
   *STOP WASTING TIME & MONEY ON MARKETING THAT **DOESN'T WORK***

The highlight word is always in `--bb-yellow`. Often one word is also italicized
(adds energy and breaks the all-caps monotony).

### Supporting copy
- Descriptive subheads under big headlines: **italic Playfair-style serif**, gray.
  *"Every service you need to plan, build, promote, and protect your business —
  all under one roof."*
- Body paragraphs: Inter regular, `--fg-2` gray, 1.55 line-height, max ~60ch.

### Lists
- Feature lists always use **yellow circle-checkmark bullets** (never dots,
  never dashes). Three-to-five items per list — if you have more, split into a
  second column.

### Emoji
- **No emoji** in marketing copy. Ever. If you're tempted, use a monoline icon
  in a yellow-outlined box instead (see iconography below).

### CTA verbs
Short, action-first: *REQUEST A QUOTE*, *GET A FREE QUOTE*, *VIEW PROJECT*,
*EXPLORE SERVICES*, *VIEW ALL WORK*, *FREE MARKETING AUDIT*. All uppercase,
Poppins Bold, often with a trailing `→`.

---

## Visual foundations

### Colors
- **Primary accent:** `#FACC15` yellow. Used for highlight words, primary
  buttons, icon boxes, chips/badges, bullet checks, small square decorative
  tiles behind numbered step icons.
- **Primary dark:** `#1A1918` (not pure black — slightly warm). This is the
  default dark section background, button text on yellow, and the border color
  in the offset-shadow treatment.
- **Secondary dark:** `#111827` (navy). Used sparingly — alt dark surfaces.
- **Mid gray:** `#505050` for secondary UI and gradient stops.
- **White / off-white:** `#FFFFFF` and `#F7F5F2` — page and card backgrounds on
  light sections.
- **Gradients** (from the brand guide): yellow `#FACC15 → #F49E1C`, dark
  `#1A1918 → #505050`. Used mostly on application mockups and occasional hero
  treatments, never on small UI.

The page alternates **dark sections (black bg, white text)** with **light
sections (white/off-white bg, black text)**. Yellow is the constant through-line.

### Type
- **Poppins Bold/ExtraBold** for all headlines, eyebrows, buttons, badges —
  almost always uppercase.
- **Inter Regular** for body copy, labels, form fields, small print.
- **Playfair Display italic** (or any transitional serif italic) for subheads
  under big headlines and pull-quotes. This is the "warm" counter-weight to the
  heavy sans headlines. *Not in the official brand guide* — inferred from the
  live marketing site. If the team has a specific serif, swap `--font-serif`.
- Uppercase headlines get tight tracking (`-0.02em`) so they feel dense, not
  airy.

### Backgrounds
- **Solid color fills only** — no noise, no grain, no hand-drawn illustration,
  no repeating pattern. Photography is used full-bleed (teammates, clients,
  work mockups) but never behind text without a dark overlay.
- Dark sections = `--bb-black` flat. Light sections = `#FFFFFF` or `#F7F5F2`.
- Full-bleed imagery appears in case study cards and application mockups, not
  in general page chrome.

### The signature "offset shadow" treatment
Cards, CTAs, and feature blocks often use a **hard offset shadow**: a solid
black rectangle sitting 6–10px down-right of the element, no blur. This is
Business Builders' single most recognizable visual device.
```
box-shadow: 6px 6px 0 0 #1A1918;
```
Combined with a 1–2px black border, it gives the "paper sticker on a dark wall"
effect that appears on every service card, step card, and quote block.

### Standard card
- Square or very slightly rounded corners (`2–4px`, never more than `8px`).
- 1–2px `#1A1918` border.
- Hard offset shadow (see above) or a soft `--shadow-md` for interior UI.
- Generous padding: `24–32px` on mobile, `32–48px` on desktop.

### Protection gradient vs capsule
- **Eyebrow tags** = solid yellow box OR solid black pill, uppercase tracked
  text inside. The two alternate (yellow on dark sections, black on light
  sections).
- No frosted/blur chips. No glassmorphism.
- Transparency/blur is essentially unused — the brand is flat, graphic, high
  contrast.

### Buttons
- **Primary:** yellow fill, black text, square/2px radius, hard black offset
  shadow on hover-off and compressed on hover.
- **Secondary on dark:** black fill, yellow 2px border, white text, yellow
  underline on hover.
- **Outline:** transparent, 2px border, inherits fg color.
- Height ≥ 52px on desktop, 48px on mobile. Padding `16px 24px`.

### Hover / press states
- Buttons: on hover, background nudges to `--bb-yellow-deep` or reveals an
  underline. On press, the offset shadow collapses (shadow → 2px 2px) and the
  element translates 4px down-right — "button got pressed into the wall."
- Links in body: underline on hover, color unchanged.
- Cards: on hover, lift `translateY(-2px)` OR enlarge offset shadow from 6→10px.

### Iconography
See the Iconography section below.

### Corner radii
- Buttons, cards, badges: `0px` to `4px`. Never pill-shaped except for
  hero-eyebrow chips and avatars.
- Images in cards: `0px` (flush with the card edge).
- Circular avatars and step-number chips only when semantically "a person" or
  "a checkmark."

### Layout rules
- **12-column grid, 1200px max-width container**, 24px gutter, 64–96px vertical
  rhythm between sections.
- Dark and light sections alternate. Never two same-color sections in a row
  without a divider.
- Section headers are **centered**, anchored by a small eyebrow chip, headline,
  and italic-serif subhead — in that order.
- Fixed elements: the top navigation stays pinned on scroll, with a yellow
  "REQUEST A QUOTE" button always visible top-right.

### Motion
- **Fades and short translates, 200–360ms, ease-out.** Nothing bouncy.
- Scroll-triggered reveals stagger by 80ms.
- Button hovers: 120ms. Offset-shadow press: 160ms.
- No parallax, no confetti, no 3D. The brand reads as "no-nonsense operator."

### Transparency & blur
- Essentially unused. Overlays on photography are **solid dark 60–80% opacity**
  rectangles, not blurred surfaces.

### Imagery vibe
- Warm, natural, un-stylized. Real team members, real clients, real offices.
- Application mockups (t-shirts, business cards, building signage, phone
  screens) are photographed on neutral warm-gray backdrops.
- **No illustration, no isometric, no 3D renders.** Photos only.

---

## Iconography

Business Builders uses a **monoline, rounded, medium-stroke icon style** —
evergreen utility icons rendered inside a **yellow-outlined square box** on
dark sections, or a **solid yellow box with black icon** on light sections.

- **Closest open-source match: [Lucide](https://lucide.dev) at stroke-width 2.**
  The live site's industry icons (graduation cap, shopping bag, car, tooth,
  building, heart, hard hat, factory, stethoscope, sparkle) are all available
  in Lucide 1:1.
- **CDN-linked** in UI Kit examples: `https://unpkg.com/lucide@latest`. No icon
  font needed.
- **Placement pattern:** 56–72px yellow-bordered box, icon centered at 28–32px.
- **Color:** icon color matches the accent on the containing surface — yellow
  on dark bg, black on yellow bg.

⚠️ **Substitution flagged.** The brand guide does NOT specify an icon library.
Lucide is a best-visual-match substitution. If Business Builders has an
official icon set (custom SVGs, a Figma library, a proprietary font), please
drop them in `assets/icons/` and update the UI kit.

**Emoji:** never used.
**Unicode icons:** not used. `→` and `✓` are the only two unicode glyphs that
appear — `→` after CTA labels, `✓` as a bullet (but usually replaced with a
yellow circle-check Lucide icon).

**Logo assets** live in `assets/`:
- `logo-primary.png` — full lockup with anvil mark (dark on light)
- `logo-dark-on-light.png` — same as primary, explicit naming
- `logo-mark.png` — anvil-only mark

⚠️ **Missing assets:** The brand guide references a white-on-dark logo version
and a mark-only white version that weren't included in uploads. Please share
those when available.

---

## Font substitution notice

The brand guide calls for **Poppins Bold** (headlines) and **Inter** (body) —
both are already Google Fonts, so they're loaded directly in
`colors_and_type.css`, **no substitution needed**.

**Playfair Display** (italic serif for supporting copy) is my inference from
the live site — the marketing PDF shows a transitional serif italic that
matches Playfair's proportions closely. If the actual typeface is different
(Lora, Source Serif, a custom foundry face), swap `--font-serif` in the CSS.
Flagging so you can confirm.

---

## How to use

```html
<link rel="stylesheet" href="/path/to/colors_and_type.css" />

<div class="bb-root">
  <p class="bb-eyebrow" style="color: var(--bb-yellow)">STORYBRAND CERTIFIED AGENCY</p>
  <h1 class="bb-h1">
    CLEAR MESSAGE.
    <em style="font-style: italic">PROVEN STRATEGY.</em>
    <span class="bb-hl">REAL GROWTH.</span>
  </h1>
  <p class="bb-serif-italic">
    Get a team that leverages the latest in AI, combined with StoryBrand
    messaging, to help you grow.
  </p>
</div>
```

See `ui_kits/website/index.html` for a full working composition.

---

## Open questions for the team
1. Is there a production codebase or Figma library we can link to tighten the
   UI kit to pixel parity?
2. The serif used under hero headlines on the live site — is it Playfair
   Display, or a different face?
3. Do you have a canonical icon set (SVG sprite, custom font) beyond what was
   visible on the live site? Lucide is currently standing in.
4. White-on-dark and mark-only-white logo variants — do you have these as
   separate files?
