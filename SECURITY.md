# Security & Privacy Policy

The **AI & Machine Learning Club – Oriental College of Technology (OCT), Bhopal** takes digital security and student data privacy seriously. This document outlines our security standards and responsible vulnerability disclosure process.

---

## 🔒 Security Standards for Contributors

When contributing code, notebooks, or documentation across any AIML Club OCT repository, you must adhere to the following privacy and security requirements:

### 1. No Hardcoded Secrets or Credentials
Never commit sensitive credentials into any repository, branch, or issue. This includes:
- OpenAI, Hugging Face, Google Gemini, Anthropic, or other AI provider API keys.
- AWS, Azure, GCP, or Firebase service account keys and tokens.
- Database passwords, connection strings, or JWT secrets.
- Personal access tokens (PATs) or SSH keys.

> **Best Practice:** Use environment variables (e.g., via a `.env` file and `python-dotenv`) and ensure `.env` is listed in your `.gitignore`. Provide a `.env.example` file containing dummy variable names only.

### 2. Privacy & Personal Data
Never publish personal or confidential student records:
- Phone numbers, personal email addresses, home addresses, or student roll/enrollment numbers.
- Private attendance sheets, evaluation sheets, or grade rosters.
- Private event feedback with identifiable student details without prior consent.

---

## 🚨 Reporting a Vulnerability or Security Issue

If you discover a security vulnerability, exposed credential, or sensitive data leak in any repository under the [AIMLCLUBOCT](https://github.com/AIMLCLUBOCT) organization, **please do not open a public issue**.

Instead, follow this responsible disclosure procedure:

1. **Email us directly:** Send an email to [aimlcluboct@gmail.com](mailto:aimlcluboct@gmail.com) with the subject line:  
   `[SECURITY VULNERABILITY] <Repository Name> - <Brief Description>`.
2. **Include Key Details:**
   - The repository name and file path(s) involved.
   - A description of the vulnerability or exposed asset.
   - Steps to reproduce the issue.
   - Suggested mitigation or fix (if known).
3. **Response Time:** The AIML Club technical team will acknowledge receipt of your report within 48 hours and work with maintainers to patch the vulnerability, rotate exposed credentials, or purge git history.

---

## 🛠️ Accidental Secret Leaks

If you accidentally commit a secret or credential:
1. Immediately **revoke and rotate** the exposed token/key at the provider dashboard.
2. Notify the repository maintainers or email [aimlcluboct@gmail.com](mailto:aimlcluboct@gmail.com) so git history can be purged using tools like `git filter-repo` or BFG Repo-Cleaner.
3. Simply making a new commit that deletes the key is **insufficient** as it remains in the Git commit history.
