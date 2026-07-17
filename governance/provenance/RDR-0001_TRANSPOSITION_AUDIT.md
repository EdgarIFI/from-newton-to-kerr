# RDR-0001 Transposition Audit

| Field | Value |
| --- | --- |
| Record status | DRAFT |
| Record date | 17 July 2026 |
| Governing workstream | `[NTK-P00B]` Repository and Collaboration Foundation |
| Related decision | `RDR-0001` — RATIFIED |
| Canonical transition | AUTHORIZED — NOT YET EFFECTIVE |
| Audit coverage | Document 00 transposition completed; Document 01 not yet performed |
| Responsible owner | Edgar Axel Pérez Flores |
| Required collaborator reviewer | Naomi Sánchez Torres |
| Human comparison state | PENDING |
| Independent review state | PENDING |
| Final scientific sign-off | PENDING |
| Adoption evidence | PENDING |

---

## 1. Purpose and Authority Boundary

This audit records the traceability of the Markdown transposition work authorized by the ratified repository decision `RDR-0001`. It binds each transposition output to its exact source byte stream and documents every structural mapping, macro expansion, mathematical conversion, and non-mechanical change.

This audit does **not** itself establish semantic fidelity, canonical adoption, scientific validation, human review, or final sign-off. Automated and Claude-assisted comparisons recorded here are preliminary traceability evidence only. Semantic fidelity can be established only by the pending human source-to-output comparison, the pending independent collaborator review, and the pending final scientific sign-off. The canonical-format transition remains not yet effective until all `RDR-0001` adoption conditions are satisfied and the foundation contribution is merged through protected `main`.

## 2. Authoritative Source Inventory

Document `00` source identity, independently reverified before conversion on 17 July 2026:

| Attribute | Value |
| --- | --- |
| Document | Scientific Constitution — *From Newton to Kerr* |
| Source path | `.ntk-local-inputs/00_Scientific_Constitution_From_Newton_to_Kerr.tex` |
| Source filename | `00_Scientific_Constitution_From_Newton_to_Kerr.tex` |
| Declared source version | `0.1.0` |
| Declared source date | 16 July 2026 |
| Declared source-state wording | `Phase 0 Foundational Draft` |
| Classification | LaTeX 2e document, ASCII text |
| MIME and charset | `text/x-tex; charset=us-ascii` |
| Exact bytes | `38899` |
| Newline count from `wc -l` | `910` |
| CR byte count | `0` |
| First three bytes, hexadecimal | `5c646f` |
| SHA-256 | `6ac268e9d4772a8c6ff0a9a5d5c53752571126ea925b873f6907c3ee0d16bc46` |
| Git state | ignored (`.gitignore` rule `.ntk-local-inputs/`) and untracked |

All values above agree exactly with `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md` and with the identities independently accepted by the NTK-MASTER ratification of `RDR-0001`.

Document `01` (`01_Project_Governance_and_Repository_Charter.tex`) has **not** been transposed in this task. Its source identity is already recorded in `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md` and is not restated here as transposition evidence.

## 3. Output Inventory

Document `00` output:

| Attribute | Value |
| --- | --- |
| Output path | `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` |
| Exact bytes | `41971` |
| Newline count from `wc -l` | `711` |
| Encoding | UTF-8 (validated by strict decode) |
| Line-ending state | LF-only; CR byte count `0`; final byte `0x0a` |
| SHA-256 | `61871118be82dff1247e91efcc177c53573268f048bcbcd4fba53ff0356a6f9d` |
| Creation state | AUTHORIZED DRAFT — NOT YET CANONICAL |

Document `01` output: **no output exists yet.** The path `governance/01_Project_Governance_and_Repository_Charter.md` is intentionally absent from the repository at this stage.

## 4. Source-to-Output Structural Mapping

Source locators are line numbers in the `.tex` source; output locators are line numbers and GitHub anchors in the Markdown output. Dispositions: `converted` (mechanical transposition), `added` (authorized non-mechanical addition, see Section 9), `restructured` (authorized representation change, see Section 9).

