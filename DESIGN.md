---
name: LUMI
description: An intelligent daily planning atelier that transforms unstructured thoughts into clear action.
colors:
  primary: "#5B3EE8"
  primary-hover: "#4A2FD0"
  primary-light: "#F0EDFD"
  primary-gradient-end: "#6E53F1"
  selection-tint: "#E0DAFC"
  scrollbar-track: "#D5CEE5"
  scrollbar-thumb: "#BCB2D4"
  canvas: "#F8F9FC"
  surface: "#FFFFFF"
  text-primary: "#1A162B"
  text-secondary: "#5E5B73"
  text-muted: "#8A879E"
  border-subtle: "#EAE7F2"
  border-strong: "#DDD8EB"
  border-hover: "#D6CEEC"
  priority-high-bg: "#FDF2F4"
  priority-high-text: "#A11D33"
  priority-high-border: "#F9D5DC"
  priority-med-bg: "#FEF6EB"
  priority-med-text: "#87510C"
  priority-med-border: "#FCE4C3"
  priority-low-bg: "#EDFBF2"
  priority-low-text: "#166534"
  priority-low-border: "#C8F0D6"
typography:
  display:
    fontFamily: "Manrope, sans-serif"
    fontSize: "2.25rem"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "-0.03em"
  headline:
    fontFamily: "Manrope, sans-serif"
    fontSize: "1.5rem"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.02em"
  title:
    fontFamily: "Manrope, sans-serif"
    fontSize: "1.125rem"
    fontWeight: 700
    lineHeight: 1.4
    letterSpacing: "-0.015em"
  body:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
    lineHeight: 1.6
    letterSpacing: "0em"
  label:
    fontFamily: "DM Sans, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 600
    lineHeight: 1.4
    letterSpacing: "0.02em"
rounded:
  xs: "6px"
  sm: "9px"
  md: "10px"
  card: "12px"
  lg: "14px"
  surface: "16px"
  xl: "20px"
  full: "9999px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
components:
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "#FFFFFF"
    rounded: "{rounded.md}"
    padding: "10px 20px"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
---

# Design System: LUMI

## Overview

**Creative North Star: "The Daylight Atelier"**

LUMI creates a distraction-free, elegant workspace designed to calm cognitive anxiety and sharpen personal agency. Instead of washed-out novelty pastels or overbearing neon glows, LUMI combines a pristine porcelain canvas with rich violet-slate typography, tactile surfaces, and purposeful iris accents.

Every visual element serves clear readability: information hierarchy is established through precise typographic scale and weight rather than gratuitous boxes or jarring gradients. Spacing is intentional: tight groups within task units and generous separation between navigational zones.

**Key Characteristics:**
- **Pristine Contrast:** High-contrast violet-slate typography (`#1A162B`) over clean porcelain (`#F8F9FC`), passing WCAG AAA standards.
- **Purposeful Iris Accent:** Bold royal iris (`#5B3EE8`) reserved strictly for primary actions, focused tabs, and progress milestones.
- **Refined Tactility:** Crisp borders (`#EAE7F2`) combined with gentle, soft-focus ambient elevation rather than heavy zero-blur drop shadows.
- **Zero Eyebrow Policy:** Headings speak for themselves with authoritative typography without amateurish decorative labels.

## Colors

The palette balances clean airy neutrality with a distinctive, focused royal iris signature and clear semantic priority signifiers.

### Primary
- **Royal Iris** (`#5B3EE8`): Used for primary action buttons, active tab indicators, and progress tracks.
- **Iris Hover** (`#4A2FD0`): Subtle deepening on hover for immediate tactile feedback.
- **Iris Tint** (`#F0EDFD`): Soft background tint for brand badges and highlighted states.

### Neutral
- **Canvas Pearl** (`#F8F9FC`): Calm, eye-friendly light backdrop that prevents glare.
- **Surface Pure** (`#FFFFFF`): Crisp white card layer providing clean physical definition.
- **Text Primary** (`#1A162B`): Rich, deep violet-slate providing effortless readability.
- **Text Secondary** (`#5E5B73`): Clear, balanced secondary copy for descriptions and metadata.
- **Text Muted** (`#8A879E`): Subtle helper labels and placeholders.
- **Border Subtle** (`#EAE7F2`): 1px boundary separating surface layers without visual clutter.

### Semantic Priorities
- **Urgent / High** (`#A11D33` on `#FDF2F4`, border `#F9D5DC`): Refined cranberry crimson for immediate attention without harsh alarmism.
- **Focused / Medium** (`#87510C` on `#FEF6EB`, border `#FCE4C3`): Warm honey amber for scheduled deliverables.
- **Steady / Low** (`#166534` on `#EDFBF2`, border `#C8F0D6`): Calm meadow emerald for low-urgency tasks.

