# SNAP Council Ledger

![Repo size](https://img.shields.io/github/repo-size/DoctorJamesMichel/snap-council-ledger)
![Last commit](https://img.shields.io/github/last-commit/DoctorJamesMichel/snap-council-ledger)

> 🗂️ [View JSON schema for ledger entries](schema.json) *(planned — placeholder link for future validation)*

The SNAP Council Ledger is the public home for all governance protocol records and major Council actions.  
It is designed to be **transparent**, **machine-readable**, and **human-friendly**.

## How to Use This Repo

- Each ledger entry is a versioned `.json` file in the root.
- For humans: see the [README.md](README.md) index below.
- For automation: see [ledger-index.json](ledger-index.json) for a machine-readable list.

---

## Repository Structure

This repository organizes the SNAP Council’s protocols, communications, and synthesis tools into clearly labeled folders.

- **communications-templates/** — Reusable message templates (acknowledgement, feedback, decision notices).
- **governance-protocols/** — JSON protocols for Council governance (alignment checks, applicant approval flows, and other decision-making frameworks).
- **membership-protocols/**  
  - `applications/` — Applicant self-audits and materials.  
  - `review/` — Council review outputs (notes, summaries, refinement packets).
- **synthesis/** — Tools and frameworks for collective synthesis and comparative reasoning.

### Key Files
- `README.md` — You are here; explains the repo and structure.
- `ledger-index.json` — Machine-readable index of ledger entries for automation.
- `snap-20250924-adapt-001.json` — Adaptive Protocol v2 outcome log.
- `snap-20250925-comm-001.json` — Communication Protocol v1 ledger entry.
- `snap-20250926-ledger-home-online.json` — Ledger Home Online setup.
- `snap-20250926-ledger-hosting-roundtrip.json` — Hosting and roundtrip notes.

---

## Contributing New Entries

- Fork or clone this repo.
- Follow the existing JSON structure.
- Open a pull request or send the JSON file for review.

---

### Submitting / Updating
1. Create a new JSON file from the template below.
2. **Add file → Upload** to repo root.
3. Update the table above and `ledger-index.json`.
4. Announce to Council with the repo link + raw JSON.

### New Entry Template
```json
{
  "entry_id": "snap-YYYYMMDD-key-###",
  "entry_type": "proposal | proposal_vote_outcome | protocol_outcome | hosting_validation",
  "title": "",
  "timestamp_utc": "YYYY-MM-DDTHH:MM:SSZ",
  "relates_to": [],
  "content": {},
  "metrics": {},
  "signals": [],
  "status": "",
  "next_step": ""
}