| # | Source level | Source heading or element | Source locator | Markdown heading or element | Output locator / anchor | Disposition | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | title block | `\title`, `\author`, `\date`, `\maketitle` | 39–46 | `#` title, subtitle line, metadata table | 1–20 | restructured | Version/date/state moved into metadata table; see Section 9 |
| 2 | — | (not in source) | — | `## Canonical-Format Amendment Note` | 22 / `#canonical-format-amendment-note` | added | Authorized by `RDR-0001` §3.4 |
| 3 | environment | `abstract` | 48–62 | `## Abstract` | 35 / `#abstract` | converted | Verbatim prose; macros expanded |
| 4 | command | `\tableofcontents` | 64 | `## Contents` | 39 / `#contents` | converted | Rebuilt as Markdown anchor links |
| 5 | section | Purpose and Authority of This Constitution | 67 | `## 1. Purpose and Authority of This Constitution` | 97 / `#1-purpose-and-authority-of-this-constitution` | converted | Explicit numbering added to reproduce LaTeX auto-numbering |
| 6 | section | Project Identity | 88 | `## 2. Project Identity` | 110 / `#2-project-identity` | converted | — |
| 7 | subsection | Formal identity | 90 | `### 2.1 Formal identity` | 112 / `#21-formal-identity` | converted | — |
| 8 | subsection | Positioning statement | 105 | `### 2.2 Positioning statement` | 126 / `#22-positioning-statement` | converted | — |
| 9 | subsection | Strategic academic objective | 119 | `### 2.3 Strategic academic objective` | 134 / `#23-strategic-academic-objective` | converted | — |
| 10 | section | Central Scientific Thesis | 138 | `## 3. Central Scientific Thesis` | 148 / `#3-central-scientific-thesis` | converted | Includes chain display equation |
| 11 | section | Research Questions and Working Hypotheses | 168 | `## 4. Research Questions and Working Hypotheses` | 172 / `#4-research-questions-and-working-hypotheses` | converted | — |
| 12 | subsection | Primary research questions | 170 | `### 4.1 Primary research questions` | 174 / `#41-primary-research-questions` | converted | Description list → bold-label list |
| 13 | subsection | Working hypotheses | 192 | `### 4.2 Working hypotheses` | 182 / `#42-working-hypotheses` | converted | Description list → bold-label list |
| 14 | section | Mandatory Scientific Spine | 213 | `## 5. Mandatory Scientific Spine` | 191 / `#5-mandatory-scientific-spine` | converted | — |
| 15 | subsection | M1: Kepler problem and central-force foundations | 218 | `### 5.1 M1: Kepler problem and central-force foundations` | 195 / `#51-m1-kepler-problem-and-central-force-foundations` | converted | — |
| 16 | subsection | M2: Geometric numerical integration laboratory | 237 | `### 5.2 M2: Geometric numerical integration laboratory` | 209 / `#52-m2-geometric-numerical-integration-laboratory` | converted | — |
| 17 | subsection | M3: Circular restricted three-body problem | 253 | `### 5.3 M3: Circular restricted three-body problem` | 221 / `#53-m3-circular-restricted-three-body-problem` | converted | — |
| 18 | subsection | M4: First post-Newtonian test-particle bridge | 271 | `### 5.4 M4: First post-Newtonian test-particle bridge` | 235 / `#54-m4-first-post-newtonian-test-particle-bridge` | converted | — |
| 19 | subsection | M5: Schwarzschild geodesic dynamics | 289 | `### 5.5 M5: Schwarzschild geodesic dynamics` | 248 / `#55-m5-schwarzschild-geodesic-dynamics` | converted | — |
| 20 | subsection | M6: Kerr geodesic dynamics | 305 | `### 5.6 M6: Kerr geodesic dynamics` | 260 / `#56-m6-kerr-geodesic-dynamics` | converted | `(a)/(b)` labels preserved literally |
| 21 | subsection | M7: Curated relativistic orbit atlas | 321 | `### 5.7 M7: Curated relativistic orbit atlas` | 269 / `#57-m7-curated-relativistic-orbit-atlas` | converted | Macros `\E`, `\Lz` expanded in math |
| 22 | section | Explicit Exclusions and Nonclaims | 337 | `## 6. Explicit Exclusions and Nonclaims` | 281 / `#6-explicit-exclusions-and-nonclaims` | converted | — |
| 23 | section | Global Mathematical and Physical Conventions | 359 | `## 7. Global Mathematical and Physical Conventions` | 300 / `#7-global-mathematical-and-physical-conventions` | converted | — |
| 24 | subsection | Relativistic conventions | 361 | `### 7.1 Relativistic conventions` | 302 / `#71-relativistic-conventions` | converted | Two display equations inside list item |
| 25 | subsection | Units and nondimensionalization | 387 | `### 7.2 Units and nondimensionalization` | 328 / `#72-units-and-nondimensionalization` | converted | — |
| 26 | subsection | Initial-value formulation | 402 | `### 7.3 Initial-value formulation` | 340 / `#73-initial-value-formulation` | converted | — |
| 27 | section | Theory-First Development Doctrine | 417 | `## 8. Theory-First Development Doctrine` | 351 / `#8-theory-first-development-doctrine` | converted | — |
| 28 | subsection | Theory-readiness gate | 443 | `### 8.1 Theory-readiness gate` | 372 / `#81-theory-readiness-gate` | converted | — |
| 29 | section | Physics-to-Software Contract | 460 | `## 9. Physics-to-Software Contract` | 387 / `#9-physics-to-software-contract` | converted | — |
| 30 | section | Numerical Doctrine | 483 | `## 10. Numerical Doctrine` | 406 / `#10-numerical-doctrine` | converted | — |
| 31 | subsection | Model-appropriate integration | 485 | `### 10.1 Model-appropriate integration` | 408 / `#101-model-appropriate-integration` | converted | LaTeX quotes → typographic quotes |
| 32 | subsection | Error observables | 498 | `### 10.2 Error observables` | 416 / `#102-error-observables` | converted | `align` → `aligned` in `$$`; see Section 7 |
| 33 | subsection | No universal tolerance | 524 | `### 10.3 No universal tolerance` | 441 / `#103-no-universal-tolerance` | converted | — |
| 34 | subsection | Singularities and coordinate boundaries | 531 | `### 10.4 Singularities and coordinate boundaries` | 445 / `#104-singularities-and-coordinate-boundaries` | converted | — |
| 35 | section | Validation and Evidence Doctrine | 545 | `## 11. Validation and Evidence Doctrine` | 456 / `#11-validation-and-evidence-doctrine` | converted | — |
| 36 | subsection | Evidence hierarchy | 547 | `### 11.1 Evidence hierarchy` | 458 / `#111-evidence-hierarchy` | converted | E0–E5 description list → bold-label list |
| 37 | subsection | Required validation layers | 573 | `### 11.2 Required validation layers` | 471 / `#112-required-validation-layers` | converted | — |
| 38 | subsection | Classification validation | 586 | `### 11.3 Classification validation` | 482 / `#113-classification-validation` | converted | — |
| 39 | section | Product Architecture | 598 | `## 12. Product Architecture` | 492 / `#12-product-architecture` | converted | — |
| 40 | subsection | Comprehensive technical monograph | 600 | `### 12.1 Comprehensive technical monograph` | 494 / `#121-comprehensive-technical-monograph` | converted | Part I–VI labels preserved literally |
| 41 | subsection | Python repository | 620 | `### 12.2 Python repository` | 509 / `#122-python-repository` | converted | `\texttt` → code span |
| 42 | subsection | Preprint-style paper | 630 | `### 12.3 Preprint-style paper` | 515 / `#123-preprint-style-paper` | converted | `\textit` title → italic in blockquote |
| 43 | subsection | Public datasets and figures | 647 | `### 12.4 Public datasets and figures` | 525 / `#124-public-datasets-and-figures` | converted | — |
| 44 | section | Writing and Communication Standard | 663 | `## 13. Writing and Communication Standard` | 538 / `#13-writing-and-communication-standard` | converted | — |
| 45 | section | Publication and Novelty Doctrine | 684 | `## 14. Publication and Novelty Doctrine` | 554 / `#14-publication-and-novelty-doctrine` | converted | — |
| 46 | section | Project Phases and Hard Dependencies | 705 | `## 15. Project Phases and Hard Dependencies` | 568 / `#15-project-phases-and-hard-dependencies` | converted | `longtable` → Markdown table, 11 phase rows |
| 47 | section | Collaboration Boundary for Phase 0 | 751 | `## 16. Collaboration Boundary for Phase 0` | 594 / `#16-collaboration-boundary-for-phase-0` | converted | — |
| 48 | section | Risk and Feasibility Control | 774 | `## 17. Risk and Feasibility Control` | 609 / `#17-risk-and-feasibility-control` | converted | — |
| 49 | subsection | Scope inflation | 776 | `### 17.1 Scope inflation` | 611 / `#171-scope-inflation` | converted | — |
| 50 | subsection | Theory without completion | 790 | `### 17.2 Theory without completion` | 621 / `#172-theory-without-completion` | converted | — |
| 51 | subsection | Code without scientific authority | 797 | `### 17.3 Code without scientific authority` | 625 / `#173-code-without-scientific-authority` | converted | — |
| 52 | subsection | Visual-first bias | 802 | `### 17.4 Visual-first bias` | 629 / `#174-visual-first-bias` | converted | — |
| 53 | subsection | Unfounded publication expectations | 808 | `### 17.5 Unfounded publication expectations` | 633 / `#175-unfounded-publication-expectations` | converted | — |
| 54 | section | Definition of Full Project Completion | 814 | `## 18. Definition of Full Project Completion` | 637 / `#18-definition-of-full-project-completion` | converted | — |
| 55 | section | Phase 0 Decision Register | 837 | `## 19. Phase 0 Decision Register` | 658 / `#19-phase-0-decision-register` | converted | `longtable` → Markdown table, 17 frozen rows |
| 56 | section | Immediate Next Authorized Work | 872 | `## 20. Immediate Next Authorized Work` | 682 / `#20-immediate-next-authorized-work` | converted | — |
| 57 | — | (not in source) | — | Section 20 operational amendment note (blockquote) | 699 | added | Phase 1 boundary clarification; authorized non-mechanical addition (Section 9); placed after the preserved source-derived closing sentence of Section 20 |
| 58 | section* | Approval Status (`\section*` + `\addcontentsline`) | 893–894 | `## Approval Status` | 701 / `#approval-status` | converted | Original wording preserved; marked amendment note appended at output line 707 (Section 9) |
| 59 | environment | signature block (`center`, `\rule`, `\vfill`) | 902–908 | two-column signature table | 709–711 | restructured | Names and roles preserved; ruled lines omitted as typesetting |

