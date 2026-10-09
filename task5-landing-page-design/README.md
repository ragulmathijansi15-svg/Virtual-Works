# Relay — Landing Page Design

> A high-converting desktop SaaS landing page for Relay, a lightweight customer feedback platform.

## Project snapshot

| Field | Details |
|---|---|
| **Role** | Product designer: UX strategy, information architecture, interaction design, visual design, and handoff specification |
| **Scope** | One responsive-ready desktop marketing page, from first impression through conversion CTA |
| **Platform** | Desktop web, optimized for 1440 px viewport and designed to scale down gracefully |
| **Timeline** | 2 weeks: discovery and content strategy (days 1–3), wireframes (days 4–5), visual design (days 6–9), validation and handoff (days 10–14) |
| **Primary audience** | Startup founders, product managers, and customer-facing teams at small B2B SaaS companies |
| **Deliverables** | Page strategy, content hierarchy, user flow, high-fidelity screen specification, design system, interaction states, testing plan, and implementation-ready canvas organization |

## Problem and opportunity

Customer feedback tools often present a familiar tension: enterprise platforms feel powerful but heavy, while forms and spreadsheets fragment the workflow. A visitor needs to understand three things quickly:

1. **What is Relay?** A shared place to capture, tag, and prioritize feedback.
2. **Why change now?** Relay turns scattered requests into a visible decision signal.
3. **What will it cost me?** The first useful workflow should feel achievable before a sales conversation.

The opportunity is to position Relay as the calm, focused alternative: enough structure to make feedback actionable, with none of the implementation burden associated with larger platforms. The page should convert intent created by content, search, referrals, or product-led comparisons into a low-friction trial start.

### Assumptions

- Visitors have experienced feedback in multiple channels—email, support tickets, calls, and chat—but do not yet have a shared system.
- The initial buying decision is made by a founder or product lead, with input from support and engineering.
- A free trial is the primary conversion; a secondary “See how it works” path serves cautious evaluators.
- Relay can credibly offer short setup, transparent pricing, integrations, and exportable data.

## Goals and success metrics

### Design goals

- Communicate Relay’s category and value proposition within the first viewport.
- Make the workflow tangible: collect → understand → prioritize → close the loop.
- Build trust before asking for an account through proof, transparent pricing, and specific product language.
- Give high-intent visitors a persistent, unambiguous path to start a trial.
- Keep cognitive load low: one primary CTA, one secondary action, and progressive detail.

### Success metrics

The following are measurement targets for launch, not historical results:

| Funnel stage | Metric | Target / signal |
|---|---|---|
| Awareness | Hero comprehension in a five-second test | 80% of participants can describe Relay and its audience |
| Engagement | Scroll depth to pricing | 55% of qualified visitors reach the pricing section |
| Consideration | Feature-to-pricing interaction rate | 20% engage with a feature detail or pricing toggle |
| Conversion | Trial-start rate from landing page | 6–10% of qualified sessions |
| Quality | Trial completion within 24 hours | 65% of trial starts create a first feedback board |
| Trust | CTA-to-demo split | At least 10% of CTA interactions choose the secondary walkthrough path, indicating a useful evaluation route |

Analytics should distinguish hero, navigation, pricing, and footer CTA clicks, while qualitative validation verifies whether the numbers represent comprehension rather than accidental taps.

## Target users and jobs-to-be-done

### Primary: product-led founder or product manager

- **Job:** “When requests arrive from everywhere, help me see patterns and decide what deserves attention without another complex tool.”
- **Pain:** Roadmap debates rely on the loudest customer, and evidence is difficult to retrieve.
- **Buying trigger:** A launch, churn risk, or growing request volume exposes the limits of a shared spreadsheet.

### Secondary: customer success or support lead

- **Job:** “When I hear the same issue repeatedly, help me capture it once, route it internally, and show customers that it was heard.”
- **Pain:** Feedback disappears into tickets; follow-up is manual and inconsistent.
- **Buying trigger:** Rising ticket volume or repeated requests for product updates.

