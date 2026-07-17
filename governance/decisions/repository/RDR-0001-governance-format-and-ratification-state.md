# RDR-0001 — Governance Format and Ratification-State Transposition

| Field | Value |
| --- | --- |
| Record ID | `RDR-0001` |
| Record type | Repository Decision Record |
| Repository decision status | ACCEPTED |
| Master decision | RATIFIED |
| Master decision date | 17 July 2026 |
| Change class | Class A |
| Governing workstream | `[NTK-P00B]` Repository and Collaboration Foundation |
| Decision owner | Edgar Axel Pérez Flores |
| Required collaborator reviewer | Naomi Sánchez Torres |
| Master ratification authority | NTK-MASTER |
| Implementation authorization | AUTHORIZED |
| Implementation state | AUTHORIZED — NOT YET EFFECTIVE |
| Canonical transition | PENDING ADOPTION CONDITIONS |
| Submitted source commit | `637192b5e7709c0e6f2e28b3d24ea2693dd48dae` |
| Affected artifacts | Original LaTeX inputs `.ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex` and `.ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex`; authorized Markdown paths `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` and `governance/01_Project_Governance_and_Repository_Charter.md` |

---

## 1. Purpose

This record establishes a controlled transposition of the two foundational governance documents — the Scientific Constitution and the Project Governance and Repository Charter — with respect to two dimensions only: their **canonical file format** and their **settled-state metadata**. The ratified decision is to adopt Markdown as the canonical repository representation of these documents and to correct their surface metadata from foundational-draft wording to the settled, ratified state already recorded in the master project record. NTK-MASTER ratified this decision on 17 July 2026; implementation is authorized, and the canonical-format transition remains not yet effective until the adoption conditions in Section 6 are satisfied.

This record does **not** create a new scientific constitution or a new charter. It does not re-open, re-derive, or re-ratify the scientific or governance substance of either document. The substantive content of both instruments was ratified, and that ratified state is recorded in the master project record dated 16 July 2026; the ratification is presupposed here and is preserved intact. The decision ratified by NTK-MASTER concerns a change of representation and of settled-state description, not a change of meaning.

## 2. Context

The two governance documents were originally authored in LaTeX. Their embedded source metadata still describes them as foundational drafts: document `00` carries the declared source-state wording `Phase 0 Foundational Draft`, and document `01` carries `Gate 0B Foundational Draft`. Both declare source version `0.1.0` and source date 16 July 2026.

Subsequent to that authoring, the master project record — dated 16 July 2026 — recorded **both documents as ratified**. There is therefore a discrepancy between the settled governance state (ratified) and the surface metadata still carried by the LaTeX sources (foundational draft). The originals were never edited to reflect their settled state.

Repository foundation work is now active under Gate 0B on the working branch `foundation/scientific-governance`, and the repository is public. Governance documents rendered directly on GitHub improve accessibility and collaborator review: reviewers can read them in a browser, comment inline on pull requests, and follow durable version history without compiling LaTeX.

This change is **not purely mechanical**. Several ratified Gate 0B requirements presupposed that the governance documents would exist as `.tex` files and would be produced by LaTeX compilation — for example, canonical `.tex` governance paths in the initial architecture, clean-clone compilation of the governance documents, and continuous-integration compilation targeting them. Adopting Markdown as the canonical governance format changes those presupposed requirements. Because it alters ratified Gate 0B requirements, the change is a Class A change and must be represented by this record and ratified through NTK-MASTER before merge. The original decision-register entries must not be silently rewritten to make this transition appear to have been part of the original plan.

## 3. Accepted Decision

### 3.1 Canonical format and paths

Adopt Markdown as the canonical repository format for the two governance documents, at exactly these repository-relative paths:

```
governance/00_Scientific_Constitution_From_Newton_to_Kerr.md
governance/01_Project_Governance_and_Repository_Charter.md
```

The long filename stems are retained deliberately so that the canonical Markdown documents remain unambiguously identifiable with their originals. The monograph and the future preprint remain LaTeX works and are entirely out of scope for this format decision.

### 3.2 Authority transition

The authority relationship is stated here conditionally and precisely. NTK-MASTER has ratified this record and authorized its implementation, but the canonical-format transition is not yet effective: master ratification of `RDR-0001` alone did not change the canonical governance files.