Heading totals: source 20 `\section` + 32 `\subsection` + 1 `\section*` = 53 headings; output 1 H1 + 24 H2 + 32 H3 = 57 headings. The four additional output headings are the title H1 rendering of `\maketitle` and the H2 headings `Canonical-Format Amendment Note` (added), `Abstract` (rendering of the `abstract` environment), and `Contents` (rendering of `\tableofcontents`). No source heading was dropped, merged, split, or reordered.

## 5. Historical Decision-Register Preservation

All 17 expected identifiers `D0-01` through `D0-17` were verified present in the source, each exactly once, and the supplied expected family matched the source exactly — no discrepancy. Comparison below is a preliminary Claude-assisted textual comparison; human comparison remains PENDING.

| ID | Source occurrence (line) | Output occurrence (line) | Order preserved | Identifier preserved | Substantive wording preservation (preliminary) | Review state |
| --- | --- | --- | --- | --- | --- | --- |
| D0-01 | 850 | 664 | yes | yes | verbatim | human review PENDING |
| D0-02 | 851 | 665 | yes | yes | verbatim | human review PENDING |
| D0-03 | 852 | 666 | yes | yes | verbatim | human review PENDING |
| D0-04 | 853 | 667 | yes | yes | verbatim, `$N$` math preserved | human review PENDING |
| D0-05 | 854 | 668 | yes | yes | verbatim | human review PENDING |
| D0-06 | 855 | 669 | yes | yes | verbatim | human review PENDING |
| D0-07 | 856 | 670 | yes | yes | verbatim | human review PENDING |
| D0-08 | 857 | 671 | yes | yes | verbatim | human review PENDING |
| D0-09 | 858–859 | 672 | yes | yes | verbatim; two-line source cell joined | human review PENDING |
| D0-10 | 860 | 673 | yes | yes | verbatim | human review PENDING |
| D0-11 | 861 | 674 | yes | yes | verbatim | human review PENDING |
| D0-12 | 862 | 675 | yes | yes | verbatim | human review PENDING |
| D0-13 | 863 | 676 | yes | yes | verbatim; `18--22` → `18–22` (typography only) | human review PENDING |
| D0-14 | 864 | 677 | yes | yes | verbatim | human review PENDING |
| D0-15 | 865–866 | 678 | yes | yes | verbatim; two-line source cell joined | human review PENDING |
| D0-16 | 867 | 679 | yes | yes | verbatim | human review PENDING |
| D0-17 | 868 | 680 | yes | yes | verbatim | human review PENDING |

