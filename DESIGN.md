---
name: Antonello Totaro Portfolio
description: Warm-dark editorial portfolio for a GTM operator and AI-native builder
colors:
  bg: "#0a0a0a"
  surface: "#111111"
  surface2: "#1a1a1a"
  border: "#222222"
  text: "#f0ece4"
  muted: "#8d8881"
  accent: "#c9b99a"
  gold: "#d4a853"
typography:
  display:
    fontFamily: "Instrument Serif, Georgia, serif"
    fontSize: "clamp(4rem, 9vw, 8rem)"
    fontWeight: 400
    lineHeight: 0.9
    letterSpacing: "-0.02em"
  headline:
    fontFamily: "Instrument Serif, Georgia, serif"
    fontSize: "clamp(2rem, 4vw, 3.2rem)"
    fontWeight: 400
    lineHeight: 1.15
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Instrument Serif, Georgia, serif"
    fontStyle: "italic"
    fontSize: "1.3rem"
    fontWeight: 400
    lineHeight: 1.2
  body:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 300
    lineHeight: 1.7
  label:
    fontFamily: "DM Mono, monospace"
    fontSize: "10px"
    fontWeight: 400
    lineHeight: 1.4
    letterSpacing: "0.15em"
rounded:
  none: "0"
  chip: "3px"
  full: "9999px"
spacing:
  xs: "0.5rem"
  sm: "1rem"
  md: "1.5rem"
  lg: "3rem"
  xl: "6rem"
components:
  card:
    backgroundColor: "{colors.bg}"
    textColor: "{colors.text}"
    rounded: "{rounded.none}"
    padding: "2.5rem"
  card-hover:
    backgroundColor: "{colors.surface}"
  chip:
    backgroundColor: "{colors.bg}"
    textColor: "{colors.muted}"
    rounded: "{rounded.none}"
    padding: "0.3rem 0.8rem"
  button-ghost:
    backgroundColor: "{colors.bg}"
    textColor: "{colors.accent}"
    rounded: "{rounded.none}"
    padding: "0.75rem 1.5rem"
  badge-open:
    textColor: "{colors.gold}"
    rounded: "{rounded.none}"
    padding: "0.4rem 1rem"
---

# Design System: Antonello Totaro Portfolio

## 1. Overview

**Creative North Star: "The Operator's Dossier"**

This is a confidential, high-signal file on a person who closes deals and builds his own tools. The page reads like a dossier opened on a desk at night: near-black paper, a worn-brass ink for the things that matter, and a single live gold marker for what is current. Monospace runs the margins as field tags and metadata; an Instrument Serif italic is the human voice that speaks between the data. Nothing shouts. The proof does the talking.

The system is editorial first. Hierarchy comes from type scale and the contrast between a quiet 300-weight sans body and an oversized serif display, not from boxes or color. Surfaces are flat and layered tonally (three steps of near-black); the only depth is a restrained lift when you reach for something. Accent is rationed: most of the page is neutral, brass appears where craft or emphasis lives, and gold is reserved almost entirely for the "live / open to work" signal.

It explicitly rejects three things. **No generic SaaS landing**: no gradient blobs, no hero-metric template, no identical feature-card grids. **No LinkedIn / corporate CV**: no stock-blue, no buzzword soup, no timeline-résumé scaffolding. **No AI-slop dark portfolio**: no neon-on-black, no decorative glassmorphism, no glowing gradient text, no off-the-shelf dev-folio clone. The warmth of the palette is what keeps it human and out of the template lane.

**Key Characteristics:**
- Warm-dark, never cold: every neutral is tinted toward brass, the off-white text is `#f0ece4`, not white.
- Sharp-cornered (0 radius) surfaces with hairline `#222` borders and tonal layering instead of shadow.
- Oversized Instrument Serif display against quiet DM Sans body and DM Mono metadata.
- One rationed accent (Aged Brass) plus one rare live signal (Lamp Gold).
- Restraint as the default; motion and color are earned, not sprayed.

## 2. Colors

A warm-neutral dark palette: three tonal near-blacks, a tinted off-white, and two warm accents that earn their rare appearances.

### Primary
- **Aged Brass** (`#c9b99a`): The dominant accent. Worn, expensive, never bright. Carries serif emphasis (`em` inside display and headlines), section-label leads, system titles, ghost-button text, deal amounts, the divider-line fade. This is the page's "ink for what matters."

### Secondary
- **Lamp Gold** (`#d4a853`): The live signal, used sparingly. The pulsing "open to work" badge dot, status border, partner amounts, map pulse points, the reading-progress bar's bright end. Its scarcity is what makes it read as "current / active."

