# RDR-0001 Transposition Audit

| Field | Value |
| --- | --- |
| Record status | DRAFT |
| Record date | 17 July 2026 |
| Governing workstream | `[NTK-P00B]` Repository and Collaboration Foundation |
| Related decision | `RDR-0001` — RATIFIED |
| Canonical transition | AUTHORIZED — NOT YET EFFECTIVE |
| Audit coverage | Documents 00 and 01 transposed; human comparison and adoption pending |
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

Document `01` source identity, independently reverified before conversion on 17 July 2026:

| Attribute | Value |
| --- | --- |
| Document | Project Governance and Repository Charter |
| Source path | `.ntk-local-inputs/01_Project_Governance_and_Repository_Charter.tex` |
| Source filename | `01_Project_Governance_and_Repository_Charter.tex` |
| Declared source version | `0.1.0` |
| Declared source date | 16 July 2026 |
| Declared source-state wording | `Gate 0B Foundational Draft` |
| Classification | LaTeX 2e document, ASCII text |
| MIME and charset | `text/x-tex; charset=us-ascii` |
| Exact bytes | `43382` |
| Newline count from `wc -l` | `1068` |
| CR byte count | `0` |
| First three bytes, hexadecimal | `5c646f` |
| SHA-256 | `fb74ae936a6dba21efe4aab1d6b6f099d57dbeded6ca56c55cff0ce6c33af3f4` |
| Git state | ignored (`.gitignore` rule `.ntk-local-inputs/`) and untracked |

All document `01` values above agree exactly with `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md` and with the identities independently accepted by the NTK-MASTER ratification of `RDR-0001`. Both original LaTeX sources remain ignored, untracked, byte-unchanged, and retained privately under the durable-retention rule of that provenance record.

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

Document `01` output:

| Attribute | Value |
| --- | --- |
| Output path | `governance/01_Project_Governance_and_Repository_Charter.md` |
| Exact bytes | `52545` |
| Newline count from `wc -l` | `942` |
| Encoding | UTF-8 (validated by strict decode) |
| Line-ending state | LF-only; CR byte count `0`; final byte `0x0a` |
| SHA-256 | `3de90bc18014fa33e9d4574b105c2fa761b6d50115b6209e36f3d271ce425ff1` |
| Creation state | AUTHORIZED DRAFT — NOT YET CANONICAL |

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

Document `01` mapping (source: `01_Project_Governance_and_Repository_Charter.tex`; output: `governance/01_Project_Governance_and_Repository_Charter.md`):

