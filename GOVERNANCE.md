# Repository Governance

This document defines the minimum operating standards for repositories maintained by the AIML Club OCT GitHub organization.

## 1. Roles and responsibilities

- **Organization owners:** Manage organization membership, app installations, security policy, repository visibility, and organization-wide settings.
- **Repository maintainers:** Triage issues, review pull requests, maintain labels and project health, and coordinate releases.
- **Contributors:** Propose changes through issues and pull requests, follow repository instructions, and respond constructively to review feedback.
- **Faculty coordinators and club leadership:** Provide institutional oversight and resolve escalated operational or conduct concerns.

A role listed in a document does not itself grant GitHub permissions. Access must be granted through GitHub's organization and repository settings.

## 2. Branch and pull request policy

1. Do not push directly to `main` for routine development.
2. Use short-lived branches with descriptive prefixes such as `feat/`, `fix/`, `docs/`, or `chore/`.
3. Submit changes through pull requests targeting the repository's default branch.
4. Keep pull requests focused. Separate unrelated documentation, feature, and maintenance changes.
5. Link the relevant issue where one exists and explain the user-visible impact.
6. Do not merge a pull request solely because it is green; review correctness, scope, security, maintainability, and documentation.
7. Resolve requested changes and rerun relevant checks before merging.

## 3. Review standard

Reviewers should check, as applicable:

- **Correctness:** Does the change solve the stated problem? Are edge cases and failure paths handled?
- **Tests:** Are meaningful tests included? Do existing tests and CI checks pass?
- **Security and privacy:** Are credentials, personal data, student identifiers, and private information excluded? Are permissions and untrusted inputs handled safely?
- **Reproducibility:** Are setup steps, dependencies, data sources, and execution instructions clear?
- **Documentation:** Are README files, examples, and usage instructions consistent with the implementation?
- **Scope:** Is the change focused, non-duplicative, and compatible with existing project structure?

Use review outcomes consistently:
- **Approve** only when the change is ready to merge and required checks are satisfactory.
- **Request changes** when a blocking correctness, security, or maintainability issue remains.
- **Comment** for non-blocking feedback, questions, or suggestions.

Authors should not treat an approval as a substitute for required CI checks or repository branch protection.

## 4. Issue triage

Maintainers should:

- Confirm that the report is reproducible and has enough context.
- Search for duplicates before creating a new tracking issue.
- Apply labels that reflect type, priority, and contributor suitability when those labels exist.
- Ask for clarification respectfully and close stale or out-of-scope issues with an explanation.
- Avoid assigning work to contributors without their consent or an established team process.

Suggested priority meanings:

| Priority | Meaning |
| --- | --- |
| P0 — Critical | Active security exposure, data loss, or organization-wide outage |
| P1 — High | Major functionality broken with no reasonable workaround |
| P2 — Normal | Important defect or planned improvement |
| P3 — Low | Cosmetic, minor, or optional enhancement |

These are suggested meanings; repositories may use their own label taxonomy.

## 5. Security and privacy

- Never commit access tokens, API keys, passwords, private keys, or session cookies.
- Do not publish student records, enrollment numbers, personal phone numbers, private email addresses, or other personal data without an appropriate basis and consent.
- Use repository secrets or approved secret-management systems for CI credentials.
- Treat pull request content, uploaded files, notebooks, and external links as untrusted input.
- Report suspected vulnerabilities privately using the process in [SECURITY.md](./SECURITY.md); do not publish exploit details in a public issue.
- Grant the minimum permissions required and review access when responsibilities change.

## 6. Automation standards

- Prefer least-privilege workflow permissions. Set explicit `permissions:` at workflow or job level.
- Pin third-party actions to reviewed versions; use full commit SHAs for security-sensitive production workflows where practical.
- Do not execute untrusted pull request code in privileged contexts such as `pull_request_target`.
- Keep automation transparent: document what it changes, when it runs, and how maintainers can recover from failures.
- Avoid workflows that automatically merge contributions or send external invitations without an explicit maintainer decision.
- Test workflow changes on a branch before relying on them for organization-wide operations.

## 7. Releases and project handover

For projects that publish releases, maintainers should document the supported version, installation steps, known limitations, and change summary. Before handing over a repository, confirm that at least two responsible maintainers understand its build, deployment, issue triage, and recovery process where feasible.

## 8. Exceptions and updates

Repository-specific instructions may add stricter requirements. If they conflict with this document, follow the stricter security or quality requirement and ask maintainers to clarify the discrepancy. Changes to this governance policy should be made through a pull request and reviewed by an organization maintainer.

---

**Maintained by:** AIML Club OCT repository maintainers  
**Scope:** Public repositories in the AIMLCLUBOCT organization, unless a repository provides more specific guidance.
