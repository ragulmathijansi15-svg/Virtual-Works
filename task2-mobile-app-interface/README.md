# Momentum — Mobile App Interface Design

> A complete mobile productivity and task-management app concept for turning daily intentions into a calm, achievable plan.

## 1. Project snapshot

| Attribute | Details |
|---|---|
| **Role** | Product strategist and UI/UX designer: research framing, IA, interaction design, visual system |
| **Scope** | Task model, core flows, mobile screens, states, accessibility, validation, and presentation system |
| **Platform** | iOS-first mobile app; 390 × 844 pt reference viewport, with Android-ready principles |
| **Timeline** | 3-week concept sprint: structure (days 1–4), interface (days 5–11), validation and case study (days 12–15) |
| **Deliverables** | Product brief, user flows, 12 screens, states, tokens, components, prototype-ready canvas, test plan |
| **Status** | Design specification and case study; no production code or claimed Figma file |

## 2. Problem, opportunity, and assumptions

Task managers often make planning feel like another task. People capture work in scattered notes, underestimate available time, and then face a dense list with no clear next step. Most tools optimize for storing and configuring tasks rather than helping someone decide what is realistic today; overdue items can also create guilt.

**Opportunity:** design a focused companion for the question, “What can I realistically move forward today?” Momentum makes capture frictionless, turns a backlog into a time-aware plan, and provides progress without distracting gamification.

**Assumptions**

- The primary user balances work, personal, and recurring responsibilities but does not need enterprise project management.
- A phone is used for quick capture and check-ins; longer planning happens in short weekly sessions.
- Users will trust scheduling suggestions when the reasoning is visible and manual control remains available.
- Calendar availability is useful but optional; the first experience must work without connected accounts.
- Completion means a meaningful next action moved forward, not necessarily an entire project finished.
- Notifications should be selective and user-controlled.

## 3. Goals and success metrics

**Product goals:** capture a task in under 10 seconds; make the next action obvious; turn backlog into a manageable plan using time, energy, and priority; preserve context through subtasks and notes; make progress visible without pressure.

| Metric | Target / signal | Evaluation |
|---|---|---|
| First-task completion | 80% create and complete one task in session one | Moderated test and funnel |
| Capture speed | Median basic task creation under 10 seconds | Prototype timing |
| Plan confidence | 4/5 average to “I know what to do next” | Day-one pulse |
| Plan adherence | 60% of planned tasks completed or intentionally rescheduled in 7 days | Pilot telemetry |
| Findability | 90% locate an overdue or scheduled task unaided | Task-based test |
| Accessibility | Zero critical touch, contrast, or assistive-technology failures | Manual audit |

These are **targets**, not measured outcomes.

## 4. Target users and jobs-to-be-done

**Primary: the overloaded knowledge worker.** A 25–40-year-old professional or student balancing projects, meetings, and personal commitments. They are comfortable with mobile apps, but their system is split among notes, calendar reminders, and mental notes.

**Secondary: the recovering list-maker.** Someone who has accumulated hundreds of tasks and now avoids opening the app. They need a fresh start, forgiving rescheduling, and a smaller daily surface.

**Jobs to be done**

- When I remember something mid-task, capture it instantly so I can return to what I was doing.
- When my day begins, show me what matters today so I can start without sorting a backlog.
- When a task feels too large, suggest a next step so progress feels actionable.
- When plans change, let me reschedule without feeling that I failed.
- When I finish work, give me a quick reflection that helps tomorrow.

## 5. Current-state and research observations

This concept is grounded in a lightweight comparative review of common mobile task-manager patterns and five assumed discovery conversations. These are directional hypotheses to validate, not claims of completed research.

- Capture is fast, but the resulting task often lacks a clear date, duration, or next action.
- Users distinguish “important” from “urgent,” yet many products collapse both into one flag.
- A long list creates choice paralysis; a short Focus set is easier to act on while the backlog remains accessible.
- Rescheduling is common and should be a first-class action, not a hidden edit.
- People need context at execution: expected duration, energy, location, and notes.
- Progress motivates when it shows meaningful movement; streaks can punish unpredictable schedules.

## 6. Design decisions and rationale

- **Today-first home:** “Focus,” “Up next,” and “Later today” reduce the cognitive load of a full backlog.
- **Progressive-detail Quick add:** title is required; date, duration, energy, project, and reminder are optional chips. Basic capture stays fast without losing planning depth.
- **Three priority levels:** “Must,” “Should,” and “Could” communicate consequence more naturally than a five-star system and work with time and energy cues.
- **Task detail as workbench:** notes, subtasks, links, and activity stay in one predictable sheet so context is not lost.
- **Gentle rescheduling:** “Tomorrow,” “This week,” and “Choose date” are prominent after a missed task. Copy is neutral and undo is available.
- **Explainable scheduling:** Plan states why a suggestion appears, such as “30 min available before 11:00,” and always permits manual override.
- **Four destinations:** Today, Plan, Inbox, and Insights stay in bottom navigation; Settings is behind Profile.
- **Calm visual hierarchy:** warm neutral canvas, one accent, restrained borders, and generous whitespace create support rather than urgency.

