# AIML Club OCT — Open Source Contributor Program

**Program vision:** turn the club's GitHub organization into a reliable, student-led engineering environment where contributors can learn, ship useful work, receive mentorship, and build a verifiable public portfolio.

This is a scalable operating blueprint. Maintainers should adopt it in stages rather than introduce every process at once.

## 1. Operating principles

1. **Real work over vanity metrics:** prioritize useful, maintainable outcomes over issue counts, stars, or activity streaks.
2. **One accountable owner:** every active project has one primary owner; collaborators receive distinct deliverables.
3. **Public and auditable:** decisions, scope changes, blockers, reviews, and completion evidence live in GitHub.
4. **Beginner-safe:** starter tasks include setup instructions, expected outcomes, and a named help contact.
5. **Research integrity:** datasets, licenses, baselines, seeds, metrics, and limitations are documented.
6. **Human-reviewed:** no automatic assignment, approval, or merge based only on activity or bot output.
7. **Privacy by design:** publish GitHub usernames and contribution evidence; do not expose student IDs, phone numbers, personal emails, or private performance data.
8. **Portable and open:** use GitHub-native Markdown, YAML, Issues, PRs, and Projects so the program can migrate later.

## 2. Program roles

| Role | Responsibilities | Authority |
|---|---|---|
| Program Lead | Owns program health, quarterly priorities, and escalation | Approves program-level changes |
| Repository Maintainer | Triages issues, scopes work, assigns owners, reviews PRs | Manages repository workflow |
| Project Mentor | Helps with design, setup, technical blockers, and learning | Advises; does not bypass review |
| Project Owner | Coordinates a scoped project and reports progress | Owns delivery and issue updates |
| Contributor | Implements an agreed deliverable and documents evidence | Opens PRs and requests review |
| Reviewer | Checks correctness, security, maintainability, and acceptance criteria | Approves or requests changes |

One person may hold more than one role in a small team, but the reviewer should not approve their own changes.

## 3. Contributor journey

`Discover → Explore → Volunteer → Scope Check → Assignment → Build → Review → Merge → Showcase → Alumni/Advanced Work`

