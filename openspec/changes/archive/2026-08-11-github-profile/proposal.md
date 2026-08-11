# Proposal: GitHub Profile README

## Intent

Create an honest, professional GitHub profile `README.md` for recruiters, engineering leaders, architects, and clients. The `.opencode/skills/build-senior-tech-profile/` skill and `references/profile-brief.md` are the authoritative source for professional claims, superseding the earlier CV-only raw-material framing.

## Scope

### In Scope
- English-only static README with dual-mode structure: 10–15 second scan plus deeper review.
- Primary identity: Senior Cloud Data Infrastructure Engineer / Platform Architect with architecture depth, hands-on AWS/IaC execution, distributed systems, and Industrial IoT.
- Space/GNSS emerging specialization as a credible bridge from distributed systems, telemetry, cloud infrastructure, networking, signal processing, positioning, and coordinate systems.
- Public README facts: 7+ years Industrial IoT, TucanBit consulting/portfolio activity, AWS SAA, AWS Solutions Architect Professional preparation, Joint Navigation Satellite Programme training starting Sept 2026, PhD in Distributed Systems and Wireless Sensor Networks at University of Bern, Faculty of Science dissertation prize, Bern Switzerland, Spanish native, English fluent, French B1 conversational.
- Restrained visuals, honesty guardrails, growth-ready projects, and Digital Twin ColdRoom as a future project.

### Out of Scope
- Dynamic README generation, GitHub Actions, tokens, scheduled updates, or workflow automation.
- Multilingual content.
- Private facts: Swiss Permit C, detailed geographic market targeting, or any claim of professional satellite/ground-segment experience.
- Fake projects, fake metrics, exaggerated claims, full portfolio site, CV rewrite, or detailed case studies.

## Capabilities

### New Capabilities
- `github-profile-readme`: Professional static GitHub profile README content, structure, visual restraint, honesty rules, growth placeholders, and manual rendering verification.

### Modified Capabilities
- None.

## Approach

Use the project skill workflow: read the brief/checklist, inspect README, plan before editing, then review against the checklist. The README should lead with one coherent story, show evidence-backed capabilities, keep the PhD supportive rather than dominant, and present Space/GNSS as forward-looking transferability only.

## Affected Areas

| Area | Impact | Description |
|------|--------|-------------|
| `README.md` | New | Future profile README deliverable. |
| `openspec/changes/github-profile/` | Modified | Proposal artifact for this change. |
| `.opencode/skills/build-senior-tech-profile/` | Source | Authoritative profile-claim skill and review checklist. |

## Risks

| Risk | Likelihood | Mitigation |
|------|------------|------------|
| README drifts from the skill/brief | Med | Treat skill as source of truth; spec mirrors it; review against checklist. |
| Space/GNSS credibility overclaims experience | Med | State emerging specialization/training only; never claim professional satellite or ground-segment experience. |
| Visual elements reduce scanability | Med | Use few badges/cards and keep sections short. |
| External badge/stat services fail | Low | Treat them as decorative; core content remains readable. |
| Scope exceeds 400-line review budget | Low | Keep README static, concise, and section-based. |

## Rollback Plan

Revert the future `README.md` addition or restore the previous README state. No data migration, runtime, or automation rollback is required.

## Dependencies

- User-provided LinkedIn URL: `linkedin.com/in/jlcarvi`.
- `.opencode/skills/build-senior-tech-profile/SKILL.md`, `references/profile-brief.md`, and `references/review-checklist.md`.
- User-approved public/private split and honesty constraints.

## Success Criteria

- [ ] README supports scan-mode and deep-dive audiences.
- [ ] Public facts match the profile brief and approved public/private split.
- [ ] Space/GNSS trajectory is credible without overclaiming experience.
- [ ] No invented projects, metrics, or unverifiable claims are present.
- [ ] Projects section is ready to grow from real project history.
- [ ] Markdown renders cleanly on GitHub with working links and restrained visuals.