| # | Source level | Source heading or element | Source locator | Markdown heading or element | Output locator / anchor | Disposition | Notes |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | title block | `\title`, `\author`, `\date`, `\maketitle` | 37–44 | `#` title, subtitle line, metadata table | 1–25 | restructured | Version/date/state moved into metadata table; see Section 9 |
| 2 | — | (not in source) | — | `## Canonical-Format and Operational-State Amendment Note` | 27 / `#canonical-format-and-operational-state-amendment-note` | added | Authorized by `RDR-0001` §3.4 |
| 3 | environment | `abstract` | 46–59 | `## Abstract` | 47 / `#abstract` | converted | Verbatim prose; macros expanded |
| 4 | command | `\tableofcontents` | 61 | `## Contents` | 51 / `#contents` | converted | Rebuilt as Markdown anchor links |
| 5 | section | Purpose and Authority | 64 | `## 1. Purpose and Authority` | 125 / `#1-purpose-and-authority` | converted | Explicit numbering reproduces LaTeX auto-numbering |
| 6 | section | Relationship to the Scientific Constitution | 85 | `## 2. Relationship to the Scientific Constitution` | 139 / `#2-relationship-to-the-scientific-constitution` | converted | — |
| 7 | subsection | Authority hierarchy | 87 | `### 2.1 Authority hierarchy` | 141 / `#21-authority-hierarchy` | converted | — |
| 8 | subsection | Repository as documentary source of truth | 103 | `### 2.2 Repository as documentary source of truth` | 154 / `#22-repository-as-documentary-source-of-truth` | converted | — |
| 9 | subsection | Amendment boundary | 114 | `### 2.3 Amendment boundary` | 160 / `#23-amendment-boundary` | converted | — |
| 10 | section | Project and Repository Identity | 120 | `## 3. Project and Repository Identity` | 164 / `#3-project-and-repository-identity` | converted | Description list → bold-label lines |
| 11 | section | Public-From-Day-One Doctrine | 137 | `## 4. Public-From-Day-One Doctrine` | 186 / `#4-public-from-day-one-doctrine` | converted | — |
| 12 | subsection | Meaning of public development | 139 | `### 4.1 Meaning of public development` | 188 / `#41-meaning-of-public-development` | converted | LaTeX quotes → typographic quotes |
| 13 | subsection | Required public status declaration | 166 | `### 4.2 Required public status declaration` | 209 / `#42-required-public-status-declaration` | converted | `quote` → blockquote |
| 14 | section | Governance Principles | 179 | `## 5. Governance Principles` | 217 / `#5-governance-principles` | converted | `G\arabic` labels preserved literally as G1–G10 |
| 15 | section | Human Roles and Responsibilities | 198 | `## 6. Human Roles and Responsibilities` | 232 / `#6-human-roles-and-responsibilities` | converted | — |
| 16 | subsection | Edgar Axel Pérez Flores: Scientific Lead and Repository Owner | 200 | `### 6.1 Edgar Axel Pérez Flores: Scientific Lead and Repository Owner` | 234 / `#61-edgar-axel-pérez-flores-scientific-lead-and-repository-owner` | converted | Accents → Unicode |
| 17 | subsection | Naomi Sánchez Torres: Scientific Collaborator and Co-developer | 218 | `### 6.2 Naomi Sánchez Torres: Scientific Collaborator and Co-developer` | 248 / `#62-naomi-sánchez-torres-scientific-collaborator-and-co-developer` | converted | Accents → Unicode |
| 18 | subsection | Shared responsibilities | 236 | `### 6.3 Shared responsibilities` | 261 / `#63-shared-responsibilities` | converted | — |
| 19 | subsection | No shared credentials | 251 | `### 6.4 No shared credentials` | 274 / `#64-no-shared-credentials` | converted | — |
| 20 | section | Decision Authority Matrix | 257 | `## 7. Decision Authority Matrix` | 278 / `#7-decision-authority-matrix` | converted | `longtable` → Markdown table, 10 rows × 4 columns |
| 21 | section | Classes of Change and Review Requirements | 296 | `## 8. Classes of Change and Review Requirements` | 295 / `#8-classes-of-change-and-review-requirements` | converted | — |
| 22 | subsection | Class A: Constitutional and scientific-authority changes | 300 | `### 8.1 Class A: Constitutional and scientific-authority changes` | 299 / `#81-class-a-constitutional-and-scientific-authority-changes` | converted | — |
| 23 | subsection | Class B: Scientific implementation and evidence changes | 324 | `### 8.2 Class B: Scientific implementation and evidence changes` | 319 / `#82-class-b-scientific-implementation-and-evidence-changes` | converted | — |
| 24 | subsection | Class C: Administrative and low-risk changes | 339 | `### 8.3 Class C: Administrative and low-risk changes` | 331 / `#83-class-c-administrative-and-low-risk-changes` | converted | — |
| 25 | section | Repository Access and Protection | 353 | `## 9. Repository Access and Protection` | 342 / `#9-repository-access-and-protection` | converted | — |
| 26 | subsection | Account roles | 355 | `### 9.1 Account roles` | 344 / `#91-account-roles` | converted | — |
| 27 | subsection | Protection of the default branch | 361 | `### 9.2 Protection of the default branch` | 348 / `#92-protection-of-the-default-branch` | converted | — |
| 28 | section | Git Workflow | 380 | `## 10. Git Workflow` | 363 / `#10-git-workflow` | converted | — |
| 29 | subsection | Branch doctrine | 382 | `### 10.1 Branch doctrine` | 365 / `#101-branch-doctrine` | converted | Description list → bold code-label list; `verbatim` → fenced `text` block |
| 30 | subsection | Commit doctrine | 410 | `### 10.2 Commit doctrine` | 391 / `#102-commit-doctrine` | converted | `verbatim` → fenced `text` block |
| 31 | subsection | Merge strategy | 429 | `### 10.3 Merge strategy` | 409 / `#103-merge-strategy` | converted | — |
| 32 | section | Pull-Request Standard | 438 | `## 11. Pull-Request Standard` | 415 / `#11-pull-request-standard` | converted | — |
| 33 | section | Issues, Milestones, and Project Tracking | 459 | `## 12. Issues, Milestones, and Project Tracking` | 432 / `#12-issues-milestones-and-project-tracking` | converted | — |
| 34 | subsection | Issues | 461 | `### 12.1 Issues` | 434 / `#121-issues` | converted | — |
| 35 | subsection | Milestones | 478 | `### 12.2 Milestones` | 448 / `#122-milestones` | converted | — |
| 36 | subsection | Project board | 483 | `### 12.3 Project board` | 452 / `#123-project-board` | converted | `verbatim` → fenced `text` block |
| 37 | section | Decision Records | 494 | `## 13. Decision Records` | 462 / `#13-decision-records` | converted | — |
| 38 | subsection | Record types | 496 | `### 13.1 Record types` | 464 / `#131-record-types` | converted | Description list → bold-label list |
| 39 | subsection | Required fields | 507 | `### 13.2 Required fields` | 471 / `#132-required-fields` | converted | — |
| 40 | section | Master Orchestration and Specialized Work Sessions | 527 | `## 14. Master Orchestration and Specialized Work Sessions` | 488 / `#14-master-orchestration-and-specialized-work-sessions` | converted | — |
| 41 | subsection | Master orchestration | 529 | `### 14.1 Master orchestration` | 490 / `#141-master-orchestration` | converted | — |
| 42 | subsection | Specialized sessions | 536 | `### 14.2 Specialized sessions` | 494 / `#142-specialized-sessions` | converted | — |
| 43 | section | Use of Artificial-Intelligence Tools | 567 | `## 15. Use of Artificial-Intelligence Tools` | 519 / `#15-use-of-artificial-intelligence-tools` | converted | — |
| 44 | subsection | Permitted role | 569 | `### 15.1 Permitted role` | 521 / `#151-permitted-role` | converted | — |
| 45 | subsection | Human accountability | 583 | `### 15.2 Human accountability` | 533 / `#152-human-accountability` | converted | — |
| 46 | subsection | Disclosure | 601 | `### 15.3 Disclosure` | 546 / `#153-disclosure` | converted | — |
| 47 | section | Authorship, Attribution, and Contribution Records | 608 | `## 16. Authorship, Attribution, and Contribution Records` | 550 / `#16-authorship-attribution-and-contribution-records` | converted | — |
| 48 | subsection | Repository attribution | 610 | `### 16.1 Repository attribution` | 552 / `#161-repository-attribution` | converted | — |
| 49 | subsection | Publication authorship | 618 | `### 16.2 Publication authorship` | 558 / `#162-publication-authorship` | converted | — |
| 50 | subsection | External contributors | 638 | `### 16.3 External contributors` | 574 / `#163-external-contributors` | converted | — |
| 51 | section | Licensing Doctrine | 643 | `## 17. Licensing Doctrine` | 578 / `#17-licensing-doctrine` | converted | Description list → bold-label list |
| 52 | section | Initial Repository Architecture | 663 | `## 18. Initial Repository Architecture` | 590 / `#18-initial-repository-architecture` | converted | Two `verbatim` blocks → fenced `text` blocks; tree preserved byte-faithfully |
| 53 | — | (not in source) | — | §18 architecture operational amendment (blockquote) | 651–668 | added | Identifies the repository paths authorized for eventual canonical adoption per `RDR-0001`, not paths already canonical; see Section 9 |
| 54 | section | Monograph and LaTeX Governance | 726 | `## 19. Monograph and LaTeX Governance` | 670 / `#19-monograph-and-latex-governance` | converted | — |
| 55 | subsection | Authoritative source | 728 | `### 19.1 Authoritative source` | 672 / `#191-authoritative-source` | converted | — |
| 56 | subsection | Build doctrine | 734 | `### 19.2 Build doctrine` | 676 / `#192-build-doctrine` | converted | Historical wording preserved |
| 57 | — | (not in source) | — | §19.2 build-doctrine operational amendment (blockquote) | 682–697 | added | Monograph-scaffold build scope, implementation-time Markdown checks, post-adoption canonical authority, and Overleaf boundary; see Section 9 |
| 58 | subsection | Writing standard | 745 | `### 19.3 Writing standard` | 699 / `#193-writing-standard` | converted | — |
| 59 | section | Citation and Source Governance | 752 | `## 20. Citation and Source Governance` | 703 / `#20-citation-and-source-governance` | converted | — |
| 60 | section | Data, Figures, and Reproducibility | 774 | `## 21. Data, Figures, and Reproducibility` | 719 / `#21-data-figures-and-reproducibility` | converted | — |
| 61 | subsection | Generated evidence | 776 | `### 21.1 Generated evidence` | 721 / `#211-generated-evidence` | converted | — |
| 62 | subsection | Repository size discipline | 791 | `### 21.2 Repository size discipline` | 734 / `#212-repository-size-discipline` | converted | — |
| 63 | subsection | Failure preservation | 797 | `### 21.3 Failure preservation` | 738 / `#213-failure-preservation` | converted | — |
| 64 | section | Security, Privacy, and Legal Hygiene | 803 | `## 22. Security, Privacy, and Legal Hygiene` | 742 / `#22-security-privacy-and-legal-hygiene` | converted | — |
| 65 | section | Continuous Integration and Automated Checks | 819 | `## 23. Continuous Integration and Automated Checks` | 755 / `#23-continuous-integration-and-automated-checks` | converted | Historical foundation check list preserved |
| 66 | — | (not in source) | — | §23 continuous-integration operational amendment (blockquote) | 766 | added | Governance LaTeX compilation retired; see Section 9 |
| 67 | section | Versioning and Release Doctrine | 847 | `## 24. Versioning and Release Doctrine` | 779 / `#24-versioning-and-release-doctrine` | converted | — |
| 68 | subsection | Version sequence | 849 | `### 24.1 Version sequence` | 781 / `#241-version-sequence` | converted | `verbatim` → fenced `text` block |
| 69 | subsection | Meaning of Version 1.0.0 | 864 | `### 24.2 Meaning of Version 1.0.0` | 793 / `#242-meaning-of-version-100` | converted | — |
| 70 | subsection | Release record | 870 | `### 24.3 Release record` | 797 / `#243-release-record` | converted | — |
| 71 | section | Conflict Resolution | 884 | `## 25. Conflict Resolution` | 809 / `#25-conflict-resolution` | converted | — |
| 72 | section | Repository Launch Package | 906 | `## 26. Repository Launch Package` | 824 / `#26-repository-launch-package` | converted | — |
| 73 | section | Gate 0B Exit Criteria | 928 | `## 27. Gate 0B Exit Criteria` | 843 / `#27-gate-0b-exit-criteria` | converted | All 14 criteria preserved |
| 74 | — | (not in source) | — | §27 exit-criteria operational amendment (blockquote) | 864 | added | Criterion 9 referent and acknowledgement state; see Section 9 |
| 75 | section | Gate 0B Decision Register | 954 | `## 28. Gate 0B Decision Register` | 866 / `#28-gate-0b-decision-register` | converted | `longtable` → Markdown table, 30 frozen rows; historical intro sentence preserved |
| 76 | — | (not in source) | — | §28 register amendment note (blockquote) | 903 | added | Outside the frozen register; see Section 9 |
| 77 | section | Immediate Next Authorized Work | 1014 | `## 29. Immediate Next Authorized Work` | 905 / `#29-immediate-next-authorized-work` | converted | `quote` → blockquote; may/may-not lists preserved |
| 78 | — | (not in source) | — | §29 operational note (blockquote) | 928 | added | Session-in-progress and Phase 1 boundary; see Section 9 |
| 79 | section* | Approval Status (`\section*` + `\addcontentsline`) | 1045–1046 | `## Approval Status` | 930 / `#approval-status` | converted | Three source statements preserved verbatim; marked amendment note appended at output line 938 |
| 80 | — | (not in source) | — | Approval Status amendment note (blockquote) | 938 | added | Ratified state, acknowledgement, invitation distinction; see Section 9 |
| 81 | environment | signature block (`center`, `\rule`, `\vfill`) | 1060–1066 | two-column signature table | 940–942 | restructured | Names and roles preserved; ruled lines omitted as typesetting |

