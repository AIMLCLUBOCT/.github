# Contributing to AIML Club OCT

Thank you for your interest in contributing to the **AI & Machine Learning Club – Oriental College of Technology, Bhopal**!

As a student-driven technical community, we welcome contributions from students, members, developers, and open-source contributors. Contributions may include fixing a typo, improving an AI tutorial, adding workshop material, or submitting a reproducible project.

## Code of Conduct

By participating, you agree to follow our [Code of Conduct](./CODE_OF_CONDUCT.md). Treat community members with respect and provide constructive feedback.

## Where to Contribute

1. **Learning resources:** tutorials, roadmaps, concept explanations, and verified documentation links in `learning_resources`.
2. **Projects:** documented AI, ML, deep learning, computer vision, NLP, and generative AI projects in `Projects`.
3. **Workshops:** notebooks, slides, datasets with appropriate permissions, and practical exercises in `Workshops`.
4. **Events:** event summaries, schedules, slides, and verified records in `EVENTS`.
5. **Documentation:** fixes for typos, broken links, setup instructions, and dependency documentation.
6. **Templates:** reusable project, experiment, and documentation templates.

## Contribution Workflow

### 1. Choose the right repository

Read the target repository's README and contribution instructions before making changes. If the change is substantial or introduces a new project, open an issue first to discuss its scope.

### 2. Fork and clone

Fork the target repository to your GitHub account, then clone your fork:

```bash
git clone https://github.com/YOUR-USERNAME/REPOSITORY-NAME.git
cd REPOSITORY-NAME
git remote add upstream https://github.com/AIMLCLUBOCT/REPOSITORY-NAME.git
```

### 3. Create a focused branch

Use a descriptive, lowercase branch name:

```bash
git checkout -b feat/add-linear-algebra-notes
# or: git checkout -b fix/broken-readme-links
```

Keep each pull request focused on one logical change. Do not commit directly to the upstream default branch.

### 4. Make and verify your changes

- Follow the target repository's formatting and contribution conventions.
- For Python, use the repository's configured formatter and lint rules where available.
- For notebooks, remove irrelevant outputs and check that no local paths, credentials, or personal data are exposed.
- Verify relative links, image paths, and setup instructions.
- Run the relevant tests or validation commands documented by the repository.
- Include dependency and environment details when adding executable code.

### 5. Commit and push

Use a clear commit message:

```bash
git add .
git commit -m "docs: add linear algebra study guide"
git push -u origin feat/add-linear-algebra-notes
```

Common prefixes: `feat:`, `fix:`, `docs:`, `test:`, `refactor:`, and `chore:`.

### 6. Open a pull request

Open a pull request from your fork and branch into the matching `AIMLCLUBOCT` repository. Complete the [Pull Request Template](./.github/PULL_REQUEST_TEMPLATE.md) and explain the motivation, scope, and verification performed.

A maintainer review is required before integration. Respond to review feedback with focused commits; do not force-push over shared work without coordinating with reviewers.

## Quality and Security Standards

- Do not submit plagiarized or proprietary material. Attribute external sources and respect their licenses.
- Prefer official documentation and primary sources.
- Do not invent benchmark results, project status, affiliations, or performance claims.
- Make code reproducible with clear setup steps, supported versions, and dependency files.
- Never commit API keys, passwords, access tokens, private datasets, student identifiers, or personal contact information without explicit authorization.
- Do not upload datasets or media unless you have the right to share them.

## Need Help?

- Read the [Support Guide](./SUPPORT.md).
- For questions, contact [aimlcluboct@gmail.com](mailto:aimlcluboct@gmail.com).
- Share suggestions through [voice.aimlcluboct.in](https://voice.aimlcluboct.in).