### Neutral
- **Void Black** (`#0a0a0a`): Page background and base card surface. The "paper."
- **Surface** (`#111111`): First tonal lift, hover background for rows.
- **Surface Two** (`#1a1a1a`): Second tonal lift, deepest interactive surface.
- **Hairline** (`#222222`): Every border, gridline, and divider. Structure without weight.
- **Bone** (`#f0ece4`): Primary text. A warm off-white, never pure white.
- **Ash** (`#8d8881`): Muted text, labels, secondary copy, inactive nav. A warm-tinted gray, not neutral. Tuned to clear WCAG AA on Void Black (≈5.6:1); never drop it back toward `#6b6b6b` (3.7:1, fails).

### Named Rules
**The Rationed Accent Rule.** Brass and gold together stay on roughly 10% of any screen. Most of the page is Bone-on-Black. Brass marks craft and emphasis; Gold marks what is live. If a third thing wants color, it gets weight or size instead.

**The No-White Rule.** `#fff` and `#000` are forbidden. Text is Bone (`#f0ece4`); the darkest surface is Void Black (`#0a0a0a`). Every neutral is tinted warm.

## 3. Typography

**Display Font:** Instrument Serif (with Georgia, serif)
**Body Font:** DM Sans (with sans-serif), weight 300
**Label/Mono Font:** DM Mono (monospace)

**Character:** A three-voice system. Instrument Serif is the human speaking, often in italic for emphasis and warmth. DM Sans at 300 is the quiet narrator: light, unhurried, readable. DM Mono is the machine margin: uppercase, wide-tracked metadata, section tags, and field labels. The tension between an oversized warm serif and clinical mono tags is the whole personality.

### Hierarchy
- **Display** (400, `clamp(4rem, 9vw, 8rem)`, line-height 0.9, `-0.02em`): Hero name only. Serif `em` inside it turns brass and italic.
- **Headline** (400, `clamp(2rem, 4vw, 3.2rem)`, line-height 1.15): About and contact headlines; the page's larger statements.
- **Title** (400 italic, `1.1–1.5rem`): Card subjects, deal/partner/early-role names, planet placements, language names. Always serif italic.
- **Body** (300, `0.85–0.95rem`, line-height 1.7–1.8): All running copy. Color is Ash (`#8d8881`) for descriptions, Bone for primary. Keep measure at 65–75ch.
- **Label** (400, `10–13px`, letter-spacing `0.1–0.25em`, UPPERCASE): DM Mono section labels, tags, nav links, stat captions, status text.

### Named Rules
**The Three-Voice Rule.** Serif speaks (headings, names, emphasis), Sans narrates (body), Mono tags (labels, metadata). Never mix the jobs: no mono headings, no serif body, no sans labels.

**The Italic-Brass Rule.** Emphasis inside a serif heading is expressed as italic in Aged Brass, never bold, never a different size.

## 4. Elevation

Flat by default, lift on state. Surfaces sit on the page as flat tonal layers (Void Black → Surface → Surface Two); separation comes from hairline borders and tone, not shadow. The only shadow in the system is a single soft lift that appears on card hover, paired with a 2px upward translate. Glow effects (brass/gold box-shadow on hover of buttons and the toni CTA) are atmospheric, not structural.

### Shadow Vocabulary
- **Card Lift** (`box-shadow: 0 8px 24px rgba(0,0,0,0.35)`): On hover of partner, system, and early cards, with `translateY(-2px)`. The page's only real shadow.
- **Accent Glow** (`box-shadow: 0 0 12px–15px rgba(201,185,154,0.15–0.25)`): Soft brass halo on hover of hero links and the Toni CTA. Decorative warmth, not depth.

### Named Rules
**The Flat-Until-Touched Rule.** Surfaces are flat at rest. Shadow exists only as a response to hover. A resting element never carries a drop shadow.

## 5. Components

### Buttons
- **Shape:** Sharp, 0 radius (`{rounded.none}`).
- **Ghost (primary CTA pattern):** Transparent background, 1px Brass border, Brass mono uppercase label, padding `0.75rem 1.5rem`. The Toni CTA and hero links follow this.
- **Hover / Focus:** Brass border brightens, faint Accent Glow halo appears, background lifts to `rgba(201,185,154,0.05)`. Transition `all 0.2–0.3s ease`.

### Chips / Tags
- **Style:** Transparent background, 1px Hairline border, Ash mono uppercase text, `10px`, padding `0.3rem 0.8rem`, 0 radius.
- **Variants:** Brass-bordered "highlight" tag (`rgba(201,185,154,0.2)` border, Brass text) for emphasis; standard Hairline tag for neutral skills.