No identifier was renumbered, combined, split, or reworded. No settled-state correction was made inside any register entry. The `RDR-0001` amendment note is outside the register.

## 6. Macro Expansion Inventory

Substantive custom macros (affect rendered content):

| Macro | Source definition | Rendered-content usage count | Markdown expansion | Fidelity note |
| --- | --- | --- | --- | --- |
| `\ProjectTitle` | `From Newton to Kerr` (source line 30) | 4 (lines 39, 51, 69, 92) | literal text `From Newton to Kerr` | exact expansion, plain text as rendered |
| `\ProjectSubtitle` | `Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics` (line 31) | 2 (lines 40, 94) | literal subtitle text | exact expansion |
| `\E` | `\mathcal{E}` (line 35) | 1 (line 329) | `\mathcal{E}` in inline math | exact expansion |
| `\Lz` | `L_z` (line 36) | 1 (line 329) | `L_z` in inline math | exact expansion |

Defined but unused in rendered content (definition-only; nothing to expand, omitted with the preamble):

| Macro | Source definition | Rendered-content usage count |
| --- | --- | --- |
| `\R` | `\mathbb{R}` (line 32) | 0 |
| `\dd` | `\mathrm{d}` (line 33) | 0 |
| `\Order` | `\mathcal{O}` (line 34) | 0 |
| `\Msun` | `M_{\odot}` (line 37) | 0 |