- **Before** protected-`main` adoption — that is, before the Markdown transpositions are created, audited, compared, independently reviewed, signed off, and merged through the protected-`main` workflow — the authorized Markdown files have **no adopted authority**. They do not yet exist as adopted instruments, and no canonical-format transition is in effect.
- **Upon** completion of the adoption conditions in Section 6 — human comparison, collaborator review, final scientific sign-off, successful foundation checks, and merge through the protected-`main` workflow — the Markdown files become the **canonical repository governance instruments**.
- At that point the LaTeX originals become **provenance inputs only**. They carry no independent authority to override, reinterpret, or amend the Markdown canon, and they may not be used as a competing source of governance authority.
- The **ratification of the substantive Constitution and Charter is preserved** throughout. Only the canonical representation (format) and the settled-state metadata (tense and status wording) are transposed. No substantive re-ratification is asserted or required by this record.

### 3.3 Original-input provenance

This decision requires a provenance record at:

```
governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md
```

That record must contain the exact cryptographic identities of both original LaTeX inputs — byte counts, newline counts, carriage-return counts, leading-byte fingerprints, and SHA-256 digests — as independently captured. It must **not** reproduce or distribute the complete local-only LaTeX inputs. Its role is evidentiary: to bind each future Markdown transposition to a specific, verifiable source byte-stream.

### 3.4 Decision-register integrity

- The historical decision registers — `D0-01` through `D0-17` and `D0B-01` through `D0B-30` — remain **preserved in substantive form**.
- Historical decision entries will **not** be silently rewritten to make their original conditional or draft-era wording appear retroactively current. Their original meaning is frozen.
- This record, `RDR-0001`, carries the **explicit supersession and amendment relationship** for every requirement affected by the format transition (see Section 4).
- The converted documents **may** add a clearly marked amendment note, placed outside the frozen historical register, pointing to `RDR-0001`. They may **not** conceal, overwrite, or quietly alter the original recorded decisions.

### 3.5 Build and continuous-integration consequence

- The governance documents become canonical Markdown and are **no longer LaTeX compilation targets**.
- The Gate 0B reproducible LaTeX build **remains mandatory** for the monograph scaffold.
- Governance-document LaTeX compilation checks are **replaced** by Markdown governance checks.
- Later checks should include: structural integrity of the documents, presence of required metadata, preservation of stable identifiers, internal-link checks where reliable, and general repository hygiene.
- A passing CI workflow establishes only that these formal checks passed. It does **not** establish physical correctness, numerical fidelity, or scientific validation of any kind.

### 3.6 Overleaf boundary

- The long monograph and the future preprint remain **separate LaTeX projects**.
- Overleaf is an **independent authoring and compilation environment** for those works.
- **No automatic synchronization** between Overleaf and GitHub, or between Overleaf and VS Code, is planned.
- Transfer of monograph or preprint content to GitHub is **manual, reviewed, and version controlled**.
- The **merged GitHub source is the canonical version history**.
- Overleaf is **not a CI dependency** and is not part of any automated check.

### 3.7 Current collaborator state

- Naomi Sánchez Torres is the **confirmed Scientific Collaborator and Co-developer** and is authorized for public listing and repository collaborator access.
- A repository invitation **has been issued**.
- Invitation acceptance and the independent foundation-pull-request review **may remain operationally pending** at the time this record is prepared.
- This record does **not** determine final module ownership and does **not** determine publication author order. Those remain deferred.

## 4. Explicit Supersessions and Clarifications

The following table states, for each affected earlier requirement, its source area, the ratified disposition, and what remains unchanged. This table is the explicit record of supersession required by Section 3.4; nothing in the historical registers is edited to achieve these effects.