Document `01` heading totals: source 29 `\section` + 39 `\subsection` + 1 `\section*` = 69 headings; output 1 H1 + 33 H2 + 39 H3 = 73 headings. The four additional output headings are the title H1 rendering of `\maketitle` and the H2 headings `Canonical-Format and Operational-State Amendment Note` (added), `Abstract`, and `Contents`. No source heading was dropped, merged, split, or reordered.

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

Document `01` register (`D0B-01` through `D0B-30`): all 30 expected identifiers were verified present in the source, each exactly once, and the expected family matched the source exactly — no discrepancy. An automated normalized comparison (typography conversions only: `\texttt` → code span, `\_` → `_`, accent commands → Unicode, `\Constitution` → its rendered expansion) confirmed every output row matches its source row. This comparison is preliminary and Claude-assisted; human comparison remains PENDING. No final human equivalence is claimed.

| ID | Source occurrence (line) | Output occurrence (line) | Order preserved | Identifier preserved | Wording preservation (preliminary) | Supersession state | Review state |
| --- | --- | --- | --- | --- | --- | --- | --- |
| D0B-01 | 967 | 872 | yes | yes | verbatim | none | human review PENDING |
| D0B-02 | 968 | 873 | yes | yes | verbatim; `newton\_to\_kerr` → `newton_to_kerr` (typography only) | none | human review PENDING |
| D0B-03 | 969 | 874 | yes | yes | verbatim | none | human review PENDING |
| D0B-04 | 970 | 875 | yes | yes | verbatim; accents → Unicode | none | human review PENDING |
| D0B-05 | 971–972 | 876 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-06 | 973–974 | 877 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-07 | 975–976 | 878 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-08 | 977 | 879 | yes | yes | verbatim | none | human review PENDING |
| D0B-09 | 978 | 880 | yes | yes | verbatim | none | human review PENDING |
| D0B-10 | 979 | 881 | yes | yes | verbatim | none | human review PENDING |
| D0B-11 | 980–981 | 882 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-12 | 982 | 883 | yes | yes | verbatim | none | human review PENDING |
| D0B-13 | 983–984 | 884 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-14 | 985 | 885 | yes | yes | verbatim | none | human review PENDING |
| D0B-15 | 986–987 | 886 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-16 | 988 | 887 | yes | yes | verbatim | none | human review PENDING |
| D0B-17 | 989–990 | 888 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-18 | 991–992 | 889 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-19 | 993–994 | 890 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-20 | 995–996 | 891 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-21 | 997 | 892 | yes | yes | verbatim | reaffirmed; no substantive supersession | human review PENDING |
| D0B-22 | 998 | 893 | yes | yes | verbatim | historical wording preserved; operational referent narrowed by `RDR-0001` to the monograph-scaffold LaTeX build | human review PENDING |
| D0B-23 | 999–1000 | 894 | yes | yes | verbatim; two-line source cell joined; `\Constitution` expanded | none | human review PENDING |
| D0B-24 | 1001 | 895 | yes | yes | verbatim | none | human review PENDING |
| D0B-25 | 1002–1003 | 896 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-26 | 1004 | 897 | yes | yes | verbatim | none | human review PENDING |
| D0B-27 | 1005–1006 | 898 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-28 | 1007–1008 | 899 | yes | yes | verbatim; two-line source cell joined | none | human review PENDING |
| D0B-29 | 1009 | 900 | yes | yes | verbatim | none | human review PENDING |
| D0B-30 | 1010 | 901 | yes | yes | verbatim | historical wording preserved; current activation still requires Gate 0B closeout ratification and explicit NTK-MASTER authorization | human review PENDING |

