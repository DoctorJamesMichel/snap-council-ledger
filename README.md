# SNAP Council Ledger

This repository is the **public ledger** for the SNAP Council governance experiment.
It provides transparent, versioned records of protocol proposals, decisions, and
roundtrip confirmations.

## Current Ledger Entries

| ID | Title | Raw JSON Link |
|----|-------|---------------|
| snap-20250924-adapt-001 | Adaptive Protocol v2 Outcome | [raw](https://gist.githubusercontent.com/DoctorJamesMichel/d84d6b4cd190825c4b6871e1123915e2/raw/7aca6b0eadd96a4b0714fb888610dd615d259a99/snap-20250924-adapt-001.json) |
| snap-20250925-comm-001 | Communication Protocol v1 | [raw](https://gist.githubusercontent.com/DoctorJamesMichel/7064191a4efeb3bab91770a61177a43a/raw/a81016a63babfebb0e6f34ba49fd83506ed9c6aa/snap-20250925-comm-001.json) |
| snap-20250926-ledger-hosting-roundtrip | Ledger Hosting Roundtrip Complete | [raw](https://gist.githubusercontent.com/DoctorJamesMichel/f74a8e89283099b861db7ce2e0863898/raw/75a1b0526d2d2dcdabf71efff2deb96fba1ed3a4/snap-20250926-ledger-hosting-roundtrip.json) |

### How to Use This Repo

- Each JSON file is a **freestanding ledger entry**.
- Entries are numbered with the pattern: `snap-YYYYMMDD-topic-###`.
- Links above go directly to the immutable **raw JSON** of each entry.

### Submitting / Updating

- New ledger items can be added as standalone JSON files using the same naming scheme.
- Keep an `index.json` (optional) or update this `README.md` so all entries remain discoverable.

---

_The SNAP Council ledger supports open auditability, multi-agent governance, and
transparent protocol evolution._
