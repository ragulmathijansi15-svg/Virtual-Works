# Task 1 Design Specification — Northstar Home Services

## Design direction

The redesign uses a calm, high-trust service language: deep blue-green for reliability, warm orange for urgency and action, generous white space for clarity, and plain-language labels that work for both emergency and planned service visitors.

## Typography

| Token | Typeface | Size / line height | Use |
|---|---|---:|---|
| Display | Inter / system sans | 48/56 desktop; 36/44 tablet; 32/38 mobile | Hero headline |
| H1 | Inter 700 | 40/48 | Page titles |
| H2 | Inter 700 | 32/40 | Major sections |
| H3 | Inter 600 | 24/32 | Cards and subsections |
| Body | Inter 400 | 16/24 | Paragraphs and form help |
| Small | Inter 500 | 14/20 | Metadata, labels, helper copy |
| Button | Inter 600 | 16/20 | CTAs and controls |

Use sentence case, a maximum reading width of 65 characters, and a consistent heading hierarchy. Never communicate urgency through all-caps alone.

## Color system

| Token | Value | Intended use |
|---|---|---|
| `ink-900` | `#17202A` | Primary text and headings |
| `ink-600` | `#53606D` | Secondary text |
| `surface-0` | `#FFFFFF` | Main surfaces |
| `surface-50` | `#F5F7F8` | Alternating sections |
| `line-200` | `#D8DEE3` | Borders and dividers |
| `north-700` | `#164A63` | Links, navigation, primary trust color |
| `north-100` | `#DCECF1` | Soft information backgrounds |
| `signal-500` | `#C56B3D` | Primary CTA and urgent action |
| `success-700` | `#246B4A` | Confirmation and positive status |
| `danger-700` | `#A33A3A` | Validation and emergency warning |

Check every foreground/background pair for WCAG 2.2 AA contrast. Use icons and labels with color so status is never color-only.

## Layout foundations

- 4px base spacing scale: 4, 8, 12, 16, 24, 32, 48, 64, 80, 96.
- Desktop: 12 columns, 24px gutters, 80px outer margins, 1200px max content width.
- Tablet: 8 columns, 20px gutters, 40px outer margins.
- Mobile: 4 columns, 16px gutters, 20px page padding.
- Section padding: 80px desktop, 56px tablet, 40px mobile.
- Minimum touch target: 44 × 44px.

## Component breakdown

### Header
Logo, service-area cue, navigation, emergency phone link, and a persistent `Request service` button. On mobile, preserve the phone and CTA outside the menu.

### Hero intent selector
Three action cards: `Emergency help`, `Book a repair`, and `Explore services`. Each card includes an icon, one-sentence description, and a clear destination.

### Service card
An icon, plain-language service title, problem examples, proof cue, and `Learn more` link. Cards support default, hover, focus, and unavailable states.

### Trust strip
License/insurance, workmanship guarantee, service area, and review count. Every trust claim requires an approved source before production.

### Review and proof card
Rating, short quote, customer locality, and optional service category. Do not fabricate customer names, logos, or outcomes.

### Form fields
Label above control, helper text where needed, inline error, error summary, and success confirmation. Progressive disclosure keeps the first step short.

### CTA patterns
- Primary: filled `signal-500`, white label.
- Secondary: outlined `north-700` or text link.
- Emergency: visually distinct but still accessible; pair with safety guidance.

## States and behavior

Define default, hover, focus-visible, pressed, disabled, loading, success, error, and empty states. Use a 2px focus ring with 2px offset. Preserve form data on validation errors. Every asynchronous action receives a loading label and completion announcement.

## Auto-layout rules

Use vertical auto-layout for page sections and horizontal auto-layout for buttons, trust items, and card metadata. Headings hug height; body copy fills available width; cards use min-height only when aligning a row. Use component properties for service type, urgency, icon visibility, and state. Use constraints for persistent phone and CTA elements, and swap stacked layouts at the documented breakpoints.
