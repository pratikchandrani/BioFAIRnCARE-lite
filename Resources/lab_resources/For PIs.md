---
type: guide
id: for-pis
title: "For PIs"
description: "How a PI checks and archives a student's Lite vault after receiving it."
created: 2026-10-02
updated: 2026-10-02
status: active
owner: Lab
confidentiality: public
license: CC-BY-4.0
ai_assisted: false
lab_owned: true
---

# For PIs — checking and archiving a student's vault

In the Lite edition nothing is approved inside the student's vault. Students keep their records and
hand the vault to you when you ask — as a zipped copy or by giving you read access to their private
GitHub repository (see *Sharing your vault with your PI* in the [[New Student Note-Taking Guide]]).
How and when you check and archive is up to you; this note is a suggestion.

## Looking through a received vault

1. Open the vault folder in Obsidian (or unzip it first) and open [[Vault Health]] — it lists
   missing properties, broken links, oversize or raw files, and missing CARE / ethics fields.
2. Skim the [[Experiments/_Index|Experiments]] index: completed experiments should have `end_date`,
   `outcome` and, for failed or negative results, an `outcome_reason`.
3. For human or community-derived material, check the CARE fields and ethics approvals
   ([[CARE guide]]); for animal work, the IAEC approval, humane end-points and 3Rs statement.
4. Check that raw and large data are registered as data references with location and checksum
   ([[Data capture guide]]) rather than stored in the vault.
5. Optional, on a computer with Python: run `python Resources/tools/validate_vault.py` inside the
   vault for the full check.

## Archiving

- Keep each received copy **read-only** in lab storage, named with the student and the date, e.g.
  `Archive/<Student>/<YYYY-MM-DD>_vault.zip`. That copy is the authoritative record.
- Follow the lab's backup rule (3 copies, 2 media, 1 off-site) for the archive.
- If you find something to correct, ask the student to fix it in their vault and add a dated line
  under *Amendments*; the next copy you receive will contain it. Never edit an archived copy.