### Influencer: engineer or operations partner

- **Job:** “Give implementation enough context to act without another clarification loop.”
- **Pain:** Requests lack source, frequency, impact, and ownership.

## Current-state and research observations

This concept uses competitive message review, SaaS heuristics, and assumption-led interviews; confirm the observations in validation.

- Category pages tend to lead with abstract claims such as “voice of the customer,” leaving visitors to infer the actual workflow.
- Buyers scan headings, proof points, pricing, and CTA labels before reading feature copy in full.
- Testimonials are more credible when they name a role and outcome rather than praise the product generally.

Core hypothesis: **a concrete end-to-end story, paired with transparent pricing and role-specific proof, will outperform a feature inventory.**

## Design decisions and rationale

1. **Outcome-led hero.** The headline “Turn customer feedback into your next clear decision” explains the benefit without pretending Relay replaces product judgment. Supporting copy names the audience and removes setup fear.
2. **Single primary CTA.** “Start free” is used consistently in the navigation, hero, pricing, and closing CTA. “See how it works” is secondary and supports evaluation without competing visually.
3. **Workflow before feature grid.** A three-step visual—capture, connect, prioritize—makes the product legible before individual capabilities are introduced.
5. **Pricing in the decision path.** Pricing appears after value and proof, not hidden behind a sales gate. A monthly/annual toggle is explicit, with annual savings stated in plain language.
6. **Role-specific social proof.** Testimonials identify a person’s role and a measurable operational change, such as fewer duplicate requests or faster weekly triage.
7. **Objection-handling FAQ.** Questions address setup time, integrations, data ownership, and team size—the practical blockers most likely to delay a trial.

## Information architecture and user flow

**Entry → orient → believe → evaluate → act**

1. Visitor enters from a referral, search result, or product comparison.
2. Hero establishes the category, audience, benefit, and primary action.
3. Workflow section demonstrates how Relay turns raw feedback into a decision.
4. Feature sections explain the mechanisms: capture from any channel, tag and group themes, prioritize with context, and close the loop.
5. Social proof validates the workflow for similar teams.
6. Pricing answers commitment and scalability questions.
7. FAQ resolves remaining objections.
8. Closing CTA repeats the trial promise and returns the visitor to the account-start action.

## Detailed screen and page layout breakdown

### 1. Global header — 80 px high

A centered 1200 px container holds the wordmark, three anchor links, and “Start free.” The header becomes sticky after the hero, with a subtle scroll border and 2 px active-section rule.

### 2. Hero — 680 px minimum height

The hero uses a 7/5 split. Left: eyebrow, two-line headline, support copy, CTA pair, and “Free 14-day trial · No credit card.” Right: a product story card showing an incoming request, grouped theme, and priority decision. A proof strip closes the viewport.

### 3. Workflow — 420 px

Heading: “Make feedback useful at every step.” Three equal cards show **Capture**, **Connect**, and **Prioritize**, each with a marker, explanation, and example.

### 4. Feature narrative — approximately 900 px

Three alternating rows create rhythm:

- **Capture anywhere:** a request inbox and lightweight share link; emphasize source retention.
- **Find the signal:** tags, duplicate grouping, and theme counts; emphasize pattern recognition.
- **Move with confidence:** owner, priority, and status; emphasize a decision that can be communicated.

Each row has a heading, short explanation, proof point, and framed illustration using the same sample request.

### 5. Social proof — 360 px

A pale-blue band contains one prominent testimonial and two compact snippets, each with role, company descriptor, and specific result. Placeholder logos must be labeled in concept work and replaced with verified customer permission in production.

### 6. Pricing — 620 px

Heading: “Start small. Keep the context.” Two cards compare **Starter** and **Team**, with a monthly/annual toggle, limits, included features, and one CTA per card. Avoid preselected upgrades, hidden taxes, or “contact us” for core plans.