No macro expansion altered mathematical meaning or notation.

## 7. Mathematical and Equation Audit

| Measure | Source | Output |
| --- | --- | --- |
| Inline-math instances (`$...$`) | 15 | 15 |
| Display-math environments | 4 (3 `equation`, 1 `align` with 3 lines) | 4 `$$` blocks (one containing `aligned` with 3 lines) |
| Numbered display lines (LaTeX auto-numbering) | 6 — implicit numbers (1)–(6) | not rendered (see limitation below) |

Equation mapping (no source equation carries a `\label`; none is referenced anywhere in the source):

| Source equation | Source locator | Output locator | Conversion |
| --- | --- | --- | --- |
| Thesis chain (`\text{physical model} \longrightarrow … \text{orbit classification}`) | 151–163 | 156–168 | `equation` → `$$` block; content byte-faithful |
| `a=\frac{J}{Mc}` | 376–378 | 315–317 | `equation` → indented `$$` block inside list item |
| `\chi=\frac{cJ}{GM^2}=\frac{ac^2}{GM}, \qquad \|\chi\|\leq 1` | 380–383 | 321–324 | `equation` → indented `$$` block inside list item; `\qquad` and `\leq` preserved |
| `\Delta E`, `\Delta L`, `\Delta C` block | 502–506 | 420–426 | `align` → `aligned` inside `$$` (delimiter/environment change; alignment `&` and `\\` preserved) |

Inline-math one-to-one mapping (source line → output line, recomputed from the current output): `$N$` 56→37, 268→233, 343→286, 782→615, 853→667; `$v/c$` 279→240; `$GM/(rc^2)$` 279→240; `$(\E,\Lz,Q)$` 329→275 (expanded to `$(\mathcal{E},L_z,Q)$`); `$(-,+,+,+)$` 366→306; `$G$` and `$c$` 367→307; `$\tau$` 371→310; `$\lambda$` 372→311; `$G=c=M=1$` 400→338; `$C$` 508→428.

No sign, symbol, index placement, unit, convention name, or dimensional assumption was changed. No natural units were introduced. No equation was simplified.

Equation-rendering review state: preliminary automated conversion only; **human equation review PENDING**.

Known rendering limitations:

1. LaTeX auto-numbers (1)–(6) on the six display lines are not rendered by GitHub math. No cross-reference in the source depends on any equation number, so no reference breaks; the mapping above is the permanent numbering record.
2. The `align` environment was converted to `aligned` inside `$$` because GitHub does not reliably render top-level `align`; alignment structure and content are otherwise identical.
3. The two display equations nested inside a Markdown list item (Section 7.1 of the output) depend on GitHub's rendering of indented `$$` blocks within lists; the math source itself is faithful. Rendered appearance requires human inspection.

## 8. Tables, Lists, Quotations, Code, Footnotes, Citations, and Links

| Category | Source count | Output count | Disposition |
| --- | --- | --- | --- |
| Tables | 2 (`longtable`: Phases 11 rows; Decision Register 17 rows) | 4 Markdown tables | Both source tables converted row-for-row. Two authorized additions: document metadata table and signature-block table (Section 9) |
| Unordered lists (`itemize`) | 21 | 22 | All 21 converted; +1 in added Canonical-Format Amendment Note |
| Ordered lists (`enumerate`) | 8 | 6 ordered + 2 literal-label lists | Enumerates with `1.`-style labels → Markdown ordered lists; `(a)/(b)` (M6) and `Part I–VI` (12.1) rendered with their literal labels to preserve appearance |
| Description lists (`description`) | 3 (RQ1–RQ5; H1–H4; E0–E5) | 3 bold-label lists | Bold labels reproduce LaTeX description-item typography |
| Quotations (`quote`) | 4 | 6 blockquotes | All 4 converted (positioning statement, central thesis, provisional title, Phase 1); +2 authorized amendment blockquotes: the Section 20 operational amendment note and the marked amendment note in Approval Status (Section 9) |
| Code / verbatim environments | None present (verified from complete source) | 0 | — |
| Inline code (`\texttt`) | 1 (`pyproject.toml`) | 1 code span | Plus authorized code-formatted references in metadata, amendment note, and this audit's cross-references |
| Footnotes | None present (verified from complete source) | 0 | — |
| Citations / bibliography | None present (verified from complete source) | 0 | — |
| URLs / external links | None present (verified from complete source) | 0 external | Output adds internal ToC anchor links only (55, all resolving in-file) |

