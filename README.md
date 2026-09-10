# BSL Ready — by cSeeker

**Tagline:** Book BSL support with confidence.

BSL Ready is a free, beginner-friendly interactive checklist for organisations and individuals who have never booked British Sign Language (BSL) interpreting support before.

## What the site does

- Walks a first-time booker through 9 simple questions.
- Checks whether the core booking information is ready.
- Produces a readiness percentage and missing-information checklist.
- Flags assignments where the interpreting provider should review whether a team may be appropriate.
- Creates a pre-filled email enquiry to `bookings@cseeker.co.uk` from the user's answers.
- Uses plain UK English and a mobile-first, keyboard-friendly design.

## Brand

- Product: **BSL Ready**
- Endorsement: **by cSeeker**
- Tagline: **Book BSL support with confidence.**
- Main colour: deep violet `#5927E8`
- Accent: accessible warm yellow `#FFD84D`
- Dark text/background: `#171B2E`
- Background: `#F7F8FB`

## Analytics events

The front-end emits these events:

- `checklist_start`
- `checklist_step_view`
- `checklist_complete` with `readiness_score`
- `quote_click`
- `checklist_restart`

For development, event counts are also stored in the visitor's own browser under the localStorage key `bslReadyDemoAnalytics`. **This is not aggregate analytics and must not be presented as total users.**

For real cross-user reporting, connect an analytics service such as GA4 or Plausible. The site already pushes events to `window.dataLayer` when available and also emits `bslready:analytics` custom browser events, so another analytics provider can be wired in without rewriting the checklist.

Recommended dashboard measures:

1. Unique visitors
2. Checklist starts
3. Completion rate
4. Average readiness score
5. Quote clicks
6. Start-to-quote conversion rate
7. Step drop-off rate
8. Returning users

Do not send the user's actual checklist answers to analytics unless the privacy notice and lawful basis have been reviewed. The current version keeps answers in the browser and only transfers them when the visitor deliberately opens the pre-filled email to cSeeker.

## Hosting

This is a static site (`index.html`, `styles.css`, `app.js`) and can be hosted using GitHub Pages, Vercel, Netlify or cSeeker's existing web host.

## Suggested next version

- Add cSeeker's final logo assets and exact brand fonts/colours.
- Connect aggregate analytics.
- Add a BSL introduction video.
- Add an optional contact form/API instead of mailto.
- Create an admin dashboard for real funnel data.
- Add a downloadable/printable booking summary.
- Add organisation-specific pathways for events, healthcare, education and workplaces.

## Important wording

BSL Ready is guidance, not a rule engine. It should not state that a fixed duration automatically requires a fixed number of interpreters. Duration, complexity, setting, breaks, preparation, the Deaf person's preferences and other factors can affect the appropriate provision. The interpreting provider should confirm the support required.
