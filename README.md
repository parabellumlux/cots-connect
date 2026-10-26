# COTS Connect

An agentic outreach and care-coordination app for **Church on the Street of Texas (COTS)**, a real Odessa street-ministry nonprofit: people in need text in, an AI agent triages and opens a care case, volunteers get coordinated by text, and nothing falls through the cracks.

Built for the OutSystems **"Build for the Future 2026"** hackathon (Taikai), November 2–9, 2026.
Beneficiary nonprofit: Church on the Street of Texas — all prize winnings go to COTS.

## The problem

Small street ministries run on goodwill, group texts, and memory. A cry for help lands in a volunteer's personal phone, between shifts and family life. Follow-ups depend on someone remembering. Needs get lost, duplicated, or answered too late — and the people who fall through the cracks are the ones with the least margin for it.

The barrier is not caring. It is coordination.

## How it works

| Module | What it does |
|---|---|
| **Text-a-Need intake** | A person texts the ministry number (Twilio). An AI agent converses in plain language, identifies the need (food / clothing / shelter referral / prayer / ride), urgency, location, and household size, and opens a structured care case in OutSystems ODC. |
| **Follow-up copilot** | The agent watches open cases and drafts the next step — a check-in text, a referral note, a volunteer reminder. **A human approves every outbound message before it sends.** The agent drafts; people decide. |
| **Volunteer & food-run coordinator** | Volunteers register once. The coordinator builds outreach runs and donation pickups, assigns them, and sends Twilio reminders. Completion is logged by replying "DONE" — no volunteer app to install. |
| **Impact dashboard** | People served, needs by type, follow-ups closed, response time from first text to first help — the grants-and-donors view. |

No app to install for the person in need. No form. No literacy barrier beyond sending a text.

## Stack

- **OutSystems ODC** — data model, case management, screens, Agentic AI tooling (intake conversation + follow-up copilot)
- **Twilio** — SMS intake, reminders, completion logging
- **Human-in-the-loop by design** — agents triage, draft, and watch; humans approve, decide, and show up

## Open source

COTS Connect is a template, not just an app. Any small church or street ministry can clone it, connect its own number, and stop losing people through the cracks. *Built for one ministry in Odessa, reusable by thousands.*

## Team

- **Diana Kathleen Pettigrew** (@ignisalgos2) — Project owner; co-founder, Ignis Algos; founding director, COTS
- **Damon Cory Pettigrew** (@parabellumlux) — Founder, Ignis Algos; president & organizer, COTS

## Status

- Taikai project: **Cots Connect** (Build for the Future 2026)
- Team Confirmation: Wednesday, October 28, 2026, 11:00 AM CT
- Kickoff: Monday, November 2, 2026 · Final submission: Monday, November 9, 2026, 4:59 PM CT
- **Development happens during the hackathon window (Nov 2–9, 2026).** Until kickoff this repo holds the concept, design, and documentation only — no application code, per the hackathon's rules.
- Concept video: https://www.youtube.com/watch?v=e2A8cj3EsWg
- Project site: https://cotsconnect.ignisalgos.com
- Docs: [concept memo](docs/concept.md) · [full project description](docs/project-description.md)

## License

MIT — see [LICENSE](LICENSE). The point of the license is the point of the project: take it, clone it, use it for your neighbors.