| Earlier requirement | Source area | Ratified disposition | What remains unchanged |
| --- | --- | --- | --- |
| Canonical `.tex` governance paths | Initial repository architecture | Superseded by the two exact `.md` paths: `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` and `governance/01_Project_Governance_and_Repository_Charter.md` | The identity and substance of the two governance documents; their long filename stems |
| Clean-clone build of governance **and** monograph documents | Gate 0B build requirement | Governance compilation retired; monograph scaffold clean-clone build retained | The monograph scaffold build remains mandatory and reproducible |
| CI compilation of governance documents | Gate 0B continuous integration | Replaced with Markdown integrity checks | Monograph compilation in CI is retained where applicable |
| `D0B-22` reproducible LaTeX build | Gate 0B decision register | Interpreted and amended to refer to the **monograph scaffold** LaTeX build | The requirement for a reproducible LaTeX build of the monograph scaffold |
| Gate 0B exit criterion 9 | Gate 0B exit criteria | Interpreted and amended to require the **monograph-scaffold clean-clone LaTeX build** | A clean-clone LaTeX build remains a Gate 0B exit condition, now scoped to the monograph scaffold |
| Overleaf boundary | Working-environment policy | Additive clarification, **not** a supersession of any source clause | The independence of Overleaf as an authoring and compilation environment |
| Long filename stem for document `00` | Naming convention | Explicitly adopted as `00_Scientific_Constitution_From_Newton_to_Kerr.md` | The document's identity, scope, and substance |

## 5. Explicit Nonchanges

`RDR-0001` does **not** change any of the following:

- the project thesis;
- the mandatory scientific spine;
- the research questions or hypotheses;
- the physical conventions;
- the theory-first doctrine;
- the physics-to-software contracts;
- the evidence hierarchy `E0`–`E5`;
- the validation requirements;
- the scientific exclusions and nonclaims;
- the human authority boundaries;
- the independent-review requirements;
- the collaborator role boundaries;
- the deferred module allocation;
- the deferred publication author order;
- the licensing doctrine;
- the publication doctrine;
- the completion criteria;
- the production-code authorization state.

Any apparent substantive drift discovered in the Markdown transpositions is by definition a **conversion defect**. It must be corrected against the ratified LaTeX originals. It must **not** be silently accepted, normalized, or ratified through this record. This record grants no authority to change substance under the guise of formatting.

## 6. Adoption Conditions

Adoption of this record and of the resulting canonical Markdown transition requires **all** of the following. Condition 1 is now satisfied — NTK-MASTER ratified `RDR-0001` on 17 July 2026 — and the remaining conditions stay pending:

1. NTK-MASTER ratification of `RDR-0001`;
2. faithful Markdown transposition of both governance documents;
3. human comparison of each transposition against its original input;
4. Naomi Sánchez Torres's collaborator review once repository access is active;
5. Edgar Axel Pérez Flores's explicit final scientific sign-off;
6. inclusion of the exact provenance record at `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md`;
7. all required checks passing;
8. no unresolved blocking review comment;
9. no forbidden architecture and no unsupported scientific claim introduced;
10. the foundation pull request merged through the protected-`main` workflow.

Until every one of these conditions is satisfied, the authorized Markdown documents have no adopted authority, and the canonical transition remains not yet effective.

## 7. Risks and Mitigations

| Risk | Description | Mitigation |
| --- | --- | --- |
| Conversion loss | Substantive content silently dropped or weakened during LaTeX-to-Markdown conversion | Mandatory human comparison of each transposition against its ratified original (Adoption Conditions 3 and 5); any drift treated as a defect per Section 5 |
| Identifier loss | Stable identifiers (`D0-*`, `D0B-*`, section and decision IDs) lost or renumbered | Preservation of stable identifiers is a required structural check (Section 3.5); registers preserved in substantive form (Section 3.4) |
| Mathematical-rendering differences | Equations rendered differently or incorrectly in GitHub-compatible math syntax | Equations preserved in GitHub-compatible math; human review of rendered mathematics during comparison; defects corrected against originals |
| Historical-record rewriting | Draft-era conditional wording quietly edited to appear retroactively current | Historical registers frozen; supersessions carried only by this record's Section 4 table; amendment notes marked and kept outside the frozen register |
| Dual-authority ambiguity | Uncertainty over whether LaTeX or Markdown governs after transition | Section 3.2 states a single, conditional authority transition; after merge the LaTeX originals are provenance-only and cannot override the Markdown canon |
| Manual Overleaf transfer divergence | Monograph or preprint content in Overleaf diverging from the GitHub canon | Overleaf transfer is manual, reviewed, and version controlled; merged GitHub source is the canonical history; Overleaf is not a CI dependency |
| Validation misinterpretation | Passing Markdown checks mistaken for scientific validation | Section 3.5 states explicitly that CI success is not physical correctness or scientific validation; nonclaims restated in Section 5 |

## 8. Alternatives Considered