No `D0B` identifier was renumbered, combined, split, or reworded. No current-state prose was added inside any historical `D0B` row. The register amendment note in the Charter output (line 903) is outside the frozen register.

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

Document `01` substantive custom macros (all verified against the complete source):

| Macro | Source definition | Rendered-content usage count | Markdown expansion | Fidelity note |
| --- | --- | --- | --- | --- |
| `\ProjectTitle` | `From Newton to Kerr` (source line 30) | 4 (lines 37, 50, 66, 123) | literal text `From Newton to Kerr` | exact expansion |
| `\ProjectSubtitle` | `Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics` (line 31) | 2 (lines 38, 124) | literal subtitle text | exact expansion |
| `\RepositoryName` | `from-newton-to-kerr` (line 32) | 1 (line 125, inside `\texttt`) | code span `from-newton-to-kerr` | exact expansion |
| `\PackageName` | `newton\_to\_kerr` (line 33) | 1 (line 126, inside `\texttt`) | code span `newton_to_kerr` | exact expansion; `\_` → `_` |
| `\Constitution` | `Scientific Constitution` (line 34) | 14 | literal text `Scientific Constitution` | exact expansion |
| `\Charter` | `Project Governance and Repository Charter` (line 35) | 6 (including the title) | literal text `Project Governance and Repository Charter` | exact expansion |