## 7. Information architecture and user flow

**Navigation:** Today → current focus; Plan → week and scheduling; Inbox → uncategorized captures; Insights → patterns and wins; Profile → preferences, integrations, notifications, accessibility.

**Core flow:** Open app → Today → Add → enter title → optional planning chips → Save → task appears in Inbox or Today → Start → Complete / Snooze / Edit → feedback → next task.

**Planning flow:** Today → Plan → choose date → review suggested Focus set → adjust duration or priority → confirm → Today reflects the plan.

**Exception flow:** Task due → Snooze → Tomorrow / This week / Date → Confirm → task leaves current focus with a reschedule label; Undo remains available for 5 seconds.

## 8. Detailed screen and layout breakdown

Every screen uses a 24 pt horizontal safe-area margin, an 8 pt column gutter, and an 80 pt bottom-navigation zone where applicable.

| Screen | Layout and behavior |
|---|---|
| **Welcome / setup** | Brand, value proposition, “Start with a sample plan,” and optional notification/calendar permissions after value is demonstrated. |
| **Today** | Greeting and date; progress ring; Focus card with up to three tasks; Up next list; Add button; bottom navigation. |
| **Quick add sheet** | Autofocus title field, voice affordance reserved for future scope, date/duration/priority chips, Save, and “Add another.” Expand only on demand. |
| **Inbox** | Items grouped by age with schedule, project, complete, and delete actions. Banner explains Inbox is temporary. |
| **Plan / week** | Seven-day selector, available-time summary, explainable suggestion, and movable task blocks; non-drag controls also exist. |
| **Task detail** | Completion control, title, metadata, duration, priority, subtasks, notes, links, reminder, activity, and sticky Start/Complete/Reschedule action. |
| **Focus mode** | Minimal execution view: task title, next subtask, notes preview, pause/complete, and exit; no forced timer method. |
| **Reschedule sheet** | Neutral prompt, three recommended choices, date/time picker, optional reason, Confirm, and undo. |
| **Project view** | Project title, progress, next milestone, task sections, and color marker; project controls remain secondary. |
| **Insights** | Weekly trend, planned-versus-finished ratio, productive time/energy pattern, and one reflection prompt; no rankings. |
| **Empty states** | Today offers “Plan one small win”; Inbox says “Nothing waiting”; Project offers “Add the next action.” One primary action each. |
| **System states** | Content-shaped loading; offline capture with sync label; errors preserve entered text; delete confirms or offers undo. |

## 9. Design system

### Typography

Use Inter or the platform system sans with Dynamic Type. Greeting: 28 pt semibold/34 line height. Screen title: 22/28 semibold. Card title: 17/22 semibold. Body: 16/24 regular. Metadata: 13/18 medium. Button label: 15/20 semibold.

### Color tokens

| Token | Value | Usage |
|---|---|---|
| `Canvas` | #F8F7F4 | App background |
| `Surface` | #FFFFFF | Cards and sheets |
| `Ink` | #1F2421 | Primary text/icons |
| `Muted` | #66706A | Secondary text |
| `Line` | #E3E6E1 | Dividers |
| `Momentum` | #2F7D68 | Actions, progress, selected state |
| `Momentum tint` | #DCEFE8 | Soft emphasis |
| `Must / Should / Could` | #B84C45 / #B9782B / #5E75A5 | Priority indicators |
| `Focus wash` | #FFF4D8 | Non-critical attention cue |

Check text combinations against WCAG AA; never use color alone to convey meaning.

### Spacing, grid, and components

Use a 4 pt base unit: 4, 8, 12, 16, 20, 24, 32, 40. Standard card padding is 16 pt; major sections use 24 pt separation. Minimum touch target is 44 × 44 pt. Cards use 12 pt radius, sheets 16 pt, and pills only for compact metadata. Core components are App bar, bottom navigation, task row, priority and metadata chips, progress ring, buttons, text field, date picker, sheet, toast, empty state, and confirmation dialog.

Each interactive component defines default, pressed, focused, disabled, loading, selected, error, and success states. Task rows support complete, snooze, edit, and undo; swipe is never the only path.

### Accessibility

Support Dynamic Type, VoiceOver/TalkBack labels, logical reading order, reduced motion, high contrast, visible focus, and 16 pt-or-larger body text. Do not rely on drag-and-drop in Plan; provide Move earlier/later controls. Announce completion and undo status. Test the largest text size for clipping and reflow.

