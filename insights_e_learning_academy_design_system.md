---
name: "Insights E-Learning Academy - K-12 Online Tutoring Design System"
description: "A friendly, trustworthy, and modern educational design system pairing crisp cobalt blue and vibrant mint with Outfit and Spline Sans typography."
---

## Overview

Insights E-Learning Academy is an online K–12 e-tutoring platform supporting CBSE, ICSE, and IGCSE students across Maths, Psychology, Coding with Python, Web Development, and Computational Thinking. The design system balances academic credibility for parents with approachable, interactive energy for students. It pairs clean warm-tinted surfaces, crisp 12px rounded cards with subtle 1px outlines, and generous breathing room so learning pathways and interactive activities feel clear and inviting rather than corporate or cluttered.

## Colors

The palette pairs a deep, trustworthy cobalt blue primary with a vibrant mint-emerald secondary accent on soft, airy light surfaces.

- **Primary:** Deep Cobalt (`#003E94` / `#1D56B8` container) anchors primary actions, active navigation states, and key academic badges.
- **Secondary:** Emerald Mint (`#006C4F` / `#80F9CA` container) highlights technology pathways, interactive challenges, and positive learning outcomes.
- **Tertiary:** Warm Amber-Terracotta (`#732F00` / `#FFDBCB` soft tint) draws attention to Fun Facts, featured blog highlights, and consultation prompts.
- **Surfaces:** Bright airy off-white (`#FAF8FF`) canvas with pure white (`#FFFFFF`) elevated cards and soft cool-tinted containers (`#F3F3FC`, `#EDEDF6`).

```yaml
colors:
  primary: "#003E94"
  on-primary: "#FFFFFF"
  primary-container: "#1D56B8"
  on-primary-container: "#FFFFFF"
  primary-soft: "#EEF0FF"
  on-primary-soft: "#002D6F"
  secondary: "#006C4F"
  on-secondary: "#FFFFFF"
  secondary-container: "#80F9CA"
  on-secondary-container: "#002116"
  secondary-soft: "#F4FFF7"
  on-secondary-soft: "#003827"
  tertiary: "#732F00"
  on-tertiary: "#FFFFFF"
  tertiary-container: "#FFDBCB"
  on-tertiary-container: "#341100"
  error: "#BA1A1A"
  on-error: "#FFFFFF"
  error-container: "#FFDAD6"
  on-error-container: "#410002"
  background: "#FAF8FF"
  on-background: "#191B22"
  surface: "#FAF8FF"
  surface-container-lowest: "#FFFFFF"
  surface-container-low: "#F3F3FC"
  surface-container: "#EDEDF6"
  surface-container-high: "#E7E7F0"
  on-surface: "#191B22"
  surface-variant: "#DFE2F1"
  on-surface-variant: "#434652"
  outline: "#737784"
  outline-variant: "#C3C6D5"
```

## Typography

**Spline Sans** drives display and section headings with crisp geometric clarity, **Outfit** handles all body copy, navigation, and UI labels with friendly open counters, and **JetBrains Mono** renders code snippets and interactive coding puzzles.

```yaml
typography:
  display-lg:
    fontFamily: "Spline Sans"
    fontSize: 48px
    fontWeight: 700
    lineHeight: 56px
    letterSpacing: -0.75px
  display-lg-mobile:
    fontFamily: "Spline Sans"
    fontSize: 32px
    fontWeight: 700
    lineHeight: 40px
    letterSpacing: -0.5px
  headline-lg:
    fontFamily: "Spline Sans"
    fontSize: 36px
    fontWeight: 700
    lineHeight: 44px
    letterSpacing: -0.5px
  headline-lg-mobile:
    fontFamily: "Spline Sans"
    fontSize: 28px
    fontWeight: 700
    lineHeight: 34px
    letterSpacing: -0.25px
  headline-md:
    fontFamily: "Spline Sans"
    fontSize: 26px
    fontWeight: 600
    lineHeight: 32px
    letterSpacing: -0.25px
  title-lg:
    fontFamily: "Spline Sans"
    fontSize: 20px
    fontWeight: 600
    lineHeight: 28px
    letterSpacing: 0px
  title-md:
    fontFamily: "Outfit"
    fontSize: 18px
    fontWeight: 600
    lineHeight: 24px
    letterSpacing: 0px
  body-lg:
    fontFamily: "Outfit"
    fontSize: 18px
    fontWeight: 400
    lineHeight: 28px
    letterSpacing: 0px
  body-md:
    fontFamily: "Outfit"
    fontSize: 16px
    fontWeight: 400
    lineHeight: 24px
    letterSpacing: 0px
  body-sm:
    fontFamily: "Outfit"
    fontSize: 14px
    fontWeight: 400
    lineHeight: 20px
    letterSpacing: 0px
  label-lg:
    fontFamily: "Outfit"
    fontSize: 15px
    fontWeight: 600
    lineHeight: 20px
    letterSpacing: 0.1px
  label-md:
    fontFamily: "Outfit"
    fontSize: 13px
    fontWeight: 600
    lineHeight: 18px
    letterSpacing: 0.2px
  label-sm:
    fontFamily: "Outfit"
    fontSize: 12px
    fontWeight: 500
    lineHeight: 16px
    letterSpacing: 0.25px
  code-md:
    fontFamily: "JetBrains Mono"
    fontSize: 14px
    fontWeight: 500
    lineHeight: 22px
    letterSpacing: 0px
```