Document `01` has no defined-but-unused macros. No macro expansion altered governance meaning.

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

Document `01` mathematics: **None present** — verified from the complete source. The Charter source contains zero inline-math delimiters, zero `equation`/`align` environments, and zero mathematical expressions; the output likewise contains none. No equation audit is applicable to document `01`.

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

Document `01` categories (source counts verified from the complete source):

| Category | Source count | Output count | Disposition |
| --- | --- | --- | --- |
| Tables | 2 (`longtable`: Decision Authority Matrix 10 rows; Gate 0B Decision Register 30 rows) | 4 Markdown tables | Both source tables converted row-for-row. Two authorized additions: document metadata table and signature-block table (Section 9) |
| Unordered lists (`itemize`) | 24 | 25 | All 24 converted; +1 in the added Canonical-Format and Operational-State Amendment Note |
| Ordered lists (`enumerate`) | 8 | 7 ordered + 1 literal-label list | Seven `1.`-style enumerates → Markdown ordered lists; the `G\arabic` Governance Principles list rendered with literal `G1`–`G10` labels to preserve appearance |
| Description lists (`description`) | 4 (identity; branch doctrine; record types; licensing) | 4 bold-label structures | Bold labels reproduce LaTeX description-item typography |
| Quotations (`quote`) | 2 (README status; foundation-session objective) | 9 blockquotes | Both converted; +7 authorized amendment/operational blockquotes (Section 9) |
| Verbatim / code environments | 6 (branch examples; commit types; board states; architecture tree; forbidden paths; foundation tag) | 6 fenced `text` blocks | Byte-faithful content |
| Inline code (`\texttt`) | 25 occurrences | 25 code spans from source | Plus authorized code-formatted governance references in metadata, amendment notes, and this audit |
| Footnotes | None present (verified from complete source) | 0 | — |
| Citations / bibliography | None present (verified from complete source) | 0 | — |
| URLs / external links | None present (verified from complete source) | 0 external | Output adds internal ToC anchor links only (71, all resolving in-file) |
| Source comments | None present (verified: zero `%`-comment lines) | 0 | — |

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

Document `01` non-mechanical changes — complete list. Every change below is authorized by `RDR-0001` (ratified by NTK-MASTER, 17 July 2026) or by the NTK-MASTER operational rulings it records; in every item the historical source wording remains preserved and unrewritten.