## 10. Auto-layout and Figma implementation guidelines

Build screens from nested vertical and horizontal auto-layout frames, not absolute positioning. Use fixed viewport shells, fill-container content, hug contents for labels/buttons, and minimum widths for controls. Treat card padding and internal gaps as component properties. Create variants for task status, priority, density, and theme; expose text, icon visibility, completion, and metadata as properties.

Reuse one task-row component across Today, Inbox, Project, and Plan. Define pressed, focus-visible, disabled, and loading states. Test the 390 × 844 reference frame and a 375 × 667 frame for wrapping. Name layers by function, such as `Today / Focus / Task row / Title`. Keep source components centralized; presentation frames use instances only.

## 11. Detailed Figma canvas layout

Coordinates use the canvas top-left as origin. Sections run left-to-right by journey and top-to-bottom by fidelity.

| Section | Position and frames | Ordering |
|---|---|---|
| **00 — Cover & brief** | x=0, y=0; 1200 × 900 | Cover, snapshot, principles, scope |
| **01 — Foundations** | x=1400, y=0; 1200 × 1100 | Tokens, type, spacing, grid, accessibility |
| **02 — IA & flows** | x=2800, y=0; 1600 × 1200 | Navigation, capture, planning, exception flows |
| **03 — Wireframes** | x=0, y=1400; twelve 390 × 844 frames in 4 × 3 grid | Welcome through system states |
| **04 — Core UI** | x=1900, y=1400; twelve 390 × 844 frames in two rows | Same screens at final fidelity, primary-flow order |
| **05 — Components** | x=0, y=4300; 1400 × 1300 | Masters, variants, states, annotations |
| **06 — Prototype & validation** | x=1700, y=4300; 1800 × 1300 | Route map, test tasks, findings template |
| **07 — Presentation selects** | x=3900, y=1400; 1500 × 2600 | Hero, flow strip, detail, system board, a11y callouts |

Use 80 pt section gutters and 40 pt frame gutters. Name and order screens by user mental model, not design chronology.

## 12. Validation and testing plan

Recruit 6–8 participants across both audiences for a clickable prototype. Test capture of “send the renewal form,” planning around a 30-minute window, breaking “prepare presentation” into a next action, completing a task, and rescheduling a missed item. Observe first click, hesitation, terminology, and recovery.

Run VoiceOver/TalkBack, largest-text, contrast, reduced-motion, offline-capture, and failed-sync passes. Test that errors never discard entered text. After iteration, use at least 20 unmoderated participants to measure capture time, first-plan completion, plan confidence, findability, and reschedule completion.

**Iteration gates:** Can users capture and find a task unaided? Can they understand and change the Focus logic? Can they recover from missed work without anxiety or data loss? Can assistive-technology users complete the same loop?

## 13. Outcomes and impact

No live-product measurements are available because Momentum is a design concept. **Expected impact:** reduce decision fatigue through a small explainable Focus set, improve follow-through by attaching duration and next actions, and make rescheduling constructive. The metrics above are future pilot targets, not shipped performance.

## 14. Ready-to-publish GitHub README section

### Problem

People capture responsibilities across notes, calendars, and messages, then face an overwhelming list with little help deciding what is realistic today. Many task apps add configuration without reducing cognitive load.

### Solution

Momentum is a calm, iOS-first productivity app that turns a backlog into a time-aware daily plan. It combines fast capture, a focused Today view, transparent scheduling suggestions, meaningful priorities, and forgiving rescheduling. Task detail preserves the context needed to execute.

### User flow

Capture in Quick add → triage in Inbox or assign to Today → review the explainable Focus set in Plan → start the next action → complete, snooze, or reschedule → review lightweight progress in Insights.

### Key highlights

- Today-first hierarchy limits choice paralysis without hiding the backlog.
- Progressive-detail capture supports a basic task in under 10 seconds.
- Must/Should/Could priorities pair with duration and energy.
- Rescheduling is normal, reversible, and neutral in tone.
- Reusable states and accessibility requirements are specified up front.
- Offline-aware and error-resilient interactions protect user trust.

## 15. Portfolio presentation checklist

- [ ] Open with problem, audience, and one-sentence design thesis.
- [ ] Show Today early and explain how it reduces decision fatigue.
- [ ] Show the complete capture-to-completion flow, not isolated screens.
- [ ] Annotate decisions with the user problem they solve.
- [ ] Show hierarchy, spacing, type, component states, and accessibility examples.
- [ ] Include empty, offline/error, and reschedule states.
- [ ] Label assumptions and unmeasured outcomes explicitly.
- [ ] End with validation questions and the next iteration.
- [ ] Check captions, headings, links, and artifact labels before publishing.
