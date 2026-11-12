# MAJU Student Portal – Redesign Concept

**Team:** _add your names here_

A frontend-only redesign of a university student portal. It is an **unofficial concept** and is not connected to, or endorsed by, Muhammad Ali Jinnah University.

- **Audience:** university students checking their academic status.
- **Primary task:** see at a glance what needs attention (attendance, fees, deadlines), then act on it.

## Roles (switch with the Student / Teacher control)
- **Student:** Dashboard, My courses, Assignments (submit work), Study planner (focus timer, weekly study timings, focus mode), Attendance, Results, Fees, Schedule, Announcements.
- **Teacher (fictional instructor):** Dashboard, Assignments (create, review submissions, grade with feedback), Attendance (mark present/absent), Announcements (post to students).
- Shared in-memory data: an assignment a teacher posts appears for the student, a student's submission appears for the teacher, and grades flow back.

## Working interactions
- Attendance simulator: add missed classes and watch the percentage and warning update.
- Fees: "Pay now" opens a simulated confirmation and marks the item paid with a demo voucher.
- Announcements: filter by category, expand to read, unread count updates.
- Focus timer (Focus, break and a 10-second demo mode) with a daily study goal.
- 3D and motion: rotating cube, card tilt, animated page transitions (all switched off with reduced-motion settings).
- Results semester picker, schedule day picker, light/dark theme.

## Sample data
All names, IDs, courses, grades, fees and announcements are **fictional**. No real student, personal or health data. No backend, database, authentication or real payments.

## Assets and AI
- No images; emoji and CSS only. Fonts: Sora and DM Sans (Google Fonts, SIL OFL).
- Claude (Anthropic) generated the first version of the code and this README. _Add what your team checked or changed._

## Checks to run and record
- [ ] Mobile (~375px): bottom navigation works, no sideways scrolling
- [ ] Keyboard only: Tab through nav, chips, simulator, dialogs; Esc closes dialogs
- [ ] Contrast in light and dark theme
- [ ] Hosted link opened in a fresh/private window

## Run / host
Open `index.html`. For hosting: push to GitHub → Settings → Pages → deploy from `main`.

## Project structure
```
maju-portal/
├── index.html        page structure
├── assets/style.css  design system (light/dark themes, 3D cards, animations)
├── assets/app.js     data, views, interactions
└── README.md
```
Notifications bell, profile card, confetti on successful submit/grade/post, per-course colour bands and role-based colour themes are included. Confetti and all motion are disabled for reduced-motion users.