**A. Keep LaTeX as the sole canonical governance format.** The governance documents would remain `.tex` files and would retain the previously planned compilation requirements. This preserves the original toolchain but provides a less accessible rendered experience for casual GitHub readers and makes browser-first review less convenient. This alternative was not selected in this ratified decision.

**B. Maintain LaTeX and Markdown as co-equal canonical sources.** Both formats would be authoritative simultaneously. **This alternative was not selected in this ratified decision.** Co-equal canonical sources create a standing dual-authority hazard: any divergence between the two representations produces genuine ambiguity about which governs, invites silent drift, and forces every reviewer and every check to reconcile two sources of truth. Governance requires a single canonical instrument.

**C. Use Markdown as the canonical governance format with hashed LaTeX provenance.** Markdown becomes the single canonical format at the two exact paths; the LaTeX originals are retained locally, unmodified and untracked, and bound to the canon by exact cryptographic identity in the provenance record. This yields a single source of authority, a browser-reviewable public canon, and a verifiable evidentiary link back to the ratified originals.

**Alternative C is the selected and ratified alternative.** NTK-MASTER ratified it on 17 July 2026. It resolves the dual-authority hazard that defeats Alternative B while retaining full provenance, and it delivers the public-review benefits that Alternative A cannot.

## 9. Consequences

**Positive consequences.**

- A single, unambiguous canonical governance format.
- Governance documents readable, diffable, and reviewable directly on GitHub.
- Settled-state metadata aligned with the ratified reality recorded by the master project record.
- A verifiable cryptographic link from each future transposition back to its ratified source.

**Accepted limitations.**

- Governance documents are no longer produced by LaTeX compilation; the governance LaTeX toolchain step is retired.
- Some LaTeX constructs must be expressed in GitHub-compatible Markdown and math syntax, which may render differently and requires human review.
- Two representations of each document exist during the transition window until merge resolves authority.

**Deferred work.**

- Creation of the two Markdown transpositions (now authorized as the next implementation step; they do not become canonical until the adoption conditions in Section 6 are met).
- Definition and implementation of the Markdown governance checks and CI workflow.
- Final module ownership and publication author order remain deferred.

This decision is **accepted and its implementation is authorized**, while the **canonical transition remains not yet effective**. The consequences above describe what the canonical adoption entails, conditioned on completion of the adoption conditions in Section 6.

## 10. Review and Ratification Record

| Step | Party | State |
| --- | --- | --- |
| Drafting assistance | Claude Code under bounded instruction | completed |
| Master ratification | NTK-MASTER, 17 July 2026 | completed |
| Responsible human comparison of both transpositions | Edgar Axel Pérez Flores | pending |
| Independent collaborator review | Naomi Sánchez Torres | pending |
| Final scientific sign-off | Edgar Axel Pérez Flores | pending |
| Required checks | Gate 0B foundation checks | pending |
| Implemented in | Foundation pull request | pending |
| Adopted foundation merge commit or tag | — | pending |

Claude Code has **no scientific, authorship, ratification, independent-review, final-sign-off, or Git authority whatsoever**. Its role is strictly limited to drafting and amending this record under bounded instruction. It does not perform, and cannot substitute for, any scientific judgment, any authorship, the master ratification, the responsible human comparison, the independent collaborator review, the final scientific sign-off, or any Git staging, commit, push, tag, branch, or configuration action. All scientific judgment, all authorship, all comparison, all independent review, all final sign-off, and all Git operations are performed exclusively by the authorized human parties named above; NTK-MASTER is the sole ratification authority, and Edgar Axel Pérez Flores alone performs all Git operations.

## 11. Decision State

- `RDR-0001` is **ACCEPTED**.
- **NTK-MASTER ratified** this record on **17 July 2026**.
- Implementation is **AUTHORIZED**.
- The canonical transition is **NOT YET EFFECTIVE**.
- The adoption conditions in Section 6 remain **PENDING**.
- **Phase 1 remains BLOCKED.**
- **Production Python remains BLOCKED.**
- The next authorized implementation is preparation and audit of the two Markdown transpositions — `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` and `governance/01_Project_Governance_and_Repository_Charter.md` — together with the permanent transposition audit at `governance/provenance/RDR-0001_TRANSPOSITION_AUDIT.md`. None of these files exist yet, and creating them does not make them canonical; the canonical transition becomes effective only after all adoption conditions in Section 6 are satisfied and the foundation pull request is merged through the protected-`main` workflow.