## 9. Non-Mechanical Changes

Complete list. Every change below is authorized by `RDR-0001` (ratified 17 July 2026); no other non-mechanical change exists.

1. **Document metadata table** (output lines 5–20). Replaces the LaTeX `\date{Version 0.1.0 --- Phase 0 Foundational Draft\\16 July 2026}` title-block rendering. Source wording preserved in rows `Source version | 0.1.0`, `Source date | 16 July 2026`, `Declared source-state wording | `Phase 0 Foundational Draft``; settled-state rows added: `Substantive governance state | RATIFIED`, `Transposition state | AUTHORIZED DRAFT`, `Canonical authority | NOT YET EFFECTIVE`, `Related repository decision | `RDR-0001` — RATIFIED`, plus source identity and role rows. Reason: settled-state metadata correction and provenance binding. Authority: `RDR-0001` Section 1 (settled-state metadata transposition) and Section 3.3; provenance record Section 6 (permitted transformation: "settled-state metadata and tense corrections").
2. **Canonical-Format Amendment Note** (output lines 22–33). Entirely new marked section; no source counterpart. Reason: mandated authority clarification outside the frozen register. Authority: `RDR-0001` Section 3.4 ("The converted documents may add a clearly marked amendment note, placed outside the frozen historical register, pointing to `RDR-0001`").
3. **Qualified transposition-purpose wording** (output line 27, second amendment-note bullet). The earlier draft of this bullet asserted that the file "is a faithful Markdown transposition"; this prematurely asserted established fidelity. Corrected wording: "This file is an authorized Markdown transposition prepared to preserve the complete rendered substantive content of the ratified LaTeX source `00_Scientific_Constitution_From_Newton_to_Kerr.tex` under the ratified repository decision `RDR-0001`. Its semantic fidelity remains subject to the required human comparison, independent collaborator review, and final scientific sign-off." Reason: the transposition objective is unchanged, but fidelity is not finally established until the pending human review chain completes. Authority: `RDR-0001` Section 6 adoption conditions; correction instructed under bounded task P00B.3C-1 reconciliation.
4. **Top amendment-note Phase 1 clarification** (output line 32, penultimate amendment-note bullet). Added bullet stating that the historical authorization language in Section 20 and Approval Status is preserved verbatim but does not activate Phase 1 under the current repository-governance sequence; Phase 1 remains blocked until Gate 0B is fully completed, its closeout is ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1; production Python work remains blocked. Reason: prevents the preserved historical wording from being read as a current operational authorization. Authority: `RDR-0001` Sections 1 and 3.4; NTK-MASTER ruling of 17 July 2026 (Phase 1 BLOCKED; production Python BLOCKED).
5. **Section 20 operational amendment note** (output line 699, blockquote). Added immediately after the preserved source-derived sentence "No production solver implementation is authorized by this Phase 0 document." Every source-derived sentence and list item in Section 20 is preserved exactly; the note is visibly separate as a marked blockquote. Wording: "**Operational amendment (`RDR-0001`; NTK-MASTER, 17 July 2026):** The Phase 1 authorization language above is preserved as part of the historical ratified source. Under the current repository-governance sequence, Phase 1 remains blocked until Gate 0B is fully completed, its closeout is ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1. Production Python architecture and implementation remain blocked." Authority: `RDR-0001` Sections 1 and 3.4; NTK-MASTER ruling of 17 July 2026.
6. **Revised Approval Status amendment note** (output line 707, blockquote). The source statements "**Current status:** Foundational draft for scientific-owner review." and "**Approval effect:** …" (source lines 896–900) remain preserved **verbatim and unrewritten**. The appended marked note was revised from its earlier draft to add the NTK-MASTER attribution and date, state that the substantive Constitution was subsequently ratified, and state explicitly that the historical Phase 1 authorization wording does not activate Phase 1 under the current repository-governance sequence (Phase 1 blocked until Gate 0B closes, closeout ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1). Reason: the source statement is historically accurate but no longer the current operational state; it is annotated rather than rewritten. Authority: `RDR-0001` Sections 1, 3.4.
7. **Table of contents** (output lines 39–95). Source `\tableofcontents` (line 64) regenerated as explicit Markdown anchor links covering the full resulting heading structure. Reason: LaTeX ToC machinery does not exist in Markdown. Authority: `RDR-0001` Section 3.5 (Markdown governance checks presuppose internal navigation); mechanical equivalent of the source command.
8. **Explicit section numbering in headings** (`1.`–`20.`, `2.1`, etc.). LaTeX auto-numbering reproduced literally because Markdown has no counter machinery. Preserves the source's rendered numbering exactly; no renumbering.
9. **Signature-block table** (output lines 709–711). The `center`/`\rule` two-column signature layout rendered as a two-column table with names and roles preserved; ruled signature lines omitted as typography. Authority: mechanical layout conversion under `RDR-0001` Section 1 (format-only transposition).
10. **Removal of audit self-reference from the drafting-marker scan** (this audit, Section 11). The earlier draft of the Section 11 scan row spelled out the literal unresolved-draft marker terms, which made this audit fail its own scan. The row now describes the marker set without reproducing the literal terms, and the Section 13 scope sentence was reworded for the same reason. This change is internal to the audit record and touches no Constitution content.