### 7. FAQ and final CTA — 520 px

Four accordion questions sit beside a closing panel repeating “Bring every request into focus,” the “Start free” CTA, and trial reassurance. Footer includes privacy, terms, contact, and status.

## Design system

### Typography

Use **Inter** for interface and body text; headings use 600 and labels 500. H1 is 64/68 px, H2 40/48 px, H3 24/32 px, body 16/24 px, and metadata 13/18 px. Limit paragraph measure to 58–64 characters.

### Color tokens

| Token | Value | Use |
|---|---|---|
| Ink 950 | `#13202B` | Headlines, primary text, header wordmark |
| Ink 700 | `#42515D` | Body copy, secondary controls |
| Canvas 50 | `#FCFBF7` | Main page background |
| Surface 0 | `#FFFFFF` | Cards and pricing surfaces |
| Relay 600 | `#1769E0` | Primary CTA, links, focus ring |
| Relay 100 | `#E8F1FF` | Proof bands, selected states |
| Mint 500 | `#43B99A` | Success, “captured” status |
| Line 200 | `#DDE3E7` | Dividers, card borders |
| Danger 600 | `#B93838` | Error and destructive messaging |

Color is never the only status signal. Pair it with text, iconography, or shape.

### Spacing, grid, and components

Use a 4 px base spacing scale: 4, 8, 12, 16, 24, 32, 48, 64, 80, and 96. The desktop grid is a 12-column, 1200 px content area with 24 px gutters and 32 px outer breathing room at smaller desktop widths. Section padding is 96 px vertically, reduced to 64 px below 1200 px viewport width. Cards use 16–24 px internal padding, 12 px corner radius, and a 1 px line border.

Core components are: wordmark/header, button, text link, proof badge, workflow card, feature story row, interface illustration frame, testimonial, pricing card, toggle, accordion, and footer link group. Buttons have 48 px height, 12 px horizontal padding minimum, and a 10 px radius.

### States and accessibility

Define default, hover, pressed, focus-visible, disabled, loading, success, and error states for interactive components. Focus-visible uses a 3 px Relay 600 outer ring with 2 px contrast from the component edge. Body text and controls target WCAG AA contrast; do not place Ink 700 on Relay 100 for small text without checking contrast. Heading order follows page hierarchy, accordion buttons expose expanded state, and decorative illustrations are hidden from assistive technology while meaningful examples receive concise alt text. Keyboard users can reach every CTA, toggle, accordion, and anchor in logical order.

## Auto-layout and Figma implementation guidelines

Build around content, not fixed text boxes. Use vertical auto layout for sections/cards; text fills a readable maximum. Buttons use horizontal auto layout with hug contents and a minimum height. Pricing cards fill equally; illustrations preserve a minimum aspect ratio.

Create variables for color, spacing, radius, and type. Name properties for variant, icon visibility, state, and emphasis. Group illustration layers by request, metadata, status, and action. Pin header controls to container edges; let hero artwork scale from its right edge. Prototype anchors, pricing toggle, accordion, hover, and focus states with fast, non-blocking transitions.

## Detailed Figma canvas layout

Use a 1440 × 5200 px desktop page frame with a 1200 px centered grid. Organize the canvas left to right by intent, then top to bottom by fidelity:

| Section name | Position / size | Ordering and contents |
|---|---:|---|
| `00_Cover_And_Notes` | x=0, y=0; 1440 × 360 | Project title, hypothesis, owner, version, and reading instructions |
| `01_Research_And_Content` | x=1600, y=0; 1200 × 920 | Assumptions, audience jobs, message hierarchy, approved content outline |
| `02_Foundations` | x=2960, y=0; 1200 × 920 | Type ramp, tokens, spacing scale, grid, accessibility notes |
| `03_Flow_And_Wireframes` | x=0, y=560; 1440 × 1500 | User flow at top; low-fidelity desktop frames below, ordered hero → CTA |
| `04_Components` | x=1600, y=1080; 1200 × 1500 | Buttons, nav, cards, pricing, FAQ, states, and responsive behavior notes |
| `05_High_Fidelity_Desktop` | x=0, y=2260; 1440 × 5200 | One long page frame at 1440 × 5200; section dividers and measurement annotations outside the frame |
| `06_Interaction_States` | x=1600, y=2700; 1200 × 1300 | Hover, focus, pressed, pricing toggle, expanded FAQ, and error examples |
| `07_Validation_And_Handoff` | x=2960, y=1080; 1200 × 1800 | Test prompts, issue log, final decisions, content checklist, and export notes |

Within `05_High_Fidelity_Desktop`, name landmarks `Hero`, `Workflow`, `Feature_01_Capture`, `Feature_02_Signal`, `Feature_03_Decide`, `Social_Proof`, `Pricing`, `FAQ`, `Final_CTA`, and `Footer`. Keep 80 px between landmarks, annotations outside the frame, and layers ordered background → decoration → content → overlays.

## Validation and testing plan

1. **Five-second comprehension test:** Show only the hero for five seconds. Ask what Relay does, who it is for, and what action is available.
2. **Unmoderated first-click test:** Ask participants to find pricing, explain the three-step workflow, and start a trial without submitting personal details.
3. **Content preference test:** Compare outcome-led hero copy with a feature-led alternative; measure comprehension and confidence, not just preference.
4. **Prototype usability sessions:** Test five product leaders and three support leads. Observe navigation, pricing interpretation, and the transition from proof to CTA.
5. **Accessibility review:** Keyboard-only pass, screen-reader landmark check, contrast audit, zoom to 200%, and reduced-motion review.
6. **Launch experiment:** Instrument CTA clicks, pricing toggle use, FAQ expansion, trial completion, and qualified conversion; test one placement variable at a time.

Success criteria are: participants can restate the value proposition, locate pricing, distinguish Starter from Team, and explain the next step without facilitator help.

## Outcomes and expected impact

No production metrics are claimed. **Expected impact** is a clearer first impression, stronger signup trust, and a more qualified trial funnel. The reusable workflow, feature, pricing, and CTA patterns can support future comparison, integration, and use-case pages.

## Ready-to-publish GitHub README section

### Problem
Teams collect valuable customer feedback across email, support, calls, and chat, but lack a lightweight way to turn repeated requests into shared product decisions.

### Solution
Relay is positioned as a focused feedback workspace. The landing page explains the loop—capture feedback, connect recurring themes, and prioritize with context—through proof, transparent pricing, and a low-friction trial.

### User flow
Visitor arrives → understands Relay in the hero → sees the capture/connect/prioritize workflow → reviews concrete features → reads role-specific proof → compares Starter and Team pricing → resolves objections in FAQ → starts a free trial.

### Key highlights

- Outcome-led hero with a consistent “Start free” CTA.
- Continuous product story from incoming request to prioritized decision.
- Transparent pricing designed for small-team evaluation.
- Social proof that names roles and operational outcomes.
- Accessible states, keyboard-first interactions, and a documented desktop grid.
- Canvas organization that makes strategy, components, high fidelity, and validation easy to review.

## Portfolio presentation checklist

- [ ] Lead with the problem and the audience, not the visual style.
- [ ] Show the hero and one complete workflow story before displaying isolated screens.
- [ ] Explain why pricing appears where it does and how the CTA hierarchy reduces friction.
- [ ] Include the research observations and label assumptions versus validated findings.
- [ ] Present at least one alternate direction or rejected choice with its rationale.
- [ ] Show responsive intent, accessibility states, and content behavior—not only the polished desktop frame.
- [ ] Use realistic, permissioned proof; mark all concept testimonials and logos clearly.
- [ ] Label targets and expected impact so no unmeasured result is presented as fact.
