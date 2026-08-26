# ZeroSight360 LinkedIn V2 — Topic-Native Visual Plan

## Objective
Replace the repeated dark navy/teal/coral stat-card treatment with visual formats chosen for the subject matter. The new set uses the topic as the art direction instead of forcing every post into one brand template.

## Output contract
- 30 primary images, one per post in `posts/posts_30day.json`
- Canvas: 1080x1080 PNG
- Working source: one HTML file per image
- Naming: `v2_day01_<slug>.png` and matching `.html`
- Existing repository assets remain untouched until the new set is reviewed
- Small attribution only: `zerosight360.com` and channel marker where useful

## Visual principles
1. One dominant idea per image; supporting copy stays short.
2. Topic evidence is the visual hook: code, timeline, chart, map, receipt, or redaction.
3. Personal posts feel like field notes, not company advertisements.
4. Company posts feel like briefings, not generic motivational graphics.
5. Color is semantic and topic-led: orange/red for active danger, acid green for system state, paper/black for evidence, cobalt for technical analysis.
6. No emoji-dependent meaning, no oversized logo, and no decorative empty space that competes with the message.

## Reusable topic-native archetypes

### A — Forensic evidence / terminal
Black or warm-gray evidence sheet, case ID, line numbers, redaction bars, code or configuration as the hero.

### B — Threat bulletin / countdown
Newsroom or incident-command layout with timestamp, countdown, severity stamp, and one decisive number.

### C — Data laboratory / comparison
Paper or dark-graph layout with a large chart, ranked bars, benchmark labels, or before/after evidence.

### D — Split-screen argument
Two opposing states with a clear hinge: developer/security, traditional/AI phishing, marketing/reality, annual/continuous.

### E — Control room / system map
Process diagrams, maturity ladders, checklists, and connected controls. Visual logic matters more than decoration.

### F — Field note / human story
Editorial notebook, interview card, receipt, or incident log. Designed for credibility and narrative tension.

### G — Forecast / strategic brief
Blackboard or analyst memo style with numbered predictions, horizon markers, and uncertainty language.

## 30-post visual map

| Day | Topic | Channel | Archetype | Visual hook / treatment |
|---:|---|---|---|---|
| 01 | AI Code Review | Personal | A — Forensic evidence | Redacted code review with vulnerable lines highlighted and an AI-generated diff marker |
| 02 | Exploit Window | Company | B — Threat bulletin | Negative countdown: `-7 DAYS`, disclosure and exploitation timestamps crossing over each other |
| 03 | Dev vs Security | Personal | D — Split-screen argument | Two sticky-note columns: what developers hear vs what security means; center bridge labeled `TIMING` |
| 04 | API Security | Company | C — Data laboratory | API request/auth flow with a broken lock at the verification step and the `52%` finding as annotation |
| 05 | Startup Cost | Personal | F — Field note | Runway receipt: `18 MONTHS → 3 MONTHS`, with breach costs shown as line items |
| 06 | Secure SDLC | Company | E — Control room | Pipeline diagram from threat model to runtime, showing controls at each gate |
| 07 | Found Database | Personal | A — Forensic evidence | Public-bucket evidence card with an exposure timer: `20 MINUTES FOUND / 3 YEARS OPEN` |
| 08 | Cloud Misconfig | Company | B — Threat bulletin | Cloud control-room alert: one checkbox flips `PRIVATE` to `PUBLIC`, with 23% as incident statistic |
| 09 | IAM Policy | Personal | A — Forensic evidence | IAM case file with line-numbered wildcard policy, critical stamp, and blast-radius finding |
| 10 | Container Security | Company | E — Control room | Layered container stack: base image, OS, dependencies, runtime; CVEs glow at the hidden layers |
| 11 | Private VPC Myth | Personal | D — Split-screen argument | `PRIVATE VPC` crossed against four real exposure paths: S3, NAT, security group, IAM |
| 12 | Cloud Maturity | Company | E — Control room | Five-stage operations ladder from reactive to optimized, with enforcement—not documentation—as the gap |
| 13 | AI Reality Check | Personal | D — Split-screen argument | `NEW TOOL` versus `OLD FAILURE`: same vulnerabilities, phishing, and alert overload amplified |
| 14 | Shadow AI | Company | F — Field note | Data-leak trail from employee prompt to public model, with a red cost receipt for `$670K` |
| 15 | AI Code Test | Personal | C — Data laboratory | Ranked benchmark board for five assistants; vulnerable-code rate becomes the visual hierarchy |
| 16 | Prompt Injection | Company | B — Threat bulletin | Prompt shown as a malicious payload entering a trusted AI pipeline; `90+ ORGS` as incident marker |
| 17 | AI Phishing | Personal | D — Split-screen argument | Traditional vs AI-crafted email side by side, with `12%` and `54%` click-rate gauges |
| 18 | AI Pipeline Security | Company | E — Control room | Six-gate AI deployment checklist with model supply chain, data, prompts, output, monitoring, rollback |
| 19 | Security Theater | Personal | F — Field note | Compliance checklist stamped `ACTIVITY`, contrasted with a blank `OUTCOME` incident metric |
| 20 | Credential Theft | Company | B — Threat bulletin | Credential factory / evidence wall: passwords, cookies, tokens, certificates feeding one identity perimeter |
| 21 | Intern Story | Personal | F — Field note | Annotated code notebook with `3 SENIORS MISSED / 1 FRESH EYES FOUND` and the race-condition path |
| 22 | Incident Response | Company | B — Threat bulletin | 29-minute command clock with containment checkpoints; meeting calendar crossed out |
| 23 | Stop Annual Pentests | Personal | D — Split-screen argument | `2020: 63 DAYS` versus `2026: -7 DAYS`, ending in continuous testing rather than “never pentest” |
| 24 | MFA Not Enough | Company | E — Control room | MFA defense layers with session-token theft, fatigue, phishing proxy, and SIM swap as bypass routes |
| 25 | Axios Attack | Personal | A — Forensic evidence | npm incident timeline as an evidence log: compromise → publish → spread → discovery |
| 26 | 2027 Predictions | Company | G — Forecast / strategic brief | Analyst forecast board with seven numbered signals and an explicit `PREPARE, DON'T PREDICT` footer |
| 27 | 100 Assessments | Personal | F — Field note | Research notebook with five repeated findings, marked `80% OF CODEBASES`, not a generic list card |
| 28 | Supply Chain Stats | Company | C — Data laboratory | Year-over-year package explosion chart, with incident callouts pinned to the graph |
| 29 | 241-Day Breach | Personal | B — Threat bulletin | Slow-burn breach calendar: 241 days of invisible access before the public explosion |
| 30 | Zero Trust Reality | Company | D — Split-screen argument | Product marketing promise crossed against architecture reality: identity, least privilege, segmentation, validation |

## Publishing safety gates
Before activating the new set in automation:
- Verify every numerical claim and attribution against a source.
- Mark personal stories as real, anonymized, or illustrative.
- Resolve conflicting statistics across the old sets (for example API, cloud, AI-code, and supply-chain figures).
- Confirm whether the new set should be added under `v2/` or replace the root image references.
- Keep the existing automation unchanged until the new images and metadata are approved.