### Named Rules
**The Iris Focus Rule:** The royal iris accent is reserved strictly for interactive primary actions and active state focus. Decorative elements must not compete with primary calls to action.
**The No-Mud Rule:** Secondary text is tinted with cool slate-violet, never a washed-out mid-gray on colored surfaces.

## Typography

**Display Font:** Manrope, sans-serif
**Body Font:** DM Sans, sans-serif

**Character:** Modern geometric clarity meets editorial warmth. Manrope brings structure and confidence to metrics and titles, while DM Sans delivers comfortable, fatigue-free scanning for task lists.

### Hierarchy
- **Display** (800 weight, clamp(1.8rem, 3.5vw, 2.5rem), 1.2 line-height): Hero header and brand presence.
- **Headline** (700 weight, 1.4rem, 1.3 line-height): Main view section titles.
- **Title** (700 weight, 1.05rem, 1.4 line-height): Task card headings and metric cards.
- **Body** (400 weight, 0.9375rem, 1.6 line-height, 65ch measure): Descriptions, helper copy, and content.
- **Label** (600 weight, 0.8125rem, 0.02em letter-spacing): Form labels, metadata tags, and metric subtitles.

### Named Rules
**The Single Hierarchy Step Rule:** Visual prominence must step down smoothly: Hero Title → Section Title → Card Title → Metadata Tag. No abrupt font jumps.

## Layout

The application uses an expansive, centered container (max-width: 1280px) with responsive horizontal padding (`clamp(1rem, 3vw, 2.5rem)`).
- **Navigation:** Left-aligned or centered modern segmented tabs with clear active indicators.
- **Task Board:** Responsive dual-column layout (To Do / Completed) adapting smoothly to single-column stacking on mobile viewports (breakpoint: 768px).
- **Form Flow:** Grouped logical inputs with consistent 16px internal grid gaps.

## Elevation & Depth

Surfaces rest on subtle structural elevation. Flat by default, with micro-elevation providing depth on cards and buttons.

### Shadow Vocabulary
- **Card Rest** (`box-shadow: 0 1px 3px rgba(27, 20, 54, 0.03), 0 4px 12px rgba(27, 20, 54, 0.025)`): Applied to metric containers and task cards.
- **Card Hover** (`box-shadow: 0 4px 12px rgba(27, 20, 54, 0.06), 0 1px 4px rgba(27, 20, 54, 0.04)`): Elevates task cards gently on user interaction.
- **Button Rest** (`box-shadow: 0 1px 2px rgba(16, 24, 40, 0.05), 0 2px 4px rgba(91, 62, 232, 0.15)`): Crisp tactile depth for primary triggers.

### Named Rules
**The Layering Rule:** Layering is achieved by background contrast (`#F8F9FC` to `#FFFFFF`) and a 1px subtle border (`#EAE7F2`). Heavy dark drop shadows are forbidden.

## Shapes

- **Base Radius:** 10px on inputs and small cards; 14px on content containers and metrics; 20px on the hero atelier.
- **Buttons:** 10px smooth squircle with comfortable 44px minimum touch target.
- **Pills / Tags:** Pill shape (9999px) for priority badges, status chips, and progress bars.

## Components

### Buttons
- **Shape:** 10px radius, 44px minimum height.
- **Primary:** Solid `#5B3EE8` with `#FFFFFF` crisp text, smooth `0.2s cubic-bezier(0.4, 0, 0.2, 1)` transition.
- **Hover:** Deepened `#4A2FD0`, -1px translateY translation.
- **Focus:** 2px solid `#5B3EE8` with 2px offset.

### Inputs & Selectboxes
- **Style:** Pure white surface, 1px solid `#DDD8EB` border, 10px radius, 42px height.
- **Focus:** Border shifts to `#5B3EE8` with soft iris halo (`0 0 0 3px rgba(91, 62, 232, 0.12)`).

### Priority Badges (Chips)
- **Style:** Compact pill (`padding: 3px 10px`), 0.75rem font size, 700 weight, matching border tint.

### Metric Cards
- **Style:** Clean white card with subtle border, 14px radius, clear bold metric value in Manrope, uppercase subtle label.

## Do's and Don'ts

### Do:
- **Do** keep text contrast above 4.5:1 on all surfaces.
- **Do** use pure white text (`#FFFFFF`) on primary iris action buttons.
- **Do** provide smooth micro-transitions on interactive hover states.
- **Do** maintain balanced spacing with more whitespace above section titles than below.

### Don't:
- **Don't** use kicker/eyebrow labels above headings.
- **Don't** force pure black text (`#000000`) onto pastel buttons.
- **Don't** use right-aligned tabs that disconnect navigation from content.
- **Don't** use harsh zero-blur drop shadows or garish multi-colored gradients.
