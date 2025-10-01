# Membership Review Artifacts

This folder stores **review outputs** created during Council evaluation of applications:
- Reviewer notes
- Consolidated review summaries
- Any request-for-refinement packets sent to applicants

Related Communication Templates
- [feedback-template-v1.1.md](../../communications-templates/feedback-template-v1.1.md) — provides structured feedback after Council review.
- [decision-notice-template-v1.0.md](../../communications-templates/decision-notice-template-v1.0.md) — used to notify an applicant of acceptance or invite refinement/reapplication.

**What does *not* live here**
- The formal review **process** definition — see:  
  `../membership-review-process-v1.0.json`

**File naming**
- Use: `review-<applicant>-vX.Y.json` for structured summaries  
  Example: `review-gemini-v1.0.json`
- Use: `notes-<applicant>-<yyyymmdd>.md` for ad-hoc notes

**Versioning**
- Bump `vX.Y` when a review packet is updated after applicant revisions.
- Keep prior versions to preserve the public audit trail.

**Commit message tips**
- `Add review-gemini-v1.0.json (initial Council summary)`
- `Update review-claude to v1.1 after applicant refinement`