## Layout & Spacing

Desktop screens use a centered max-width container (`1200px` / `max-w-7xl`) with a 12-column CSS Grid and `24px` gutters, collapsing cleanly to 2-column tablet (`md:`) and single-column mobile (`390px`) stacks with `16px` page margins. A strict 8px spacing scale governs vertical rhythm and component padding.

```yaml
spacing:
  gutter-xs: 4px
  gutter-sm: 8px
  gutter-md: 16px
  gutter-lg: 24px
  gutter-xl: 32px
  section: 64px
  page-margin: 24px
```

## Elevation & Depth

Hierarchy relies on tonal surface stepping (`surface` → `surface-container-low` → `surface-container-lowest`) paired with crisp `1px` `outline-variant` borders and whisper-soft ambient shadows (`0 4px 20px rgba(25, 27, 34, 0.05)`) on interactive cards. Heavy drop shadows and glassmorphic blurs are avoided to keep text crisp for parents and students.

## Shapes

Cards use crisp `12px` (`rounded-md`) corners, primary buttons and form inputs use `8px` (`rounded`) corners, and subject/grade pills use full `9999px` (`rounded-full`) capsules.

```yaml
rounded:
  sm: 4px
  DEFAULT: 8px
  md: 12px
  lg: 16px
  xl: 24px
  full: 9999px
```

## Motion & Micro-interaction

Interactions feel responsive and calm: button hovers and accordion toggles settle in `150ms`, while card hover lifts and tab transitions ease smoothly in `220ms`. Nothing loops continuously or distracts from reading.

```yaml
motion:
  state-change:
    duration: 150ms
    delay: 0ms
    timingFunction: ease-out
  surface-enter:
    duration: 220ms
    delay: 0ms
    timingFunction: cubic-bezier(0.2, 0, 0, 1)
  surface-exit:
    duration: 150ms
    delay: 0ms
    timingFunction: cubic-bezier(0.3, 0, 1, 1)
```

## Voice & Content Strategy

- **Tone of voice:** Encouraging, clear, and trustworthy—warm enough for K–12 students, structured enough to reassure parents comparing CBSE, ICSE, and IGCSE support.
- **Capitalisation:** Sentence case for headings, labels, and body copy; Title Case for brand name, page titles, and subject names.
- **Button labels:** Clear action-oriented phrases ("Explore Courses", "Enquire Now", "Book a Free Consultation", "Enquire About This Course", "Read More").
- **Accessibility:** Plain language, generous contrast, descriptive alt text on all imagery, and clear validation feedback on forms.

## Components

Component implementations live as individual HTML sticker sheet files in
`components/`. Each file contains the canonical, styled HTML components with
`<!-- COMPONENT: name -->` comment markers. Read each file before use.

- **Accordion** → `@components/accordion.html`: `accordion-single`, `accordion-group`
- **Button** → `@components/button.html`: `button-primary`, `button-icon`, `button-with-icon`
- **Card** → `@components/card.html`: `card-elevated`, `card-action`, `card-interactive`, `card-interactive-2`
- **Chip** → `@components/chip.html`: `chip-action`, `chip-input`, `chip-with-icon`
- **Input Field** → `@components/input-field.html`: `input-field-text`, `input-field-icon`