1. **Document metadata table** (no source counterpart as a table; renders and extends the `\date{Version 0.1.0 --- Gate 0B Foundational Draft\\16 July 2026}` title block, source lines 37–44; output lines 5–25). Source wording preserved in the `Source version`, `Source date`, and `Declared source-state wording` rows; settled-state and operational rows added (`RATIFIED`, `AUTHORIZED DRAFT`, `NOT YET EFFECTIVE`, `RDR-0001 — RATIFIED`, acknowledgement COMPLETED, invitation SENT — ACCEPTANCE PENDING, Gate 0B IN PROGRESS, Phase 1 BLOCKED, Production Python BLOCKED). Reason: settled-state metadata correction and provenance binding. Authority: `RDR-0001` Sections 1, 3.3; provenance record Section 6.
2. **Canonical-Format and Operational-State Amendment Note** (no source counterpart; output lines 27–45). New marked section stating ratification, authorized-draft state, fidelity-pending state, canonical-transition state, frozen register, operational Phase 1/Gate 0B boundary, acknowledgement/invitation distinction, and the bounded scope of `RDR-0001` supersessions. Authority: `RDR-0001` Section 3.4; NTK-MASTER ruling of 17 July 2026.
3. **Collaboration acknowledgement and invitation distinction** (metadata rows, amendment-note bullets, §27 amendment, Approval Status amendment). Source (lines 218–221, 937–938, 1048–1054) conditions Naomi's representation on acknowledgement; the authoritative current state records acknowledgement COMPLETED and GitHub invitation acceptance PENDING, with no inferred access and no invented dates. Historical conditional wording preserved verbatim in §6.2, §27, and Approval Status. Authority: NTK-MASTER-recorded operational state, 17 July 2026.
4. **Architecture-path amendment** (output lines 651–668, blockquote after the preserved §18 trees; source trees at lines 668–711 and 715–721 preserved byte-faithfully). Identifies `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` and `governance/01_Project_Governance_and_Repository_Charter.md` as the repository paths authorized for eventual canonical adoption; the historical `.tex` governance paths are superseded **only as target repository paths**. It states explicitly that, before every adoption condition is satisfied and the foundation contribution is merged through protected `main`, both Markdown files remain authorized drafts with no adopted canonical authority and the original LaTeX inputs remain the current ratified source representations and immutable provenance inputs. Only the governance-file extensions and exact authorized target paths are superseded. Authority: `RDR-0001` Section 4 rows 1 and 7; Section 3.2 authority transition.
5. **No-empty-directory clarification** (same §18 blockquote). Restates that empty directories are not created to imitate the historical tree and every committed directory must contain a meaningful artifact — reaffirming, not changing, the source paragraph at lines 723–724. Authority: `RDR-0001` Section 1 (format-only change; architecture doctrine untouched).
6. **Build-doctrine amendment** (output lines 682–697, blockquote after preserved §19.2; source lines 734–743 preserved verbatim). Clean-clone LaTeX build now applies to the monograph scaffold; governance-document LaTeX compilation is retired; **during implementation** the authorized Markdown transpositions are subject to structural, link, identifier, and integrity checks; their **canonical authority begins only after** every `RDR-0001` adoption condition is satisfied and the foundation contribution is merged through protected `main`; monograph LaTeX remains authoritative; PDFs remain release artifacts; `D0B-21` unchanged; `D0B-22` narrowed. Authority: `RDR-0001` Sections 3.2 and 4 rows 2, 4, 5.
7. **Overleaf boundary** (same §19.2 blockquote). Overleaf is an independent authoring and compilation environment; no automatic synchronization; manual, reviewed, version-controlled transfers; GitHub is the durable canonical history; Overleaf is not a CI dependency. Source absence: the Charter source does not mention Overleaf. Authority: `RDR-0001` Sections 3.6 and 4 row 6 (additive clarification, not a supersession).
8. **Continuous-integration amendment** (output line 766, blockquote after the preserved foundation check list; source lines 824–831 preserved verbatim, including the historical governance-compilation item). Governance LaTeX compilation retired; Markdown governance integrity checks replace it; monograph-scaffold build retained; broken-link, hygiene, and forbidden-file checks survive; CI success is not scientific validation. Authority: `RDR-0001` Sections 3.5 and 4 row 3.
9. **Gate 0B exit-criteria amendment** (output line 864, blockquote after the preserved 14 criteria; source lines 932–949 preserved verbatim). Criterion 9 now means the clean-clone monograph-scaffold build; Markdown checks separately required; acknowledgement complete / invitation pending; remaining criteria unsatisfied; Gate 0B not complete; Phase 1 not auto-activated; NTK-MASTER closeout ratification and explicit authorization required. Authority: `RDR-0001` Section 4 row 5; NTK-MASTER ruling of 17 July 2026.
10. **D0B-21 reaffirmation** (§28 register amendment note, output line 903). Recorded as reaffirmed without change. Source row (line 997) untouched. Authority: `RDR-0001` Section 4 row 2 ("What remains unchanged").
11. **D0B-22 narrowed referent** (same note). Historical wording preserved (source line 998; output line 893); operational LaTeX-build referent narrowed to the monograph scaffold. Authority: `RDR-0001` Section 4 row 4.
12. **D0B-30 activation clarification** (same note). Historical wording preserved (source line 1010; output line 901); the row records the intended transition but does not itself activate Phase 1 — Gate 0B closeout ratification and explicit NTK-MASTER authorization are required. Authority: NTK-MASTER ruling of 17 July 2026 (Phase 1 BLOCKED).
13. **Immediate Next Authorized Work operational note** (output line 928, blockquote; source section lines 1014–1043 preserved completely). Foundation session in progress; bootstrap and transposition work do not close Gate 0B; Phase 1 and production Python blocked; only complete closeout, ratification, and explicit authorization activate Phase 1. Authority: NTK-MASTER ruling of 17 July 2026.
14. **Approval Status amendment** (output line 938, blockquote; the three source statements at lines 1048–1058 preserved verbatim). Records subsequent ratification, acknowledgement completed, invitation sent with acceptance and access pending, Gate 0B in progress, authorized-draft status, and the Phase 1 / production blocks. Authority: `RDR-0001` Sections 1, 3.4; NTK-MASTER-recorded operational state.
15. **Markdown table of contents** (output lines 51–123; source `\tableofcontents` line 61). Regenerated as explicit anchor links over the resulting heading structure. Mechanical equivalent of the source command.
16. **Explicit section numbering in headings** (`1.`–`29.`, `x.y`). Reproduces LaTeX auto-numbering literally; no renumbering.
17. **Signature-layout conversion** (output lines 940–942; source lines 1060–1066). Two-column signature layout rendered as a table with names and roles preserved; ruled lines omitted as typesetting. Mechanical layout conversion under `RDR-0001` Section 1.

