# Tasks: GitHub Profile README

## Review Workload Forecast

| Field | Value |
|-------|-------|
| Estimated changed lines | 160-230 total |
| Per-task estimates | 1.1: 20-30; 1.2: 25-35; 2.1: 30-45; 2.2: 35-55; 2.3: 20-30; 3.1: 10-15; 3.2: 0-5; 3.3: 10-15 |
| 400-line budget risk | Low |
| Chained PRs recommended | No — one static README, no generated code, no tests |
| Suggested split | Single PR with work-unit commits |
| Delivery strategy | ask-always |
| Chain strategy | pending |

Decision needed before apply: Yes
Chained PRs recommended: No
Chain strategy: pending
400-line budget risk: Low

### Suggested Work Units

| Unit | Goal | Likely PR | Notes |
|------|------|-----------|-------|
| 1 | Create README structure, hero, scan highlights, and contact path | PR 1 | Commit as README foundation; manually check first-screen scan. |
| 2 | Add skills, projects, credentials, research, and footer | PR 1 | Commit content evidence as one reviewable story. |
| 3 | Manual verification and wording polish | PR 1 | Commit final review fixes only if needed. |

## Phase 1: Foundation and First Screen

- [x] 1.1 Create `README.md` with heading hierarchy: hero, highlights, skills, projects, credentials/research, contact, footer.
- [x] 1.2 Add `README.md` hero/intro with Senior Cloud Data Infrastructure Engineer / Platform Architect positioning, AWS SAA, PhD, IoT scale, LinkedIn, and restrained badges.

## Phase 2: Evidence Content

- [x] 2.1 Add `README.md` about/skills section using the real stack: AWS IoT Core, MQTT, Lambda, SQS, DynamoDB, PostgreSQL, Docker, Terraform, Grafana, CloudWatch, TLS/mTLS, MFA.
- [x] 2.2 Add `README.md` projects section with ComatReleco descriptive entry only, research/Google Scholar entry, and future Digital Twin ColdRoom Monitoring dashboard (AWS IoT Core, Lambda, SNS, SQS, ThingsBoard) marked in development with public repos planned.
- [x] 2.3 Add `README.md` certifications, education, awards, publications, contact links, and footer: AWS SAA Credly, PhD, Fakultätspreis 2019, Scholar, LinkedIn.

## Phase 3: Manual Verification

- [x] 3.1 Inspect `README.md` against spec scenarios: first-screen recruiter scan, mobile scan, client deep-dive, verified claims, restrained visuals.
- [x] 3.2 Verify `README.md` links resolve: Credly AWS badge, Google Scholar, LinkedIn; ensure no private ComatReleco repo links are present.
- [x] 3.3 Check GitHub Markdown rendering assumptions, mobile wrapping, image alt/fallback text, English-only content, and total changed lines under 400.
