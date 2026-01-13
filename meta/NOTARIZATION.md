# NOTARIZATION — ECISA Repository

This file records external timestamping / notarization events for the ECISA core documents.

## 1. Scope

The following files are considered the canonical core for integrity purposes:

- `docs/ECISA_Model_Act_v0.1.md`
- `docs/ECISA_CIS_Template_v1.0.md`
- `docs/ECISA_EFR_Template_v1.0.md`
- `meta/HASHES.md` (meta-manifest of the above)

## 2. OpenTimestamps or equivalent

When you are ready to anchor:

1. Generate or update `meta/HASHES.md`.
2. Upload `meta/HASHES.md` to an external timestamping service (e.g., OpenTimestamps).
3. Save the resulting receipt file in this repository, e.g.:

   - `meta/ots/ECISA_hashes.txt.ots`

4. Record the event here:

- Date:
- Service used:
- File hashed:
- Receipt filename:
- Notes:

## 3. Additional notarization

If you later notarize or record these hashes in:

- a blockchain transaction,
- a public notary system,
- or institutional records,

record the details here with:

- Date,
- Method,
- Reference / transaction ID.