No anchor was created via HTML; all navigation uses GitHub's automatic heading anchors. No wording of any substantive scientific or governance statement was changed, and semantic fidelity is not claimed to be established by any change above.

## 10. Intentionally Omitted LaTeX-Only Material

Non-semantic source material omitted from the Markdown output (none of it is rendered governance substance):

- `\documentclass[11pt]{article}` (line 1);
- package imports: `inputenc`, `fontenc`, `lmodern`, `babel`, `microtype`, `geometry`, `setspace`, `amsmath`, `amssymb`, `mathtools`, `booktabs`, `longtable`, `tabularx`, `array`, `enumitem`, `xcolor`, `hyperref` (lines 3–14);
- layout commands: `\geometry{...}`, `\setstretch`, `\parindent`, `\parskip`, `\setcounter{tocdepth}` (lines 16–20);
- `\hypersetup{...}` including PDF-only `pdftitle`/`pdfauthor` metadata (lines 21–28; note the PDF metadata spells the names without accents — a PDF-string constraint, not rendered content);
- unused macro definitions `\R`, `\dd`, `\Order`, `\Msun` (Section 6 above) and the definitions (as opposed to expansions) of the used macros (lines 30–37);
- title-page machinery: `\title`, `\author`, `\date` commands themselves and `\maketitle` (lines 39–46; their rendered content is preserved);
- `\newpage` (line 65), `\vfill` (line 902), `\rule` signature lines (line 905), `\addcontentsline` (line 894);
- LaTeX table column specifications (`p{...}`, `\toprule`/`\midrule`/`\bottomrule`, `\endfirsthead`/`\endhead`) and list-option keys (`[label=...]`, `[leftmargin=...]`, `style=nextline`);
- source comments: none exist in the source (verified: zero `%`-comment lines).

No substantive content appears in this list.

## 11. Automated and Tool-Assisted Checks

Every check below was actually executed on 17 July 2026 in this task.