No other document `01` non-mechanical change exists. No current-state prose was inserted into any historical `D0B` row, list item, or source-derived sentence. Semantic fidelity is not claimed to be established by any change above.

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

Document `01` omitted LaTeX-only material (same categories, verified from the complete Charter source): `\documentclass[11pt]{article}` (line 1); the same seventeen package imports (lines 3–14); layout commands (lines 16–20); `\hypersetup` with PDF-only unaccented name metadata (lines 21–28); the definitions (as opposed to expansions) of the six macros (lines 30–35); title machinery `\title`/`\author`/`\date`/`\maketitle` (lines 37–44, content preserved); `\newpage` (line 62), `\vfill` (line 1060), `\rule` signature lines (line 1063), `\addcontentsline` (line 1046); `longtable` column specifications and `\toprule`/`\midrule`/`\bottomrule`/`\endfirsthead`/`\endhead`; `enumitem` list-option keys. The Charter source contains zero comment lines. No substantive content was omitted.

## 11. Automated and Tool-Assisted Checks

The first table below records the checks actually executed on 17 July 2026 in the document-00 task (P00B.3C-1) and its bounded corrections; its Git-scope and forbidden-path rows describe the repository state as it stood at that time, before the document-01 task created the authorized Charter output.

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

Document `01` task checks (P00B.3C-2), every one actually executed on 17 July 2026:

| Check | Method | Result |
| --- | --- | --- |
| Charter source SHA-256 | `sha256sum` before conversion and again after outputs written | `fb74ae93…af3f4` — exact match both times |
| Charter source byte / newline / CR counts | `wc -c`, `wc -l`, `tr`-based CR count | 43382 / 1068 / 0 — exact match |
| Charter source leading bytes | `head -c 3 \| xxd` | `5c646f` — exact match |
| Charter source ignored / untracked | `git check-ignore -v`; `git ls-files` | ignored by `.gitignore:10`; untracked |
| Charter output existence and identity | `wc`, `sha256sum` | 52545 bytes / 942 newlines / `3de90bc1…5ff1` (after the pre-adoption authority corrections) |
| Output UTF-8 decoding | Python strict `bytes.decode('utf-8')` | valid UTF-8 |
| LF-only line endings | CR-byte count via `tr` | 0 CR bytes |
| Final newline | `tail -c 1 \| xxd` | `0x0a` |
| Control-byte scan | `tr` scan for forbidden control bytes | 0 |
| Trailing-whitespace scan | `grep -E ' +$'` | 0 lines |
| Heading inventory | `grep '^#'` vs source sectioning list | 69 source headings all present, order preserved; +4 accounted additions |
| `D0B` identifier inventory | `grep` on source and output | 30/30 in source (each once); output register rows `D0B-01`…`D0B-30` in order |
| `D0B` wording comparison | scripted normalized comparison (typography-only transforms) | all 30 rows match; preliminary, not human review |
| Constitution `D0-*` rows still intact | committed Constitution hash comparison | `61871118…6f9d` unchanged; D0-01…D0-17 untouched |
| Unresolved-LaTeX scan | fixed-string backslash listing over full Charter output | 0 backslash occurrences — no document-level LaTeX remains |
| Drafting-marker scan | case-insensitive scan of the fixed marker set | 0 occurrences; the source-substantive word "placeholder" appears only in its two legitimate governance prohibitions (§4.1 and §26) |
| Internal-link check | Python: GitHub-style anchor generation vs all `](#…)` links | 71/71 links resolve; 0 duplicate anchors |
| Category counts | environment greps on source; structure greps on output | as recorded in Section 8 |
| Git scope check | `git status --porcelain` | one modified tracked file (this audit) and one untracked file (the Charter output); no other change |
| Tracked-record integrity | `sha256sum` of Constitution, RDR-0001, and provenance record | `61871118…6f9d`, `39eb0801…f2ab`, `8cdb9a67…f7f8` — all unchanged |
| Forbidden-architecture check | `git ls-files`; `find governance -type f` | no CI, license, monograph, status, template, or Python path exists |
| Pre-adoption canonical-authority contradiction scan | fixed-string scan for the two rejected premature-canon formulations | 0 occurrences |

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

