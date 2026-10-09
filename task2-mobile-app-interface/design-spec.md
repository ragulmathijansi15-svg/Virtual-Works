# Task 2 Design Specification — Momentum Mobile App

## Product design direction

Momentum is a focused task-management app for people who need a realistic plan, not an endless backlog. The interface uses a warm neutral canvas, cobalt action color, mint completion state, and compact task surfaces that make the next action easy to scan.

## Design tokens

### Typography

- Typeface: Inter or platform-native equivalent.
- Display: 28/34, 700.
- Screen title: 24/30, 700.
- Section title: 18/24, 600.
- Body: 16/24, 400.
- Label: 14/20, 600.
- Caption: 12/16, 500.
- Numeric emphasis: 20/24, 700.

### Color

| Token | Value | Use |
|---|---|---|
| `ink-900` | `#18212B` | Primary text |
| `ink-600` | `#5B6875` | Secondary text |
| `canvas` | `#F7F8FA` | App background |
| `surface` | `#FFFFFF` | Cards and sheets |
| `primary-600` | `#315BEA` | Primary action and selected states |
| `primary-100` | `#E9EEFF` | Soft selected backgrounds |
| `mint-600` | `#198A65` | Completed state |
| `amber-600` | `#B56B16` | Due-soon state |
| `red-600` | `#B83A45` | Destructive/error state |
| `line-200` | `#DEE3EA` | Dividers |

### Spacing and geometry

Use a 4px base scale: 4, 8, 12, 16, 20, 24, 32, 40. Default mobile page padding is 16px. Cards use 16px padding and 12px radius. Bottom sheets use 20px top radius. Controls are at least 44px tall; primary buttons are 48px tall.

## Mobile component guide

### App shell

Top bar contains the current screen title, optional contextual action, and a consistent safe-area inset. Bottom navigation has four destinations: `Today`, `Tasks`, `Focus`, and `Profile`. The selected destination uses icon + label, not color alone.

### Task row

An accessible checkbox, task title, optional project label, due metadata, and overflow action. The row supports default, completed, overdue, selected, loading, and error states. Swipe actions are progressive enhancements; every action is also available from the overflow menu.

### Task card

Use for Today priority tasks. Include a clear title, time estimate, due cue, project color marker, and one primary action. Avoid multiple competing icons in the first scan line.

### Priority and project chips

Chips are 32–36px high with visible selected and focus states. Long labels truncate with accessible full text. Use chips for filtering, not as the only way to change a task’s priority.

### Focus timer

Large timer, session label, start/pause control, progress indicator, and a secondary `End session` action. Ensure the timer remains understandable without relying on animation or color.

### Bottom sheet

Use for create/edit task, filters, and task details. Sheets have a visible drag handle, title, close action, logical focus trap, and a full-screen fallback for small devices.

### Toast and feedback

Use for reversible confirmations such as `Task completed — Undo`. Announce status changes to assistive technology and keep the toast visible long enough to read.

## Navigation and interaction rules

- Preserve scroll position when returning from task detail.
- Use optimistic completion with an undo affordance.
- Never delete immediately without a confirmation or undo window.
- Keep create-task available from Today and project views.
- Use empty states that explain the next useful action instead of celebrating emptiness.
- Support Dynamic Type / font scaling and test the longest realistic task title.

## Accessibility checklist

Target WCAG 2.2 AA intent. Provide 44px minimum targets, visible focus, VoiceOver/TalkBack labels, sufficient contrast, reduced-motion behavior, logical reading order, keyboard support when used on tablets, and non-color indicators for overdue/completed status.

## Auto-layout and Figma rules

Use vertical auto-layout for screens, horizontal auto-layout for task metadata, and nested components for icon-label pairs. Set text to hug height and fill width. Create variants for task status, priority, and loading. Design at 390px first, then verify 320px and 430px widths. Keep fixed bottom navigation outside the scroll frame and document safe-area behavior.