| Check | Method | Result |
| --- | --- | --- |
| Source SHA-256 | `sha256sum` before conversion and again after outputs written | `6ac268e9…bc46` — exact match both times |
| Source byte / newline / CR counts | `wc -c`, `wc -l`, `tr`-based CR count | 38899 / 910 / 0 — exact match |
| Source leading bytes | `head -c 3 \| xxd` | `5c646f` — exact match |
| Source ignored state | `git check-ignore -v` | ignored by `.gitignore:10` rule `.ntk-local-inputs/` |
| Source untracked state | `git ls-files` | empty output — untracked |
| Output existence | `wc`, `sha256sum` | present at authorized path |
| Output UTF-8 decoding | Python strict `bytes.decode('utf-8')` | valid UTF-8 |
| LF-only line endings | CR-byte count via `tr` | 0 CR bytes |
| Final newline | `tail -c 1 \| xxd` | `0x0a` |
| Control-byte scan | `tr` scan for bytes 0x00–0x08, 0x0B, 0x0C, 0x0E–0x1F, 0x7F | 0 forbidden control bytes |
| Trailing-whitespace scan | `grep -E ' +$'` | 0 lines |
| Heading inventory | `grep '^#'` vs source `\section`/`\subsection` list | 53 source headings all present, order preserved; +4 accounted additions (Section 4) |
| Decision-ID inventory | `grep -o 'D0-[0-9][0-9]'` on source and output | 17/17 in source (each once); output register rows D0-01…D0-17 in order (plus the two authorized mentions in the amendment note) |
| Unresolved-LaTeX scan | fixed-string backslash line listing over full output | every backslash line is inside inline or display math; 0 document-level LaTeX commands remain |
| Accent-command scan | grep for `\'`, `\"` forms | 0 remaining; all converted to Unicode (Pérez, Sánchez, Störmer, Poincaré) |
| Common unresolved drafting-marker scan | case-insensitive scan of both outputs using the task's fixed marker set | 0 actionable occurrences after removal of audit self-reference |
| Fused-token scan | regex for period+uppercase and letter,letter fusions | only match is the faithful math tuple `$(\mathcal{E},L_z,Q)$`; 0 prose fusions |
| Internal-link check | Python: GitHub-style anchor generation vs all `](#…)` links | 55/55 links resolve; 0 duplicate anchors |
| Inline-math count | `grep -o '\$[^$]*\$'` with `$$` filtered | source 15, output 15 |
| Display-math count | delimiter-line count | source 4 environments; output 4 `$$` blocks (8 delimiter lines) |
| Category counts | environment greps on source; structure greps on output | as recorded in Section 8 |
| Forbidden-path check | `find governance -type f`; explicit `ls` | document `01` output and any other new path absent |
| Git scope check | `git status --porcelain` | only the two authorized files untracked; no tracked file modified |
| Tracked-record integrity | `sha256sum` of RDR-0001 and provenance record | `39eb0801…f2ab` and `8cdb9a67…f7f8` — unchanged |

## 12. Known Limitations and Nonclaims

- Automated checks prove structural and byte-level traceability only; they do **not** prove semantic fidelity.
- Claude Code self-review does **not** constitute independent review.
- Output hashes prove identity of the output bytes, not correctness of the transposition.
- Rendered GitHub mathematics (including `$$` blocks inside list items and math inside table cells) still requires human visual inspection.
- Human source-to-output comparison remains **PENDING**.
- Naomi Sánchez Torres's independent review remains **PENDING**.
- Edgar Axel Pérez Flores's final scientific sign-off remains **PENDING**.
- Protected-`main` adoption remains **PENDING**; the canonical transition is not yet effective.
- No scientific validation of any kind is claimed by this audit or by the transposition.

## 13. Document 01 Status

- The source identity of `01_Project_Governance_and_Repository_Charter.tex` already exists in `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md` (SHA-256 `fb74ae936a6dba21efe4aab1d6b6f099d57dbeded6ca56c55cff0ce6c33af3f4`).
- Its transposition was **not performed** in this task.
- The output path `governance/01_Project_Governance_and_Repository_Charter.md` is **absent**.
- Its structural mapping is pending.
- Its equation and identifier audits (including the `D0B-*` register family) are pending.
- **No conclusion about document `01` fidelity is made here.** This is a truthful scope statement and does not assert any conclusion about document `01` fidelity.

## 14. Human Review and Adoption Record

| Step | State |
| --- | --- |
| Claude Code bounded drafting and preliminary self-audit (document 00) | completed |
| Edgar document-00 comparison | pending |
| Naomi document-00 review | pending |
| Document-01 transposition | pending |
| Edgar comparison of both transpositions | pending |
| Naomi independent review of both transpositions | pending |
| Required checks | pending |
| Final scientific sign-off | pending |
| Foundation PR | pending |
| Protected-main merge | pending |
| Merge commit | pending |
| Foundation tag | pending |

Claude Code has **no scientific, authorship, ratification, independent-review, final-sign-off, or Git authority**. Its role in this task is limited to bounded transposition drafting and preliminary automated self-audit. All comparison, review, sign-off, ratification, and Git operations are performed exclusively by the authorized human parties; NTK-MASTER is the sole ratification authority, and Edgar Axel Pérez Flores alone performs all Git staging, commits, and pushes.

## 15. Current State

- Document `00` transposition created as an **authorized draft** at `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md`.
- Document `00` preliminary traceability audit **completed** (this record).
- Human semantic comparison **pending**.
- Document `01` **not yet transposed**.
- Canonical transition **not yet effective**.
- Phase 1 **blocked**.
- Production Python **blocked**.
- Next step: independent human inspection of document `00` and of this audit before any commit.
