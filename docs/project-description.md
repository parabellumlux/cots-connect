# COTS Connect

**An agentic outreach and care-coordination app for Church on the Street of Texas (COTS), a real Odessa street-ministry nonprofit: people in need text in, an AI agent triages and opens a care case, volunteers get coordinated by text, and nothing falls through the cracks.**

## The problem

Small street ministries run on goodwill, group texts, and memory. A person in crisis reaches out — a mother who needs food for her kids tonight, a man sleeping in his car who needs a shower and a lead on work — and that cry for help lands in a volunteer's personal phone, between shifts and family life. Follow-ups depend on someone remembering. Needs get lost, duplicated, or answered too late. The people who fall through the cracks are the ones with the least margin for it.

The barrier is not caring. It is coordination.

## The solution

COTS Connect gives a small ministry the coordination layer of a big agency, through the one tool every person in need already has: **text messaging**. No app to install, no form to fill out, no literacy barrier beyond sending a text.

A person texts the ministry number. An AI agent converses in plain language, identifies the need (food, clothing, shelter referral, prayer, a ride), its urgency, location, and household size, and opens a structured care case. From there, the system keeps watch: follow-ups are drafted, volunteers are assigned and reminded, and every case stays visible until it is closed by a human who helped.

**The agent drafts — people decide.** Every outbound message is approved by a human before it sends. The technology carries the memory and the follow-through; the ministry keeps the mercy.

## How it works — four modules

1. **Text-a-Need intake (Twilio + agent).** The front door. A person in need texts in; the agent triages the conversation and opens a structured care case in OutSystems ODC — need type, urgency, location, household size — ready for a human to act on.

2. **Follow-up copilot (agent, human-in-the-loop).** The agent watches open cases and drafts the next step: a check-in text, a referral note to a partner agency, a reminder to the assigned volunteer. A human approves every message before it goes out.

3. **Volunteer & food-run coordinator.** Volunteers register once. The coordinator builds outreach runs and donation pickups, assigns them, and sends Twilio reminders with the details. Completion is logged with a simple reply text ("DONE") — no volunteer app to install.

4. **Impact dashboard.** The numbers a ministry actually needs: people served, needs by type, follow-ups closed, response time from first text to first help. This is the grants-and-donors view — proof that the work happened and the help arrived.

## Built with

- **OutSystems ODC** — the application platform: data model, case management, screens, and the Agentic AI tooling presented at the Build for the Future 2026 kickoff, which powers the intake conversation and the follow-up copilot.
- **Twilio** — SMS is the front door and the nervous system: intake, reminders, and completion logging all run on text messages.
- **Agentic AI, human-in-the-loop** — agents triage, draft, and watch; humans approve, decide, and show up.

## The beneficiary

All prize winnings go to **Church on the Street of Texas (COTS)** — a Texas nonprofit corporation (Certificate of Formation filed July 2026, Odessa, TX) doing street-level ministry in the Permian Basin: food, clothing, prayer, and practical help for neighbors in crisis. COTS Connect is built for COTS first — and built to be cloned.

## Open source

COTS Connect is open source by design. What works for one small ministry in Odessa should work for thousands like it: any church or street ministry can pick up the template, connect its own number, and stop losing people through the cracks. **Built for one ministry in Odessa, reusable by thousands.**

## The team

- **Diana Kathleen Pettigrew** (ignisalgos2) — Project owner. Co-founder, Ignis Algos; founding director, Church on the Street of Texas.
- **Damon Cory Pettigrew** (parabellumlux) — Founder, Ignis Algos; president and organizer, Church on the Street of Texas.

Two people, one ministry, and a belief that the smallest organizations deserve coordination tools as good as the biggest — because the people they serve can't wait for a callback that never comes.

---

*Submitted to OutSystems "Build for the Future 2026" on Taikai. Development window: November 2–9, 2026.*
