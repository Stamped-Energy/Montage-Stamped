---
name: Stamped Energy
description: Plant-office decision layer. ₹-scored prescriptions. Verified with evidence.
colors:
  primary: "#F75440"
  on-primary: "#ffffff"
  primary-fixed: "#ffdad4"
  inverse-primary: "#ffb4a8"
  secondary: "#000a07"
  on-secondary: "#ffffff"
  secondary-container: "#bdd9c8"
  tertiary: "#00666b"
  surface: "#f7faf5"
  surface-low: "#f1f4f0"
  on-surface: "#191c1a"
  on-surface-variant: "#5a403c"
  outline-variant: "#e3beb8"
  cream: "#fbfcf9"
  impact-lime: "#e8f07a"
  impact-lime-on: "#2f3218"
typography:
  display:
    fontFamily: "Space Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontWeight: 700
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Inter, ui-sans-serif, system-ui, sans-serif"
    fontWeight: 400
  label:
    fontFamily: "IBM Plex Mono, ui-monospace, monospace"
    fontWeight: 500
    letterSpacing: "0.12em"
rounded:
  md: "8px"
spacing:
  sm: "8px"
  md: "16px"
components:
  money-pill:
    backgroundColor: "{colors.on-surface}"
    textColor: "{colors.cream}"
    rounded: "{rounded.md}"
    padding: "4px 10px"
    typography: "{typography.label}"
  prescription-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "16px"
  signal-chip:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
---

# Design System: Stamped Energy

## 1. Overview

**Creative North Star: "Plant-office decision layer"**

Mid-morning control-office light: a plant director scanning ranked next actions with rupee impact, not a neon SaaS dashboard at 2am. Color strategy is **Committed**: Forge Coral carries identity and action; the default canvas stays demo-deck light. Imagery prefers product UI chrome (prescriptions, LIVE badges, signal chips on plant flow) over generic AI stock. Motion is progressive reveal with ease-out exponentials only.

This system inherits the stamped.work stack so OpenMontage heroes, Remotion, and HyperFrames match the marketing site. It explicitly rejects purple-on-white SaaS gradients, glassmorphism as default, hero-metric stat strips, identical icon-card grids, EMS/MES/CMMS cosplay, CVector clone kits as brand primaries, and dollar-scored prescriptions as the default.

**Key Characteristics:**
- Demo-deck light default; dark and impact-lime only as intentional scene modes
- Space Grotesk / Inter / IBM Plex Mono identity stack (no freshness swaps)
- Prescription card as the canonical UI unit; ₹ and action copy lead
- Flat tonal elevation; hairline borders; no stacked glass
- One composition per hero viewport: plant signals in → Stamped → prescriptions out

## 2. Colors

Committed Forge Coral on a cool mint-tinted office deck; neutrals stay ink-and-mute, never pure black/white.

