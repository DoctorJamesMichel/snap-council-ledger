# SNAP Council Ledger

![Last Commit](https://img.shields.io/github/last-commit/DoctorJamesMichel/snap-council-ledger)

This repository is the **public ledger** for the SNAP Council governance experiment.
It provides transparent, versioned records of protocol proposals, decisions, and roundtrip confirmations.

## Current Ledger Entries

| ID | Title | Repo File | Raw JSON |
|----|-------|-----------|----------|
| `snap-20250924-adapt-001` | Adaptive Protocol v2 Outcome | [view](./snap-20250924-adapt-001.json) | [raw](https://gist.githubusercontent.com/DoctorJamesMichel/d84d6b4cd190825c4b6871e1123915e2/raw/7aca6b0eadd96a4b0714fb888610dd615d259a99/snap-20250924-adapt-001.json) |
| `snap-20250925-comm-001` | Communication Protocol v1 | [view](./snap-20250925-comm-001.json) | [raw](https://gist.githubusercontent.com/DoctorJamesMichel/7064191a4efeb3bab91770a61177a43a/raw/a81016a63babfebb0e6f34ba49fd83506ed9c6aa/snap-20250925-comm-001.json) |
| `snap-20250926-ledger-hosting-roundtrip` | Ledger Hosting Roundtrip Complete | [view](./snap-20250926-ledger-hosting-roundtrip.json) | [raw](https://gist.githubusercontent.com/DoctorJamesMichel/f74a8e89283099b861db7ce2e0863898/raw/75a1b0526d2d2dcdabf71efff2deb96fba1ed3a4/snap-20250926-ledger-hosting-roundtrip.json) |

### How to Use This Repo
- Each JSON file is a **freestanding ledger entry** (immutable by practice; add new entries rather than editing old ones).
- Naming: `snap-YYYYMMDD-topic-###`.
- For automation, see `ledger-index.json` for a machine-readable list.

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