- Document `01` has been **transposed as an authorized draft** at `governance/01_Project_Governance_and_Repository_Charter.md` in task P00B.3C-2 (17 July 2026). Its source identity (SHA-256 `fb74ae936a6dba21efe4aab1d6b6f099d57dbeded6ca56c55cff0ce6c33af3f4`) is recorded in `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md` and in Section 2 above.
- Its structural mapping (Section 4), `D0B` register audit (Section 5), macro and category inventories (Sections 6–8), and non-mechanical change record (Section 9) are complete at the preliminary, tool-assisted level.
- The output remains an **AUTHORIZED DRAFT — NOT YET CANONICAL**; no conclusion of established semantic fidelity is asserted.

Preliminary cross-document consistency review — **preliminary and tool-assisted; human comparison remains PENDING**. The two Markdown transpositions were compared on the following points, with no inconsistency found:

| Consistency point | Result |
| --- | --- |
| Project name | `From Newton to Kerr` identical in both documents |
| Scientific subtitle | identical in both metadata tables and title blocks |
| Roles | Edgar Axel Pérez Flores (Scientific Lead; Repository Owner / final signatory) and Naomi Sánchez Torres (Scientific Collaborator and Co-developer) consistent |
| Authority hierarchy | Charter §2.1 places the Constitution above the Charter; the Constitution transposition makes no contrary claim |
| Scientific-spine noninterference | the Charter changes no scientific thesis, model set, evidence level, or completion criterion; Constitution Sections 3–11 untouched by Charter content |
| Phase 1 boundary | both documents state Phase 1 remains blocked pending Gate 0B closeout ratification and explicit NTK-MASTER authorization |
| Production-Python prohibition | both documents state production Python architecture and implementation remain blocked |
| Final author-order deferral | Constitution §16 / D0-15 and Charter §16.2 / D0B-29 consistently defer author order |
| `RDR-0001` authority | both documents cite `RDR-0001` — RATIFIED as the authorizing decision for format transposition |
| Canonical-transition state | both documents state NOT YET EFFECTIVE and AUTHORIZED DRAFT |
| GitHub documentary authority | Charter §2.2 / D0B-06 and the Constitution's product architecture consistently treat the merged repository as the documentary source of truth |
| Monograph / preprint LaTeX boundary | both documents keep the monograph and future preprint as LaTeX works with Overleaf as an independent, non-CI environment |
| No claim of adopted canon | neither Markdown file claims adopted canonical authority before completion of the `RDR-0001` adoption conditions and protected-`main` merge |

## 14. Human Review and Adoption Record

| Step | State |
| --- | --- |
| Claude Code bounded drafting and preliminary self-audit (document 00) | completed |
| Claude Code bounded drafting and preliminary audit (document 01) | completed |
| Document-01 transposition | completed as authorized draft |
| Edgar comparison of document 00 | pending |
| Edgar comparison of document 01 | pending |
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

- Both Markdown transpositions exist as **authorized drafts**: `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` and `governance/01_Project_Governance_and_Repository_Charter.md`.
- The preliminary traceability audit (this record) **covers both documents**.
- Human semantic comparison remains **pending** for both documents.
- Naomi Sánchez Torres's independent review remains **pending**.
- Edgar Axel Pérez Flores's final scientific sign-off remains **pending**.
- The canonical transition remains **not yet effective**.
- Gate 0B remains **active** and not yet complete.
- Phase 1 remains **blocked**.
- Production Python remains **blocked**.
- Next step: independent human inspection of document `01` and of this completed audit before any commit.