### Discover
Contributors browse the [open organization issues](https://github.com/issues?q=is%3Aissue+is%3Aopen+org%3AAIMLCLUBOCT) and [project catalog](./PROJECT_CATALOG.md).

### Volunteer
Comment on the issue with:
- GitHub username;
- skills and relevant experience;
- proposed implementation plan;
- expected availability and blockers;
- the specific deliverable they want to own.

### Scope check and assignment
A maintainer verifies that the issue is current, non-duplicative, sufficiently specified, and not already owned. Confirm capacity and assign only after the contributor agrees. For a multi-person task, define non-overlapping work packages and one primary owner.

### Build and review
Use a focused branch and PR. Link the issue, provide tests or reproducible validation, and disclose limitations. Reviewers use the repository's PR template and acceptance criteria.

### Showcase
After merge, record the contribution in the project's release notes or contributor showcase. Clearly distinguish merged work, ongoing work, and participation. Ask before publishing personal information beyond a public GitHub username.

## 4. Project levels and pathways

| Level | Entry expectations | Typical work | Advancement evidence |
|---|---|---|---|
| Beginner | Basic Git and programming or technical writing | Docs, starter notebooks, small UI fixes, tests | A reviewed, merged contribution with reproducible instructions |
| Intermediate | Can work independently in a familiar stack | Features, data pipelines, model evaluation, integrations | Tested feature, clear PR, and response to review |
| Advanced | Strong engineering fundamentals | Architecture, deployment, performance, security | Design rationale, tests, operational documentation |
| Research | Scientific method and evaluation literacy | Reproduction, benchmarking, ablations, dataset studies | Reproducible protocol, baseline, metrics, limitations |

Levels describe task complexity, not a person's worth or permanent rank. Contributors may move between tracks.

## 5. Project lifecycle and status definitions

Use one status field on the organization project board, if available:

- **Proposed:** idea submitted; not yet triaged.
- **Ready:** scope, owner expectations, deliverables, and acceptance criteria are clear.
- **Available:** open for volunteers; not assigned.
- **Assigned:** a contributor has accepted ownership.
- **In Progress:** implementation is underway.
- **Review:** pull request is awaiting review.
- **Changes Requested:** reviewer feedback must be addressed.
- **Blocked:** a dependency, decision, access request, or technical issue prevents progress.
- **Done:** acceptance criteria met and the relevant PR merged.
- **Archived:** no longer active; reason recorded.

Do not infer status solely from an issue's assignee or PR existence. A maintainer should keep the status field current.

## 6. Standard project record

Every substantial project should have:
- objective and user/problem statement;
- project level and required skills;
- owner, mentor, and reviewer (where applicable);
- scope and explicit non-goals;
- deliverables and testable acceptance criteria;
- dependencies, dataset/license/security notes;
- target milestone only when a real date is approved;
- linked issues, PRs, docs, and demo;
- current status and last meaningful update.

Use the [project intake issue form](./.github/ISSUE_TEMPLATE/project-intake.yml) for proposals.

## 7. Progress cadence

For work expected to take more than one week, contributors should post a short weekly update in the issue. For smaller tasks, a start and completion update is enough.

```text
Progress:
- Completed:

Next:
- Planned work:

Blockers:
- Help or decision needed:

Evidence:
- Branch / PR / commit / demo / test output:
```

This is a coordination mechanism, not a surveillance or attendance score. Do not require daily activity or punish contributors for communicating a pause.

## 8. Mentorship model

- Each active beginner project should identify a mentor or support channel before assignment.
- Mentors clarify scope, explain concepts, and help contributors learn; they do not write the entire contribution for them.
- Intermediate/advanced tasks should receive a brief design check before broad implementation.
- Research tasks should agree on hypothesis, dataset provenance, baseline, split strategy, metrics, random seed, and reproducibility before experiments.
- If a mentor is unavailable, mark the task Blocked or find a replacement; do not leave a contributor guessing.

## 9. Contributor recognition and portfolio

Recognition must be verifiable:
- showcase merged PRs and meaningful deliverables;
- link to the actual repository, PR, release, or demo;
- credit collaborators according to their actual work;
- distinguish author, reviewer, mentor, and organizer roles;
- never promise certificates, internships, jobs, prizes, or endorsements unless formally approved by the club;
- avoid leaderboards based only on commit counts or contribution volume.

A future contributor directory may use a public GitHub username, selected public contributions, interests, and optional self-submitted links. It must not become a public student database.

## 10. Quality, security, and research integrity

- Never commit credentials, access tokens, private student records, or personal contact data.
- Confirm dataset and media licenses before redistribution.
- Use synthetic or properly consented data for demos involving student performance or identity.
- Document model limitations; do not present educational predictions as high-stakes decisions.
- Include tests, environment versions, setup instructions, and reproducibility details.
- Use least-privilege workflow permissions and pin third-party GitHub Actions to reviewed versions or immutable SHAs where feasible.
- Do not execute untrusted pull-request code in privileged `pull_request_target` workflows.
- Require human review before merge; do not enable automatic merge as a substitute for review.

## 11. GitHub operating model

Recommended organization-level project fields:

| Field | Type | Example values |
|---|---|---|
| Status | Single select | Proposed, Ready, Available, Assigned, In Progress, Review, Blocked, Done, Archived |
| Level | Single select | Beginner, Intermediate, Advanced, Research |
| Repository | Text or repository field | Projects |
| Project Owner | User | GitHub username |
| Mentor | User | GitHub username |
| Priority | Single select | P0, P1, P2, P3 |
| Target Date | Date | Only approved dates |
| Last Update | Date | Last substantive progress update |
| Program Cycle | Single select | 2026-Q4, 2027-Q1, etc. |

Recommended views:
- **Intake:** Proposed and Ready.
- **Available to contributors:** Available, grouped by Level.
- **Delivery board:** Assigned, In Progress, Blocked.
- **Review queue:** Review and Changes Requested.
- **Showcase:** Done, grouped by repository or program cycle.

The existing roadmap board should be inspected and reconciled before creating a duplicate. Do not create a second board if the current one can support these fields and views.

## 12. Automation roadmap

Introduce automation only after the human workflow is stable:

**Phase A — safe defaults**
- Issue templates collect complete project proposals and progress updates.
- Labels identify level, type, and good-first-issue suitability.
- Existing welcome automation points to contribution docs.

**Phase B — low-risk workflow automation**
- Validate issue and PR templates.
- Add stale-item reminders only after a maintainer-defined inactivity window and a warning period.
- Add PR checks for formatting, tests, secret scanning, and dependency review appropriate to each repository.
- Auto-link issues to PRs using GitHub's native closing keywords.

**Phase C — program analytics**
- Produce a monthly summary of open/blocked/review/done work, median review time, and merged outcomes.
- Report team-level trends, not individual productivity rankings.
- Exclude private data and avoid measuring contribution quality by volume.

Every automation must have a named maintainer, documented permissions, failure behavior, and a manual override. No bot should auto-assign volunteers, approve PRs, or merge code.

## 13. Program metrics

Track a small set of outcome-oriented indicators:
- time from volunteer comment to maintainer response;
- time from PR open to first human review;
- percentage of active tasks with clear acceptance criteria;
- number of projects completed with docs/tests/demo;
- blocked work and reasons;
- contributor retention and self-reported learning (optional, opt-in);
- security or quality regressions discovered after merge.

Use these to improve the system, not rank students. Establish baselines before setting targets.

## 14. Rollout plan

### Phase 1 — Foundation (first 2 weeks)
- Review and approve this operating model.
- Confirm program lead, maintainers, and mentor contacts.
- Reconcile the existing project board and labels.
- Adopt project intake and progress forms.
- Triage the current five-project intake list.

### Phase 2 — Pilot (weeks 3–6)
- Pilot with 3–5 projects across at least two levels.
- Confirm owner/mentor/reviewer for each project.
- Run one weekly async progress cycle.
- Review bottlenecks and contributor feedback.

### Phase 3 — Scale (weeks 7–12)
- Add suitable CI/security checks per repository.
- Publish the first evidence-based showcase.
- Add monthly program health reporting.
- Review whether a public contributor directory is useful and privacy-safe.

### Phase 4 — Continuous improvement
- Review the process each academic term.
- Archive inactive projects transparently.
- Refresh mentors, project levels, and templates.
- Export project records periodically so the process remains portable.

---

**Governance note:** this document is a proposed program standard until approved by the club's authorized maintainers. Repository-specific rules and institutional policies take precedence.
