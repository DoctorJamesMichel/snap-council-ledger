# Contributing to the SNAP Council Ledger

Thanks for your interest in helping steward the SNAP Council Ledger!  
This repo exists to keep Council protocols transparent, auditable, and easy to evolve.

---

## How to Contribute

### 1. Fork and Clone
- Fork this repository and clone your fork locally.
- Or, if you’re a Council member with write access, you may branch directly.

### 2. Add or Update Files
- Follow the file structure and versioning you see in the repo:
  - **communications-templates/** — reusable Council communication templates (e.g., `feedback-template-v1.1.md`)
  - **governance-protocols/** — versioned JSON flows and audits (e.g., `applicant-approval-flow-v1.0.json`)
  - **membership-protocols/** — applicant self-audits and Council review artifacts
  - **synthesis/** — comparative reasoning, combined learnings, or experimental frameworks
- Each new file should be:
  - Clearly named
  - Versioned (`-vX.Y`)
  - Self-contained and machine/human-readable

### 3. Update Indexes When Needed
- If adding a new ledger event, update:
  - **ledger-index.json** — add a new object with date, ID, and title.
  - **README.md** — ensure the event appears under *Current Entries*.

### 4. Commit Conventions
- Use clear, past-tense commit messages:
  - *Add*: for new files (e.g., `Add applicant-approval-flow-v1.0.json (new protocol flow)`)
  - *Update*: for edits (e.g., `Update feedback-template to v1.1 for clarity`)
  - *Docs*: for README or CONTRIBUTING changes (e.g., `Docs: add repository structure section`)

### 5. Pull Request / Review
- Open a PR if you’re working from a fork or branch.
- Tag the Council Scribe (or other reviewers) for sign-off.

---

## Questions / Discussion
Open a GitHub issue or ping the Council Scribe.  
SNAP thrives on clarity and shared stewardship — thank you for helping evolve our living record.
