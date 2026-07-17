# Original Ratification Inputs — Provenance and Integrity Record

| Field | Value |
| --- | --- |
| Record status | DRAFT |
| Record date | 17 July 2026 |
| Responsible owner | Edgar Axel Pérez Flores |
| Governing workstream | `[NTK-P00B]` Repository and Collaboration Foundation |
| Related decision | `RDR-0001` |
| Canonical-transition state | Proposed, not yet adopted |

---

## 1. Purpose and Scope

This record identifies, by exact cryptographic identity, the two local-only LaTeX inputs selected as the sources for the planned Markdown transposition of the project's governance documents. Its purpose is to bind each future Markdown transposition to a specific, verifiable byte-stream, so that any later reviewer can confirm which exact source bytes a transposition was derived from.

This is an **evidentiary provenance record**, not an independent governance instrument. It confers no authority, ratifies nothing, and does not itself adopt `RDR-0001`. It records identity and integrity evidence only.

## 2. Authority Boundary

- The master project record recognizes the substantive Scientific Constitution and the Project Governance and Repository Charter as **ratified**.
- Until `RDR-0001` and the Markdown transpositions are ratified through NTK-MASTER and merged, **no new canonical-format transition has occurred**. The current canonical representation is unchanged by this record.
- If `RDR-0001` is adopted, the Markdown documents become canonical and these LaTeX files remain **provenance evidence only**.
- The originals may **not** later be used as a competing source of governance authority, nor to override, reinterpret, or amend the Markdown canon once that canon is adopted.

## 3. Original Input Inventory

The following identity values are recorded exactly as independently verified. They must be reproduced without alteration.

| Attribute | Input 00 | Input 01 |
| --- | --- | --- |
| Document | Scientific Constitution — *From Newton to Kerr* | Project Governance and Repository Charter |
| Original filename | `00_Scientific_Constitution_From_Newton_to_Kerr.tex` | `01_Project_Governance_and_Repository_Charter.tex` |
| Local-only relative path | `.ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex` | `.ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex` |
| Declared version | `0.1.0` | `0.1.0` |
| Declared source date | 16 July 2026 | 16 July 2026 |
| Declared source-state wording | `Phase 0 Foundational Draft` | `Gate 0B Foundational Draft` |
| File classification | LaTeX 2e document, ASCII text | LaTeX 2e document, ASCII text |
| MIME and charset | `text/x-tex; charset=us-ascii` | `text/x-tex; charset=us-ascii` |
| Exact bytes | `38899` | `43382` |
| Newline count from `wc -l` | `910` | `1068` |
| CR byte count | `0` | `0` |
| First three bytes, hexadecimal | `5c646f` | `5c646f` |
| SHA-256 | `6ac268e9d4772a8c6ff0a9a5d5c53752571126ea925b873f6907c3ee0d16bc46` | `fb74ae936a6dba21efe4aab1d6b6f099d57dbeded6ca56c55cff0ce6c33af3f4` |

## 4. Independent Hash Verification

The SHA-256 digest of each input was computed by two independent tools and compared:

- Primary computation: `sha256sum`.
- Independent computation: Windows `CertUtil` with the `SHA256` algorithm.
- Result: **exact agreement** between the two computations for **both** files.
- Capture date: 17 July 2026.
- Responsible human: Edgar Axel Pérez Flores.
- No file was modified, tracked, staged, committed, or pushed during capture.

No command output beyond the facts stated here is asserted.

## 5. Status History

**Input 00 — Scientific Constitution.**

- Authored with foundational-draft metadata (`Phase 0 Foundational Draft`, version `0.1.0`) on 16 July 2026.
- Subsequently recorded as **ratified** by the master project state.
- Selected, as a local-only source, to be the transposition input for the canonical Markdown document.
- Cryptographic identity captured on 17 July 2026.
- Markdown adoption remains **proposed** under `RDR-0001`.

**Input 01 — Project Governance and Repository Charter.**

- Authored with foundational-draft metadata (`Gate 0B Foundational Draft`, version `0.1.0`) on 16 July 2026.
- Subsequently recorded as **ratified** by the master project state.
- Selected, as a local-only source, to be the transposition input for the canonical Markdown document.
- Cryptographic identity captured on 17 July 2026.
- Markdown adoption remains **proposed** under `RDR-0001`.

No exact historical signature time and no unrecorded personal acknowledgement date are asserted for either document.

## 6. Planned Transformation Relationship

The future Markdown transpositions may contain **only** the following kinds of transformation relative to their LaTeX originals:

- mechanical LaTeX-to-Markdown conversion;
- explicit expansion of LaTeX macros;
- preservation of equations in GitHub-compatible math syntax;
- conversion of tables, lists, quotations, and code blocks;
- settled-state metadata and tense corrections;
- explicit amendment notes authorized by `RDR-0001`.

The transpositions may **not** contain any of the following:

- a changed scientific spine;
- altered evidence thresholds;
- changed role authority;
- changed publication doctrine;
- new scientific claims;
- unsupported citations;
- production architecture;
- silent rewriting of historical decision registers.

## 7. Retention and Repository Treatment

- The originals remain under `.ntk-local-inputs/`.
- They are ignored by `.gitignore` (the directory `.ntk-local-inputs/` is an ignore rule).
- They are **not tracked** by Git.
- No absolute machine path is recorded in this repository.
- The repository stores only this identity and provenance record, not the source inputs themselves.
- Redistribution of the source inputs is unnecessary once the faithful transposition and the human comparison are complete.
- Edgar Axel Pérez Flores retains responsibility for the original local copies during Gate 0B.

## 8. Reverification Procedure

The identity of each input can be reverified with the following non-destructive commands, run from the repository root. These commands read the files only; they do not modify, add, or track them.

```bash
# SHA-256, primary tool
sha256sum .ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex
sha256sum .ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex

# Byte count and newline count
wc -c .ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex
wc -l .ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex
wc -c .ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex
wc -l .ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex

# Confirm the inputs are ignored by Git
git check-ignore -v .ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex
git check-ignore -v .ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex
```

```bat
:: SHA-256, independent tool (Windows)
certutil.exe -hashfile .ntk-local-inputs\00_Scientific_Constitution_From_Newton_to_Kerr.tex SHA256
certutil.exe -hashfile .ntk-local-inputs\01_Project_Governance_and_Repository_Charter.tex SHA256
```

A reverification is successful when both SHA-256 tools agree with each other and with the digests recorded in Section 3, the byte and newline counts match, and `git check-ignore` confirms each input is ignored.

## 9. Limitations and Nonclaims

- The hashes prove **byte identity** of the source inputs; they do not prove correctness of their content.
- Matching hashes do **not** prove the **semantic fidelity** of any future Markdown conversion; only human comparison against the originals can establish that.
- The ASCII classification does **not** mean the documents lack accented human names. The LaTeX source may encode accented characters through LaTeX commands rather than as non-ASCII bytes.
- The `wc -l` values recorded in Section 3 are **newline counts**, not a universal semantic line count.
- This record is **not** scientific validation.
- This record does **not** itself adopt `RDR-0001`.

## 10. Current State

- Both source inputs verified.
- Both hashes independently reproduced, in exact agreement.
- Both inputs ignored and untracked.
- Repository canonical transition **pending**.
- Next step: human review of this record and of `RDR-0001`.
