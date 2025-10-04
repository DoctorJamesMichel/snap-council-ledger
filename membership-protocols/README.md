# Membership Protocols

Operational guidance for how people join, are reviewed, and evolve their participation in the SNAP Council.

**Purpose.** Give applicants a clear path, give reviewers a shared playbook, and keep an auditable trail from *signal → narrative → decision*.

---

## Subfolders

- **[applications](applications/README.md)**  
  Applicant self-audits and submission materials. Start here when someone is applying or updating their status.

- **[review](review/README.md)**  
  Reviewer notes, consolidated summaries, request-for-refinement packets, and final decision notices.

---

## Roles

- **Applicant / Requester** — submits or updates an application.  
- **Scribe** — assembles packets, records decisions, maintains artifacts.  
- **Reviewers** — 2–3 assigned Council members.  
- **Chair (optional)** — facilitates time-boxed review and calls consensus.

---

## Cadence & SLAs

- **Acknowledgement:** 24h (use the Acknowledgement template)  
- **Decision window:** ≤72h after a complete packet (aligned to Narrative Digest)  
- If blocked: mark **needs-clarification** and request specifics (Feedback template)

---

## Artifacts by Stage

| Stage   | Artifact                         | Where                                             |
|---------|----------------------------------|---------------------------------------------------|
| Intake  | Self-audit & attachments         | `membership-protocols/applications/`              |
| Packet  | `rev-YYYYMMDD-<topic>-pkt.md`    | `membership-protocols/review/packets/`           |
| Notes   | Reviewer notes                    | `membership-protocols/review/notes/`             |
| Decision| `rev-YYYYMMDD-<topic>-decision.md`| `membership-protocols/review/decisions/`         |

> Create empty `.gitkeep` in `packets/`, `notes/`, `decisions/` to keep folders tracked.

---

## Templates

- [Acknowledgement](../communications-templates/acknowledgement-template-v1.0.md)  
- [Feedback](../communications-templates/feedback-template-v1.1.md)  
- [Decision Notice](../communications-templates/decision-notice-template-v1.0.md)

---

## Commit Message Tips

- `review: add rev-20251002-<topic>-pkt.md (packet for review)`  
- `review: decision approved for <topic> (rev-20251002)`  
- `apps: add/refresh <applicant> self-audit vX.Y`