### Primary
- **Forge Coral** (#F75440): CTAs, LIVE dots, traveling signal chips, ₹ emphasis, active steps. Roughly 30–40% of accent moments.
- **Coral Soft** (#ffdad4): Soft fills, negative tags, gentle coral fields (`primary-fixed`).
- **On Primary** (#ffffff): Text and icons on coral fills.

### Secondary
- **Obsidian Green** (#000a07): Problem / gravity bands, title cards, short narrative beats. Large dark fills use this, not coral drench.
- **Secondary Container** (#bdd9c8): Soft green support panels when needed.

### Tertiary
- **Teal Depth** (#00666b): Sparse supporting accent; never compete with coral for primary action.

### Neutral
- **Demo-deck** (#f7faf5): Default scene and hero background (`surface`).
- **Surface Low** (#f1f4f0): Soft panels and secondary bands.
- **Ink** (#191c1a): Headlines, body, money-pill fills (`on-surface`).
- **Mute** (#5a403c): Secondary copy and negative-tag ink (`on-surface-variant`).
- **Outline** (#e3beb8): Hairline UI chrome (`outline-variant`).
- **Cream** (#fbfcf9): Text on ink pills and light-on-dark chrome.

### Scene modes (not third primaries)
- **Impact Lime** (#e8f07a) / **On Impact** (#2f3218): Optional full-bleed outcome beat only.

### Named Rules
**The One Coral Rule.** Prefer coral on text, borders, pills, metrics, and chips. Large dark fills use secondary. Full coral drench only for short CTA or end cards.

**The Light Office Rule.** Most surfaces stay demo-deck light. Dark Obsidian and impact-lime are intentional scene modes, never the default chrome theme.

## 3. Typography

**Display Font:** Space Grotesk (with ui-sans-serif, system-ui)
**Body Font:** Inter (with ui-sans-serif, system-ui)
**Label/Mono Font:** IBM Plex Mono (with ui-monospace)

**Character:** Geometric display confidence, humanist body clarity, mono only as operational chrome (LIVE, steps, money tags). Plant-office, not editorial magazine or terminal cosplay.

### Hierarchy
- **Display** (700, tight tracking ~-0.025em): Wordmarks, section titles (e.g. Prescriptions), hero brand signals. Sentence case for long titles.
- **Body** (400–500): Supporting sentences, prescription action copy (~18px in the plant-flow hero). Cap line length ~65–75ch where prose runs.
- **Label** (500–700, wide tracking ~0.12em, often uppercase): LIVE, dock names, side tags, money pills. Sparse; mono is chrome, not costume for every line.

### Named Rules
**The Font Continuity Rule.** Inherit Space Grotesk / Inter / IBM Plex Mono so OpenMontage matches stamped.work. Greenfield “fresh font” swaps are forbidden.

**The No Gradient Text Rule.** Solid ink or cream only. Emphasis via weight and size, never `background-clip: text`.

## 4. Elevation

Flat / tonal. Depth comes from surface steps (`surface` → `surface-low`) and 1px `outline-variant` borders. Soft shadow only on primary CTA moments. No stacked glass cards, no multi-layer drop shadows as decoration.

### Shadow Vocabulary
- **CTA soft** (rare): a light coral-tinted halo or soft ambient under a primary action only. Default UI sits flush.

### Named Rules
**The Flat-By-Default Rule.** Surfaces are flat at rest. Shadows appear only as a response to intentional CTA elevation, never as card costume.

**The Hairline Rule.** Borders stay 1px. Side accent bars thicker than 1px are prohibited.

## 5. Components

Operational chrome: readable, rupee-led, hairline-framed. Cards exist only when they contain ranked actions or interaction.

### Buttons
- **Shape:** Gently curved edges (8px)
- **Primary:** Forge Coral fill, on-primary text; confident padding
- **Hover / Focus:** Darken coral slightly; visible focus ring; ease-out, no bounce
- **Secondary / Ghost:** Ink or outline on demo-deck; never purple gradients

### Chips
- **Style:** Coral signal chips (dots + short labels) for plant/market/application flows; labels sit above dots in stacking order
- **Money pill:** Ink fill (#191c1a), cream text; mono or tight sans; tens of thousands–lakhs scale language
- **State:** Traveling chips fade labels near the hub; dots continue; no startup flash at 0,0

### Cards / Containers
- **Corner Style:** Gently curved (8px)
- **Background:** Demo-deck or surface-low
- **Shadow Strategy:** Flat-by-default (see Elevation)
- **Border:** 1px outline-variant
- **Internal Padding:** Comfortable (~16px); prescription rows tall enough for ~18px action copy
- **Prescription card (canonical):** Mono status label, plain-language action title, owner/context, **₹ impact**, evidence line. Coral on ₹ or status, not a thick left stripe

### Inputs / Fields
- **Style:** Hairline stroke, surface fill, 8px radius
- **Focus:** Coral or ink border shift; no glass blur
- **Error / Disabled:** Mute ink; coral-soft field when soft-negative

### Navigation
- Brand-first: Stamped mark + two-line wordmark outrank decorative nav chrome. Body Inter; labels mono when sparse.

### Plant-flow hero (signature)
- Full-bleed demo-deck stage; Frame 10 plant art; wires; inbound chips from Market data / Plant telemetry / Application systems; outbound sequential coral relay to Prescriptions. One composition: brand, short support line only as needed, no hero overlays, no stat strips.

## 6. Do's and Don'ts

### Do:
- **Do** lead with ₹-scored prescriptions and verified-with-evidence language.
- **Do** keep the plant → Stamped → prescriptions loop visible in one composition.
- **Do** use Forge Coral (#F75440) on demo-deck (#f7faf5) with ink (#191c1a) type.
- **Do** expand jargon into plain industry language (energy price, power draw, demand forecast, ToD tariff, shift plan).
- **Do** ease-out exponentials only; honor `prefers-reduced-motion` with static or simplified reveals.
- **Do** keep money pills ink-on-cream and action copy large enough to read at a glance.

### Don't:
- **Don't** use purple-on-white SaaS gradients or glassmorphism as default.
- **Don't** ship hero-metric stat strips or identical icon-card grids.
- **Don't** use generic AI neural-net / circuit-board stock as the main visual idea.
- **Don't** cosplay EMS/MES/CMMS/plant-OS dashboards.
- **Don't** clone CVector kits (their marks, metrics, or claret/mindaro as brand primaries).
- **Don't** default to dollar-scored prescriptions (use rupee).
- **Don't** bounce, elastic, or spring-overshoot motion.
- **Don't** use side accent bars thicker than 1px, gradient text, or em dashes in on-screen copy.