### Cards / Containers
- **Corner Style:** Sharp, 0 radius.
- **Background:** Void Black at rest; Surface (`#111`) on hover.
- **Shadow Strategy:** Flat at rest; Card Lift shadow + `translateY(-2px)` on hover (see Elevation).
- **Border:** Cards sit on a Hairline grid: a 1px Hairline gap (`gap: 1px; background: var(--border)`) creates dividing lines between grid cells, not per-card borders.
- **Internal Padding:** `2.5rem` (standard), `3rem 2.5rem` (partner), `4rem` (Toni block).

### Navigation
- **Style:** Fixed top bar, `rgba(10,10,10,0.85)` with `backdrop-filter: blur(12px)`, Hairline bottom border.
- **Typography:** DM Mono, `12–13px`, uppercase, wide tracking, Ash default.
- **States:** Hover and active links turn Brass. Mobile collapses to a `☰` toggle opening a full-width Surface menu.

### Signature Components
- **Reading Progress Bar:** 3px fixed top bar, `linear-gradient(to right, Brass, Gold)`, width tracks scroll. The one place the two accents blend.
- **"Open To" Badge:** Mono uppercase, 1px gold-tinted border, with a 6px Lamp Gold dot pulsing on a 2s loop. The live signal.
- **Deal Drawer:** Sharp rows that expand inline on click; a `+` indicator rotates 45° to Brass, a dashed Hairline rule separates a 3-column drawer. Inline progressive disclosure, never a modal.
- **Interactive World Map:** Low-opacity SVG behind the hero; brass-highlighting country paths and pulsing gold hotspots with mono tooltips. Atmosphere and proof of reach.

## 6. Do's and Don'ts

### Do:
- **Do** keep text Bone (`#f0ece4`) on Void Black (`#0a0a0a`). Tint every neutral warm.
- **Do** ration accent: Brass for emphasis/craft, Gold only for the live "open to work" signal. Keep both under ~10% of any screen.
- **Do** use the three-voice type system: serif speaks, sans narrates, mono tags.
- **Do** keep surfaces flat at rest; introduce the Card Lift shadow only on hover.
- **Do** express heading emphasis as italic Brass, never bold.
- **Do** disclose detail inline (the deal drawer), and honor `prefers-reduced-motion` by gating reveals, the flow stepper, and map pulses.

### Don't:
- **Don't** build a generic SaaS landing: no gradient blobs, no hero-metric template, no identical feature-card grids.
- **Don't** drift toward a LinkedIn / corporate CV: no stock-blue, no buzzword soup, no timeline-résumé layout, no headshot-and-badges.
- **Don't** produce AI-slop dark-portfolio tropes: no neon-on-black, no decorative glassmorphism, no glowing gradient text (no `background-clip: text` on a gradient).
- **Don't** use `#fff` or `#000` anywhere.
- **Don't** round corners; this system is sharp (0 radius), except the 3px tooltip and circular pulse dots.
- **Don't** add side-stripe borders (`border-left`/`border-right` >1px as a colored accent). Use full hairline borders or tonal background instead.
- **Don't** spray gold; if it stops being rare, it stops reading as "live."

---

## 7. Live Critique — 2026-06-04 (flow · hierarchy · emotional resonance)

Source: walked every section top-to-bottom on the live build (`antonello-portfolio.vercel.app`) via browser automation, exercised all clickables (nav anchors, deal drawers, mobile menu, external links), at desktop (1592w) and mobile (390w). Detector run on `index.html`. Focus per request: flow, hierarchy, emotional resonance. **Design health: 34/40 (Good).**

### Heuristic scores

| # | Heuristic | Score | Key note |
|---|-----------|-------|----------|
| 1 | Visibility of System Status | 4 | Reading-progress bar, active-nav Brass highlight, deal `+`→`×` toggle, pulsing "open to" dot — system state always legible. |
| 2 | Match System / Real World | 4 | GTM/revenue language is correct for the audience; every metric is labeled. |
| 3 | User Control & Freedom | 3 | Drawers re-collapse, mobile menu has `✕`, anchors jump cleanly. No skip-link / focus-trap handling verified. |
| 4 | Consistency & Standards | 4 | Hairline grid, three-voice type, sharp corners held everywhere. |
| 5 | Error Prevention | 3 | Few error surfaces (mailto/calendar are external); nothing to mis-submit. |
| 6 | Recognition vs Recall | 4 | Text nav labels, named sections, no icon-only traps. |
| 7 | Flexibility & Efficiency | 2 | One linear path; no keyboard shortcuts, no skip-to-content. |
| 8 | Aesthetic & Minimalist | 4 | Editorial restraint is the strongest dimension; nothing decorative competes. |
| 9 | Error Recovery | 3 | No form/error states to recover from. |
| 10 | Help & Documentation | 3 | Not needed for a portfolio; contact paths are obvious. |

