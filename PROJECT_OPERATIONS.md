# AIML Club OCT — Contributor Project Operations

This guide defines a lightweight, transparent workflow for proposing, claiming, building, reviewing, and recognizing community projects across the AIMLCLUBOCT repositories.

**Purpose:** help contributors find appropriately scoped work, give every accepted contribution a clear owner, and make progress visible without creating unnecessary bureaucracy.

## 1. Project levels

| Level | Suitable contributor | Typical scope | Expected support |
|---|---|---|---|
| Beginner | New to Git, Python, Markdown, or notebooks | Documentation, small bug fixes, starter examples, simple UI improvements | Clear steps, setup guidance, mentor check-in |
| Intermediate | Comfortable with a language/framework and basic testing | End-to-end feature, model evaluation, API integration, workshop notebook | Defined acceptance criteria, peer review |
| Advanced | Strong engineering or ML foundations | Architecture, deployment, performance, security, multi-module work | Design review, technical owner |
| Research | Familiar with scientific method and evaluation | Reproduction, benchmarking, dataset studies, ablations, paper implementation | Experiment protocol, reproducibility review |

Choose the level based on the actual scope and prerequisites, not prestige. A research task may also be beginner-friendly when it is carefully bounded.

## 2. Project lifecycle

Use the following statuses consistently in the GitHub Project board or issue labels where available:

1. **Proposed** — idea submitted; scope not yet approved.
2. **Ready** — objective, owner expectations, deliverables, and acceptance criteria are clear.
3. **Available** — open for volunteers; no contributor has been assigned.
4. **Assigned** — one accountable contributor has accepted ownership.
5. **In Progress** — implementation has started and progress is being reported.
6. **Review** — pull request is open and awaiting review.
7. **Changes Requested** — reviewer identified issues to address.
8. **Done** — pull request merged and documentation/release notes updated.
9. **Blocked** — progress depends on a decision, access, data, or external dependency.

Do not mark a task Done merely because a pull request was opened.

## 3. How to claim a project

A contributor should comment on the issue with:

- GitHub username and preferred name (optional).
- Relevant skills and a short example of related work, if available.
- A brief implementation plan.
- Estimated time commitment and any blockers.
- Which deliverable they intend to own.

Maintainers should acknowledge the request, check for existing volunteers or overlapping work, confirm the scope, and then assign the contributor. Assignment means ownership, not a guarantee that the work will be merged without review.

For a multi-person task, nominate one issue owner and split deliverables into non-overlapping sub-tasks. Do not have two contributors independently edit the same files without coordination.

## 4. Issue specification checklist

Every implementation issue should include:

- **Problem:** what is missing or broken?
- **Outcome:** what should exist when the task is complete?
- **Audience and use case:** who will use it?
- **Scope:** what is in and out of scope?
- **Prerequisites:** skills, hardware, software, datasets, or access needed.
- **Deliverables:** files, tests, docs, demo, or experiment outputs.
- **Acceptance criteria:** observable checks a reviewer can verify.
- **Validation:** commands, test cases, metrics, or manual steps.
- **Data and security:** licensing, privacy, secrets, and safe handling.
- **Owner and reviewer:** assigned contributor and responsible reviewer.
- **Dependencies:** related issues, PRs, and blockers.

Avoid invented deadlines, performance targets, certificates, or event details. Add them only after the responsible lead confirms them.

## 5. Weekly progress update

For active work, contributors should post a short update on the issue at the agreed cadence:

```text
Progress:
- What I completed:

Next:
- What I plan to do next:

Blockers:
- What is blocked / help needed:

Evidence:
- Branch, draft PR, commit, demo, or test output:
```

A weekly update is a coordination aid, not an attendance requirement. If the task is short, one start and one completion update may be enough.

## 6. Pull request and review expectations

- Work in a focused branch and submit a PR against the correct repository's default branch.
- Link the issue using `Closes #<issue-number>` when the PR fully resolves it.
- Explain the implementation, trade-offs, and verification performed.
- Include screenshots or a short demo for user-facing changes.
- Include tests or reproducible validation for code and ML changes.
- Report model metrics honestly; state dataset split, baseline, random seed, and limitations where relevant.
- Do not commit secrets, private student data, unlicensed datasets, or large model weights.
- Maintainers review for correctness, reproducibility, security, documentation, and scope.
- No automatic merge: approval and repository policy still apply.

## 7. Recognition and contributor profiles

Recognition should be evidence-based:
- Highlight merged contributions and meaningful project outcomes.
- Credit contributors in the relevant README, release notes, or contributor page after the work is merged.
- Distinguish merged work from ongoing work and issue discussion.
- Do not promise certificates, internship outcomes, prizes, or endorsements unless the club has formally approved them.
- Ask before publishing personal information beyond a public GitHub username.

## 8. Mentorship and escalation

- Beginner tasks should have explicit setup steps and a named point of contact or team channel.
- Intermediate and advanced work should receive a scope/design check before large implementation starts.
- Research work should have a written protocol before experiments: hypothesis, dataset provenance, baseline, metrics, and reproducibility notes.
- If a contributor is blocked, they should state the blocker in the issue. Maintainers should clarify scope or split the task rather than silently leaving it stalled.
- If availability changes, the contributor should update the issue so ownership can be reassigned fairly.

## 9. Maintainer triage checklist

Before assigning:
- [ ] Is the issue still relevant and not duplicated by an open PR?
- [ ] Is the level and prerequisite skill set clear?
- [ ] Are deliverables and acceptance criteria testable?
- [ ] Is the data, licensing, and security position understood?
- [ ] Has the contributor volunteered and confirmed availability?
- [ ] Is there one accountable owner and a reviewer/mentor?

Before closing:
- [ ] Acceptance criteria satisfied.
- [ ] PR reviewed and merged, or disposition explained.
- [ ] Docs and examples updated.
- [ ] Contributor credit recorded accurately.
- [ ] Related issue/PR links are correct.

## 10. Current project intake

The following are active contribution opportunities. These links point to the source issues; check their latest status and volunteer discussion before claiming:

| Repository | Project | Level | Issue |
|---|---|---|---|
| Projects | Kaggle SMS Spam Dataset Loader and Evaluation Benchmark | Intermediate | [#11](https://github.com/AIMLCLUBOCT/Projects/issues/11) |
| Projects | Interactive Student Performance Predictor | Beginner | [#1](https://github.com/AIMLCLUBOCT/Projects/issues/1) |
| Workshops | LLM Prompt Engineering and Structured Outputs Notebook | Beginner–Intermediate | [#5](https://github.com/AIMLCLUBOCT/Workshops/issues/5) |
| learning_resources | Python OOP and Dataclasses Guide | Beginner | [#7](https://github.com/AIMLCLUBOCT/learning_resources/issues/7) |
| EVENTS | HackOCT 2026 AI Tracks and Judging Rubric | Intermediate | [#1](https://github.com/AIMLCLUBOCT/EVENTS/issues/1) |

This is a starting list, not a claim that all opportunities are unassigned. Confirm live issue assignments and comments before allocation.

---

**Maintainer principle:** make the next step obvious, keep ownership explicit, review the work fairly, and never trade quality or contributor wellbeing for activity metrics.
