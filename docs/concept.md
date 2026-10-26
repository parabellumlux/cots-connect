# COTS Connect — Entry Concept for OutSystems "Build for the Future 2026"
Scoped 2026-10-20 · Status: CONCEPT — not registered; DC's go/no-go pending (registration closes Oct 28)

## The one-liner
An agentic outreach and care-coordination app for Church on the Street of Texas (COTS), a real Odessa street-ministry nonprofit: people in need text in, an AI agent triages and opens a care case, volunteers get coordinated by text, and nothing falls through the cracks.

## The nonprofit (this is the entry's unfair advantage)
- COTS is real: Texas nonprofit corporation, Certificate of Formation filed 07/26/2026 (#806716580). DC is president/organizer; directors Diana Walker and Henry Pettigrew.
- Mission direction (from the founding materials): street ministry in the Odessa/Permian Basin — food-donation partnerships, outreach to people living on the street, property/funding for a ministry base.
- Honest caveat: COTS is early-stage. EIN and the IRS exemption (Form 1023) are still in flight. That doesn't block entering or naming COTS as the beneficiary nonprofit, but prize disbursement terms are worth one question to the organizers (see Open Questions).

## The problem
A street ministry runs on texts, memory, and paper:
- Someone in need reaches out by phone or word of mouth; whoever answers writes it down — or doesn't. Follow-ups (a promised food box, a ride, a check-in next week) get lost.
- Food-donation partners (stores, restaurants) offer pickups on short notice; coordinating who collects, when, and where it goes is a scramble.
- Volunteers are few and willing, but scheduling outreach runs and reminding people is manual.
- When a grant or a donor asks "how many people did you serve, and what happened next?" there are no numbers — just stories.
For a three-person board, every dropped follow-up is a person who asked for help and heard silence.

## The app (built in OutSystems ODC, per the rules)
Four modules, deliberately scoped to what a first-time ODC team can ship in 7 days:

1. **Text-a-Need intake (Twilio + agent).** A person texts the ministry number ("I need food for my kids tonight"). The AI agent converses in plain language, identifies the need (food / clothing / shelter referral / prayer / ride), urgency, location, and household size, then opens a structured care case in ODC. No app, no form, no literacy barrier beyond texting.
2. **Follow-up copilot (agent, human-in-the-loop).** The agent watches open cases and drafts the next step: a check-in text, a referral note to a partner agency, a reminder to the assigned volunteer. A human approves every outbound message before it sends — the agent drafts, people decide. This is the "agentic" heart of the entry and fits the judging emphasis on Agentic AI.
3. **Volunteer & food-run coordinator.** Volunteers register once; the coordinator builds outreach runs and donation pickups, assigns them, and sends Twilio reminders with the details. Completion gets logged from a reply text ("DONE") — no volunteer app to install.
4. **Impact dashboard.** Counts the ministry can actually use: people served, needs by type, follow-ups closed, response time from first text to first help. This is the grants-and-donors view, and the demo's closing shot.

## How it maps to the prizes
- **Core requirement:** built on ODC using the Agentic AI features presented at the Nov 2 kickoff (a stated selection criterion) — Modules 1–2 are built on ODC's agent tooling.
- **Twilio special prize:** Twilio is the front door (SMS intake) and the nervous system (reminders, completion logging) — integrated by design, not bolted on. Rules say teams are expected to use Twilio to be eligible for the special Twilio prize.
- **AWS / Microsoft categories:** pick ONE at kickoff, whichever ODC integrates most cleanly with the supplied tokens (e.g., Bedrock or Azure OpenAI behind the intake agent's language understanding). Chasing both dilutes the build.
- **Open source:** the rules expect submissions to be open-source so other communities benefit — for COTS Connect that's a feature of the pitch: any small church or street ministry can clone it. "Built for one ministry in Odessa, reusable by thousands."

## Judging-fit notes
- Real nonprofit, real president, real community — not a hypothetical beneficiary invented for the contest.
- Human-in-the-loop agentic design is a defensible, demonstrable story: the demo video can show a text arriving, the agent drafting, a human approving, and help moving.
- Measurable impact is built in (Module 4) — the Impact dashboard answers the "so what" question judges ask.

## The week (Nov 2–9) against DC's real calendar
Known collisions: HHSC hearing + Midland plan payment Tue Nov 3, eye appointment Thu Nov 5 (10:15 AM, Midland), YouCam submission lands Nov 1–2.
- **Mon Nov 2:** Kickoff (mandatory, ≥1 team member) + ODC environment, data model, case/intake screens.
- **Tue Nov 3:** Light day (hearing morning). Agent prompts + intake conversation design — work that can pause.
- **Wed Nov 4:** Twilio SMS flow end-to-end. **Mid-submission due** (problem statement, use case, planned integrations/AI) — Baymax pre-drafts this before Nov 2 so it's a review-and-send, not a writing day.
- **Thu Nov 5:** Light morning (eye appt). Volunteer & food-run module.
- **Fri Nov 6:** Follow-up copilot (drafting + approval queue).
- **Sat Nov 7:** Impact dashboard + end-to-end polish.
- **Sun Nov 8:** Buffer, testing with real phones, fix list.
- **Mon Nov 9:** Demo video (≤5 min) + project description doc; **submit by 4:59 PM CT.**

## Pre-work (Oct 26–28, before the build week)
1. Register on Taikai — every team member individually, by Oct 28 (team confirmation step lands Oct 26). Team: DC + Diana proposed (mirrors the YouCam team; Diana is a COTS director, which strengthens the story).
2. ODC learning sprint: OutSystems' free getting-started material; get the development environment open and a hello-world deployed BEFORE Nov 2 so the kickoff isn't the first contact.
3. Accessibility note, stated plainly: ODC's designer is a visual drag-and-drop canvas — real friction with progressive vision loss. Mitigations: pair-building with Diana on the canvas while DC directs architecture/prompts/testing, large-display setup on luci, and Baymax writing the step-by-step for every build action. If the canvas proves unusable in the sprint, that's the honest kill signal — better known Oct 28 than Nov 4.
4. Baymax pre-drafts: mid-submission document, project description skeleton, demo-video script outline.

## Feasibility verdict
**Buildable, with discipline.** The scope above is CRUD + one SMS integration + agent drafting — the right size for ODC's strengths. The two real risks are (1) the first-time ODC learning curve landing in the most collision-heavy week on DC's calendar, and (2) the visual-canvas accessibility question, which the Oct 26–28 sprint exists to answer cheaply. Cut list if the week goes sideways, in order: Module 4 shrinks to a simple counts page; Module 3's pickup scheduling drops (keep volunteer runs). Modules 1–2 are the entry — protect them.

## What winning would mean
1st place: $10,000 to COTS + a 12-month ODC license for the team (2nd $5,000, 3rd $2,500 — all prize cash goes to the selected nonprofit). Even a non-winning finish leaves COTS with a working intake/follow-up system and an open-source template other ministries can adopt.

## Open questions for the organizers (ask at registration/kickoff)
1. Beneficiary nonprofits: any formation/exemption status required for prize disbursement? (COTS: TX corporation formed 07/2026; EIN/1023 in flight.)
2. Are design documents and pitch materials prepared before Nov 2 allowed? (Standard hackathon rule is build-in-window; the mid-submission is a document, so drafting support text early should be fine — confirm.)
3. ODC license seat count for a 2-person team during the event.

## Next step
DC's call: register (DC + Diana) by Oct 26–28, or pass. If go: Baymax handles the Taikai registration flow with DC present for any account verification, starts the ODC sprint checklist, and pre-drafts the Nov 4 mid-submission.