### AI-slop verdict

Passes the absolute bans (no gradient text, no glass, no SaaS-cream, no neon-on-black, sharp corners held). **One standing risk:** the page sits squarely in the *editorial-typographic* saturated lane (display-serif italic + small mono labels + ruled separators), and every section carries a tiny uppercase tracked eyebrow (`ABOUT`, `NUMBERS`, `SOLO DEAL WINS`, `OPEN TO`, `PARTNERSHIPS BUILT`…). That repeated-kicker grammar is the lane's fingerprint. PRODUCT.md commits to this lane as identity, so **identity-preservation applies and this is defensible** — but it is the single biggest "which AI made this?" exposure, so the cadence is worth varying rather than scaffolding by reflex. Detector also flagged 22 em-dashes in body copy (a cadence tell that violates this doc's own copy rule) and `Instrument Serif` as a reflex-reject face (kept here as committed identity).

### What's working

- **Proof-first flow holds.** About → Numbers → Deals → Partnerships → Toni → GTM systems → Roots → Languages → Stack → Astro → Contact. Credibility is banked before the ask; the narrative earns the "Let's talk." close. Honors Design Principle 1.
- **The deal drawer is the emotional peak.** Clicking a row reveals a `FRICTION → BREAKTHROUGH → THE PLAY` three-column story. It shows *how he thinks*, not just what he closed — exactly the founder-audience proof PRODUCT.md asks for. Best interaction on the page.
- **Distinctive, on-brand restraint.** Warm-dark palette, three-voice type, rationed Brass/Gold. Reads as a deliberate human, not a dev-folio template (Design Principle 3 met).

### Emotional journey (peak-end)

- **Peak:** hero name reveal + the deal-drawer storytelling.
- **Valley:** the STACK chip walls and LANGUAGES grid — competent but flat; energy dips just before Astro.
- **End:** Astro "The Global Explorer" humanizes (and is correctly defused with "Read it as personality, not a hiring criterion"), then "Let's talk." lands warm. Peak-end rule satisfied.

### Priority issues (ordered)

- **[P1] Mobile hero hook is truncated.** `.hero-sub` is `-webkit-line-clamp: 4` on ≤768px, so the positioning statement cuts off mid-sentence ("…never without a team when it…"). The audience often arrives on mobile with 30–60s; the emotional hook is exactly what gets clipped. *Fix:* drop the clamp or tighten the copy to fit 3–4 lines un-truncated. → `/impeccable adapt`
- **[P2] Mobile menu reads unfinished.** `.nav-menu` is a content-height `position: fixed` sheet (`max-height: calc(100vh - 4.5rem)`) with no backdrop scrim, so page content bleeds through below the last link. *Fix:* add a dimming scrim or take the sheet full-height. Also the `.nav-toggle` tap target is ~21px (font-size 1.3rem, zero padding) — below the 44×44 minimum. → `/impeccable adapt`
- **[P2] Em-dash cadence.** 22 em-dashes in body copy is an AI-cadence tell and breaks this doc's own copy rule. *Fix:* convert to commas/colons/periods/parentheses. → `/impeccable clarify`
- **[P2] Editorial-lane / repeated-eyebrow exposure.** See AI-slop verdict. Vary the section-label cadence (drop some kickers, let a few section titles stand alone) so the rhythm reads as voice, not scaffold. → `/impeccable typeset`
- **[P3] Two stat clusters compete near the top.** Hero stats (`$600k+ · 20× · 6 · 14→1`) and the NUMBERS band (`$464k+ · 14+ · 160+ · $0`) are both four-up big-figure rows within one scroll; `$0 marketing budget` is cryptic without its framing line. Consider differentiating their visual treatment so the second doesn't read as a repeat. → `/impeccable layout`
- **[P3] Hero display ceiling.** `clamp(4rem, 9vw, 8rem)` tops out at 128px, above the ~96px display ceiling — borderline "shouting," acceptable for a brand hero but worth a glance at large viewports.

### Persona red flags

- **Casey (mobile):** truncated hero hook; sub-44px hamburger; menu sheet bleed-through; two tall stacked stat clusters push proof further down.
- **Jordan (first-timer):** `$0` stat is ambiguous without its caption; Astro could read as noise on a fast skim (mitigated by the disclaimer).
- **Sam (a11y):** verify muted-label contrast (Ash/muted on Void Black risks <4.5:1) and visible focus indicators on nav anchors and deal-drawer rows; tap targets as above.

### Questions to consider

- What would the mobile-first version of the hero say in 3 un-truncated lines?
- Do the hero stats and the NUMBERS band need to be two separate moments, or is one stronger cluster more confident?
- If you dropped half the section eyebrows, would the page feel less "designed" — or more?
