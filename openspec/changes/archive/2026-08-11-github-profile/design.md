# Design: GitHub Profile README

## Technical Approach

Design a static, English-only `README.md` as a content architecture artifact. The reader journey keeps Cloud/Data Platform Engineering as the primary identity, then introduces Space/GNSS as a visible but secondary "Direction / Emerging specialization" bridge after the core identity and scan highlights. Deep-dive sections expand only approved public facts from the profile skill/brief and keep all private or unsupported claims out.

## Architecture Decisions

| Area | Choice | Alternatives considered | Rationale |
|------|--------|--------------------------|-----------|
| Reader journey | Hero → scan highlights → direction bridge → skills → projects → credentials → contact | Badge-heavy hero, long biography first | Preserves the approved sequence while making Space/GNSS visible within 30 seconds without dominating the opening. |
| Primary identity | Lead with Senior Cloud Data Infrastructure Engineer / Platform Architect | Space-first, IoT-first, DevOps-first, academic-first | Matches the skill hierarchy and prevents competing identities. |
| Space/GNSS placement | Add one concise "Direction / Emerging specialization" element after scan highlights | Put Space/GNSS in hero title or hide it in credentials | Scan-visible but explicitly forward-looking and grounded in transferable systems work. |
| Fact inventory | Place TucanBit in scan/project evidence; AWS Pro prep and JNSP in credentials/current development; PhD, prize, location, languages in credentials/contact | Spread facts randomly across prose | Reviewers can verify facts quickly against the brief. |
| Visual system | Restrained badges only; text-first fallback | Skill-icon walls, stats-first layout | Mobile-safe Markdown remains readable when external assets fail. |

## Data Flow

Reader attention moves from identity to proof without requiring external assets:

    Hero ─→ Scan Highlights ─→ Direction Bridge ─→ Skills ─→ Projects ─→ Credentials ─→ Contact
      │            │                    │             │          │              │            │
      └──────────── text-first fallback when badges/stats fail ────────────────┘

Section inventory and order:
1. Hero: name, Senior Cloud Data Infrastructure Engineer / Platform Architect, secure cloud platforms for distributed/IoT data systems, LinkedIn.
2. Scan highlights: architecture + hands-on AWS/IaC, 7+ years Industrial IoT, TucanBit consulting/portfolio engineering, AWS SAA, PhD depth.
3. Direction / Emerging specialization: one short bridge: distributed systems + telemetry/IoT + cloud infrastructure + networking + signal processing + positioning/coordinate systems → GNSS/satellite data infrastructure.
4. Core skills: AWS, Terraform/Terragrunt, cloud networking, IoT telemetry, data-intensive systems, observability/security; avoid keyword-wall formatting.
5. Projects: TucanBit/current portfolio context where appropriate; real Industrial IoT/cloud platform evidence; distributed systems/wireless analytics research; Digital Twin ColdRoom Monitoring as clearly "in development" growth slot only.
6. Credentials/current development: AWS SAA, preparing AWS Solutions Architect Professional, JNSP training starting September 2026, PhD in Distributed Systems and Wireless Sensor Networks at University of Bern, Faculty of Science dissertation prize.
7. Location/languages/contact: Bern, Switzerland; Spanish native, English fluent, French B1 conversational; LinkedIn `https://www.linkedin.com/in/jlcarvi/` and profile-relevant links.

## File Changes

| File | Action | Description |
|------|--------|-------------|
| `README.md` | Create later | Final GitHub profile README following this information architecture. |
| `openspec/changes/github-profile/design.md` | Modify | Updated content design using real CV-backed project, credential, stack, metrics, and conflict-handling signals. |

## Interfaces / Contracts

README contract:
- Total target: 170-280 lines; hard ceiling under 400 lines.
- Top section must remain understandable as plain Markdown.
- No wide tables for critical content; bullets must wrap cleanly on mobile.
- Every image must have meaningful alt text; decorative badges must not carry exclusive meaning.
- Badge failure fallback: adjacent text/link must preserve the same information.
- Project links must be honest: GitHub URLs only for existing public repositories; otherwise use descriptive entries or “public write-up pending” phrasing.
- Certifications/current development: list AWS SAA; state AWS Professional preparation and JNSP start date as in-progress/upcoming, never completed.
- Space/GNSS wording: use "emerging specialization", "trajectory", "training", or "transferable expertise"; never claim professional satellite, GNSS, or ground-segment experience.
- Public/private boundary: include Bern, languages, public credentials, education, award; exclude Swiss Permit C and detailed geographic market targeting.
- Duration wording: use the brief-backed "7+ years Industrial IoT" source consistently.

Review checklist mapping:
- 10-15s: role/seniority, Cloud/Data Platform identity, architecture, hands-on implementation, AWS+IaC, distributed systems, Industrial IoT.
- 30s: Space/GNSS bridge is understandable as emerging; engineering evidence is findable in skills/projects/credentials.
- Fail if: PhD dominates, profile reads IoT/DevOps/Space-first, unsupported projects/metrics appear, visuals dominate, or generic AI language appears.

## Testing Strategy

| Layer | What to Test | Approach |
|-------|-------------|----------|
| Unit | Heading levels, link text, badge count, line budget, duration wording | Manual Markdown inspection against proposal/spec. |
| Integration | GitHub rendering, mobile wrapping, image alt/fallback readability | Preview rendered README on desktop and phone-width viewport. |
| E2E | 10-15s and 30s review journeys | Verify scan criteria first, then Space/GNSS bridge, evidence placement, public/private boundary, and contact path. |

## Migration / Rollout

No migration required. Rollout is adding `README.md`; rollback is reverting that file.

## Open Questions

- [ ] Which publications should be linked directly versus summarized as selected research output?
- [ ] Are there public GitHub repositories for any project entries, or should v1 use descriptive entries only? (Partially answered: ComatReleco is private; Digital Twin ColdRoom Monitoring dashboard repos are planned but not yet available.)
