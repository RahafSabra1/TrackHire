# TrackHire

**A shared hiring pipeline for QSTP internships — built for the "Build for QSTP" Internship Program Challenge (Challenge 3: Hiring Funnel Black Box).**

TrackHire replaces informal WhatsApp/email hiring updates with one shared board, tracking every candidate from Nomination through Interview, Offer, and Onboarding — while adding three intelligent layers: a Hiring Health Score for startup accountability, an AI Rejection Assistant that closes the feedback loop, and Duplicate Acceptance Detection to protect fairness across the program.

---

## How to Run This

This is a **frontend-only prototype** — no backend, no database, no installation required. Everything runs directly in the browser on mock data.

**To view it:**
1. Clone or download this repository
2. Open `HTML/login.html` in any modern browser (Chrome, Edge, Safari, Firefox)
3. Choose a role on the login screen:
   - **Startup** → goes to the Startup Dashboard, Pipeline, Feedback, and Score screens
   - **QSTP Administrator** → goes to the QSTP Dashboard, Startup Details, and Reports screens
4. Any email/password combination will log you in — there's no real authentication, this is a hackathon prototype

No `npm install`, no server, no setup. Just open the HTML file.

---

## Pages & What They Do

| Page | File | Who it's for | What it shows |
|---|---|---|---|
| Login | `HTML/login.html` | Everyone | Role selection (Startup / QSTP Admin) |
| Startup Dashboard | `HTML/startup-dashboard.html` | Startups | Startup's own job posting + quick links |
| Pipeline Board | `HTML/pipeline.html` | Startups & QSTP staff | Kanban-style candidate tracker: Nominated → Interviewed → Offer → Onboarded, with stall detection and search |
| Feedback / Rejection Assistant | `HTML/feedback.html` | Startups | AI-suggested rejection reasons based on the job description, one-click send |
| Score Breakdown | `HTML/score.html` | Startups | A startup's own Hiring Health Score and how to improve it |
| QSTP Dashboard | `HTML/qstp-dashboard.html` | QSTP staff | Leaderboard ranking all startups by Hiring Health Score |
| Startup Details | `HTML/startup-details.html` | QSTP staff | Drill-down into one startup's score breakdown, reached via "View Details" on the QSTP Dashboard |
| Program Impact Report (Future work) | `HTML/reports.html` | QSTP staff | Program-wide metrics: avg. time-to-hire, time saved, rejection reason breakdown, duplicate conflicts caught |

---

## Key Features

1. **Shared Pipeline Board** — real-time candidate status visible to both QSTP and startups, no more chasing emails
2. **Hiring Health Score** — scores each startup on responsiveness, feedback completion, offer speed, and onboarding completion
3. **AI Smart Rejection Assistant** — reads the job description, suggests specific rejection reasons, drafts and sends a respectful message in one click
4. **Duplicate Acceptance Detection** — flags QSTP staff (only) if a candidate has accepted two active QSTP-linked offers at once
5. **Program Impact Report (Future work)** — proves the tool's impact with real metrics: time-to-hire, time saved, rejection reasons, conflicts caught

---

## Tech Stack

- **Frontend:** HTML, CSS, JavaScript — no framework, no build step
- **Data:** structured mock data hardcoded per page (no backend/database) — deliberate choice to keep the prototype demoable in the hackathon's 48-hour window
- **AI layer (conceptual/planned):** the Rejection Assistant and stall-detection logic are designed around a bilingual (Arabic/English), Gulf-calendar-aware AI agent for time and structured-requirement reasoning — see the PRD for full detail on the intended production integration

---

## Team

TrackHire — Rahaf, Sally, Shahd

Built for the QSTP "Build for QSTP" Internship Program Challenge, July 2026.
