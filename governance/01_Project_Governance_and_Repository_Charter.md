# Project Governance and Repository Charter for From Newton to Kerr

*Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics*

| Field | Value |
| --- | --- |
| Document | Project Governance and Repository Charter for From Newton to Kerr |
| Scientific subtitle | Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics |
| Source version | 0.1.0 |
| Source date | 16 July 2026 |
| Declared source-state wording | `Gate 0B Foundational Draft` |
| Substantive governance state | RATIFIED |
| Transposition state | AUTHORIZED DRAFT |
| Canonical authority | NOT YET EFFECTIVE |
| Related repository decision | `RDR-0001` — RATIFIED |
| Source filename | `01_Project_Governance_and_Repository_Charter.tex` |
| Source SHA-256 | `fb74ae936a6dba21efe4aab1d6b6f099d57dbeded6ca56c55cff0ce6c33af3f4` |
| Scientific Lead and Repository Owner | Edgar Axel Pérez Flores |
| Scientific Collaborator and Co-developer | Naomi Sánchez Torres |
| Collaboration-terms acknowledgement | COMPLETED |
| GitHub collaborator access | INVITATION SENT — ACCEPTANCE PENDING |
| Governing workstream | `[NTK-P00B]` Repository and Collaboration Foundation |
| Current gate | Gate 0B — IN PROGRESS |
| Phase 1 | BLOCKED |
| Production Python | BLOCKED |

## Canonical-Format and Operational-State Amendment Note

This note is a format-governance and operational-state notice authorized by `RDR-0001`. It is placed outside the frozen historical decision register and changes no scientific or governance substance.

- The substantive Project Governance and Repository Charter was already **ratified**; that ratification is recorded in the master project record and is presupposed, not re-performed, by this file.
- This file is an authorized Markdown transposition prepared to preserve the complete rendered substantive content of the ratified LaTeX source `01_Project_Governance_and_Repository_Charter.tex` under the ratified repository decision `RDR-0001`.
- Its semantic fidelity remains subject to the required human comparison, Naomi Sánchez Torres's independent review, and Edgar Axel Pérez Flores's final scientific sign-off.
- The canonical-format transition is **not yet effective**. This file has no adopted canonical authority merely because it exists.
- Until protected-`main` adoption, the original LaTeX source remains the **current ratified source representation** and an **immutable provenance input**, identified byte-exactly in `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md`.
- After protected-`main` adoption under the conditions of `RDR-0001`, this Markdown file becomes the **canonical repository governance instrument**, and the LaTeX source remains provenance evidence only, with no authority to override, reinterpret, or amend the Markdown canon.
- The historical Gate 0B decision register (`D0B-01` through `D0B-30`) remains **frozen** below in its original wording, order, and historical meaning. It is not silently rewritten.
- The Charter's historical approval, launch, repository-state, and Phase 1 language is preserved verbatim, but it does not override the current operational state.
- Gate 0B remains **incomplete**.
- Phase 1 remains **blocked** until Gate 0B closes, its closeout is ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1.
- Production Python architecture and implementation remain **blocked**.
- Naomi Sánchez Torres's acknowledgement of the collaboration terms is **complete**; she is the confirmed Scientific Collaborator and Co-developer.
- A GitHub collaborator invitation has been sent to Naomi Sánchez Torres, but **acceptance remains pending**; no active repository access is inferred from the invitation.
- `RDR-0001` supersedes only the explicitly enumerated format, build, and continuous-integration requirements identified in its Section 4 supersession table and reflected in the marked amendment notes below.
- No other governance or scientific substance is changed by this transposition. Any substantive divergence from the ratified source is by definition a conversion defect and must be corrected against the original.

## Abstract

This charter defines the governance, authority structure, repository doctrine, collaboration rules, contribution workflow, decision process, attribution policy, licensing model, use of artificial-intelligence tools, quality controls, release discipline, and launch criteria of From Newton to Kerr. It operationalizes the ratified scientific direction established by the project's Scientific Constitution. The repository shall be public from its first formal day, but public visibility shall not be confused with scientific readiness: incomplete work may be visible, whereas unsupported claims, unreviewed production results, undocumented decisions, and premature release language are prohibited. The repository shall function simultaneously as a versioned scientific record, a collaborative workspace, a reproducibility platform, and the public home of the monograph, software, evidence, and eventual preprint. External conversations and AI-assisted work may support the project, but only reviewed and merged repository artifacts have documentary authority.

## Contents

- [Canonical-Format and Operational-State Amendment Note](#canonical-format-and-operational-state-amendment-note)
- [Abstract](#abstract)
- [1. Purpose and Authority](#1-purpose-and-authority)
- [2. Relationship to the Scientific Constitution](#2-relationship-to-the-scientific-constitution)
  - [2.1 Authority hierarchy](#21-authority-hierarchy)
  - [2.2 Repository as documentary source of truth](#22-repository-as-documentary-source-of-truth)
  - [2.3 Amendment boundary](#23-amendment-boundary)
- [3. Project and Repository Identity](#3-project-and-repository-identity)
- [4. Public-From-Day-One Doctrine](#4-public-from-day-one-doctrine)
  - [4.1 Meaning of public development](#41-meaning-of-public-development)
  - [4.2 Required public status declaration](#42-required-public-status-declaration)
- [5. Governance Principles](#5-governance-principles)
- [6. Human Roles and Responsibilities](#6-human-roles-and-responsibilities)
  - [6.1 Edgar Axel Pérez Flores: Scientific Lead and Repository Owner](#61-edgar-axel-pérez-flores-scientific-lead-and-repository-owner)
  - [6.2 Naomi Sánchez Torres: Scientific Collaborator and Co-developer](#62-naomi-sánchez-torres-scientific-collaborator-and-co-developer)
  - [6.3 Shared responsibilities](#63-shared-responsibilities)
  - [6.4 No shared credentials](#64-no-shared-credentials)
- [7. Decision Authority Matrix](#7-decision-authority-matrix)
- [8. Classes of Change and Review Requirements](#8-classes-of-change-and-review-requirements)
  - [8.1 Class A: Constitutional and scientific-authority changes](#81-class-a-constitutional-and-scientific-authority-changes)
  - [8.2 Class B: Scientific implementation and evidence changes](#82-class-b-scientific-implementation-and-evidence-changes)
  - [8.3 Class C: Administrative and low-risk changes](#83-class-c-administrative-and-low-risk-changes)
- [9. Repository Access and Protection](#9-repository-access-and-protection)
  - [9.1 Account roles](#91-account-roles)
  - [9.2 Protection of the default branch](#92-protection-of-the-default-branch)
- [10. Git Workflow](#10-git-workflow)
  - [10.1 Branch doctrine](#101-branch-doctrine)
  - [10.2 Commit doctrine](#102-commit-doctrine)
  - [10.3 Merge strategy](#103-merge-strategy)
- [11. Pull-Request Standard](#11-pull-request-standard)
- [12. Issues, Milestones, and Project Tracking](#12-issues-milestones-and-project-tracking)
  - [12.1 Issues](#121-issues)
  - [12.2 Milestones](#122-milestones)
  - [12.3 Project board](#123-project-board)
- [13. Decision Records](#13-decision-records)
  - [13.1 Record types](#131-record-types)
  - [13.2 Required fields](#132-required-fields)
- [14. Master Orchestration and Specialized Work Sessions](#14-master-orchestration-and-specialized-work-sessions)
  - [14.1 Master orchestration](#141-master-orchestration)
  - [14.2 Specialized sessions](#142-specialized-sessions)
- [15. Use of Artificial-Intelligence Tools](#15-use-of-artificial-intelligence-tools)
  - [15.1 Permitted role](#151-permitted-role)
  - [15.2 Human accountability](#152-human-accountability)
  - [15.3 Disclosure](#153-disclosure)
- [16. Authorship, Attribution, and Contribution Records](#16-authorship-attribution-and-contribution-records)
  - [16.1 Repository attribution](#161-repository-attribution)
  - [16.2 Publication authorship](#162-publication-authorship)
  - [16.3 External contributors](#163-external-contributors)
- [17. Licensing Doctrine](#17-licensing-doctrine)
- [18. Initial Repository Architecture](#18-initial-repository-architecture)
- [19. Monograph and LaTeX Governance](#19-monograph-and-latex-governance)
  - [19.1 Authoritative source](#191-authoritative-source)
  - [19.2 Build doctrine](#192-build-doctrine)
  - [19.3 Writing standard](#193-writing-standard)
- [20. Citation and Source Governance](#20-citation-and-source-governance)
- [21. Data, Figures, and Reproducibility](#21-data-figures-and-reproducibility)
  - [21.1 Generated evidence](#211-generated-evidence)
  - [21.2 Repository size discipline](#212-repository-size-discipline)
  - [21.3 Failure preservation](#213-failure-preservation)
- [22. Security, Privacy, and Legal Hygiene](#22-security-privacy-and-legal-hygiene)
- [23. Continuous Integration and Automated Checks](#23-continuous-integration-and-automated-checks)
- [24. Versioning and Release Doctrine](#24-versioning-and-release-doctrine)
  - [24.1 Version sequence](#241-version-sequence)
  - [24.2 Meaning of Version 1.0.0](#242-meaning-of-version-100)
  - [24.3 Release record](#243-release-record)
- [25. Conflict Resolution](#25-conflict-resolution)
- [26. Repository Launch Package](#26-repository-launch-package)
- [27. Gate 0B Exit Criteria](#27-gate-0b-exit-criteria)
- [28. Gate 0B Decision Register](#28-gate-0b-decision-register)
- [29. Immediate Next Authorized Work](#29-immediate-next-authorized-work)
- [Approval Status](#approval-status)

## 1. Purpose and Authority

This charter establishes how From Newton to Kerr shall be governed and how its public repository shall be created, maintained, reviewed, and released. It is a binding operational document, not an informal list of preferences.

The charter has five purposes:

1. protect the scientific coherence established by the Scientific Constitution;
2. create a fair, traceable, and reviewable collaboration between the two human collaborators;
3. make the repository a trustworthy scientific record rather than a storage location;
4. define how theory, software, evidence, writing, and public claims advance through review;
5. prevent speed, tooling, or public visibility from replacing scientific judgment.

Approval of this charter authorizes the repository-foundation session. It does not authorize production solvers, numerical campaigns, final orbit classifications, or publication claims.

## 2. Relationship to the Scientific Constitution

### 2.1 Authority hierarchy

Project authority shall follow the hierarchy below, in descending order:

1. the current ratified Scientific Constitution;
2. ratified constitutional amendments and scientific decision records;
3. the current ratified Project Governance and Repository Charter;
4. approved phase specifications and physics-to-software contracts;
5. merged pull requests, issue resolutions, benchmark registries, and release records;
6. external notes, conversations, AI-assisted sessions, and unmerged drafts.

If two records conflict, the higher-authority record controls until a formal amendment resolves the conflict.

### 2.2 Repository as documentary source of truth

The public Git repository shall become the durable documentary source of truth. A conclusion, scope change, convention, benchmark, role assignment, or release authorization discussed in a conversation is not formally adopted until it is converted into an appropriate repository artifact, reviewed, and merged.

External working conversations may remain useful as reasoning and coordination environments, but they shall not be treated as permanent governance records. Raw conversation transcripts shall not be committed as substitutes for curated scientific documentation.

### 2.3 Amendment boundary

This charter may refine operations but may not silently change the scientific thesis, mandatory model set, evidence hierarchy, or completion criteria established by the Scientific Constitution. Such a change requires a constitutional amendment.

## 3. Project and Repository Identity

**Public project title:** From Newton to Kerr

**Scientific subtitle:** Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics

**Repository name:** `from-newton-to-kerr`

**Future Python package name:** `newton_to_kerr`

**Repository owner:** Edgar Axel Pérez Flores

**Confirmed collaborator:** Naomi Sánchez Torres

**Primary technical language:** English

**Production implementation language:** Python only

**Repository visibility:** Public from the first formal repository release

The repository name is intentionally concise and narrative. The package name is reserved but shall not be instantiated until the Python-infrastructure phase authorizes a package scaffold.

## 4. Public-From-Day-One Doctrine

### 4.1 Meaning of public development

Public development means that the scientific process, not merely the final result, is visible. The repository may therefore contain incomplete but accurately labeled work, including:

- theory chapters under active review;
- literature maps and benchmark registries;
- unresolved scientific decision records;
- early software infrastructure;
- validation failures that are preserved and explained;
- explicit blockers and limitations.

Public development does not permit:

- overstated readiness;
- unsupported physical claims;
- decorative placeholder results presented as evidence;
- large numbers of empty directories suggesting nonexistent capability;
- unlicensed third-party material;
- private information, credentials, or unpublished material without permission;
- misleading use of words such as “validated,” “research-grade,” or “publication-ready.”

### 4.2 Required public status declaration

The root README shall always state the current phase, the highest completed gate, and the highest authorized type of work. The initial status shall be substantively equivalent to:

> **Current status:** Repository Foundation. The scientific constitution has been ratified. Literature cartography and theoretical development are pending. Production numerical models and scientific results have not yet been authorized.

The status shall be updated at every milestone release.

## 5. Governance Principles

The project adopts the following permanent principles:

- G1. **Scientific authority precedes implementation authority.**
- G2. **The repository records decisions; conversations propose them.**
- G3. **Every critical contribution has an author and an independent reviewer.**
- G4. **No collaborator reviews their own critical work as the sole reviewer.**
- G5. **Attribution follows documented contribution, not repository access.**
- G6. **Public visibility never lowers the evidence threshold.**
- G7. **No tool, including an AI assistant, may silently determine scientific scope, equations, citations, or claims.**
- G8. **Disagreement blocks a critical merge until the disagreement is resolved or explicitly deferred.**
- G9. **A smaller verified result is preferred to a broader unverified result.**
- G10. **The repository shall remain reconstructible from a clean clone.**

## 6. Human Roles and Responsibilities

### 6.1 Edgar Axel Pérez Flores: Scientific Lead and Repository Owner

Edgar shall serve as:

- scientific lead;
- repository owner and final administrative maintainer;
- primary theoretical architect;
- primary owner of project scope, scientific doctrine, and public claims;
- final scientific signatory for phase and release authorization;
- principal integrator of the monograph and preprint narrative;
- guardian of consistency between derivation, implementation, evidence, and interpretation.

Edgar's final scientific authority does not waive review. His critical derivations, code, and claims must receive independent review before they may become publication-grade evidence.

### 6.2 Naomi Sánchez Torres: Scientific Collaborator and Co-developer

Naomi shall be recognized as a substantive scientific collaborator and co-developer, subject to her acknowledgement of this charter. Her responsibilities may include:

- implementation and maintenance of assigned computational components;
- independent review of derivations and physics-to-software contracts;
- construction of tests, validation studies, and reproducible examples;
- scientific visualization and result interpretation;
- review and co-authorship of documentation and publication materials;
- contribution to issue triage, milestone planning, and release review.

The exact assignment of modules, chapters, code ownership, and review duties remains deferred to a later work-allocation record. This charter does not presume that Naomi is merely an implementation assistant, nor that all code belongs to her by default.

### 6.3 Shared responsibilities

Both collaborators shall:

- work through version-controlled branches and pull requests;
- document assumptions, limitations, and known failures;
- review one another's critical work;
- preserve attribution and co-authorship metadata;
- avoid presenting proposed work as completed work;
- protect the repository from secrets and improperly licensed material;
- keep public communication consistent with the current evidence level;
- disclose conflicts of interest or external restrictions relevant to the project.

### 6.4 No shared credentials

Repository access shall be granted through individual accounts. Passwords, tokens, signing keys, or recovery credentials shall never be shared between collaborators or committed to the repository.

## 7. Decision Authority Matrix

| Decision domain | Primary proposer | Required review | Final authority |
| --- | --- | --- | --- |
| Scientific thesis, mandatory scope, and nonclaims | Edgar or either collaborator | Both collaborators; literature evidence required | Edgar through constitutional amendment |
| Mathematical conventions and model equations | Assigned theory author | Independent scientific review | Edgar after recorded resolution |
| Physics-to-software contracts | Theory author or implementer | Independent theory and implementation review | Assigned gate owner; Edgar signs scientific authorization |
| Software architecture | Assigned maintainer | Other collaborator; scientific compatibility check | Edgar as repository owner after review |
| Module implementation | Assigned implementer | Non-author review and required checks | Assigned module owner within approved contract |
| Benchmark tolerances and production criteria | Validation owner | Independent review; evidence required | Edgar after joint review |
| Repository administration and access | Edgar | Consultation when collaborator access is affected | Edgar |
| Licensing and public attribution | Edgar | Naomi's consent for her name and contributions | Edgar for repository; each author controls attribution to themselves |
| Release authorization | Release proposer | Both collaborators for scientific releases | Edgar as release signatory |
| Preprint submission and author order | Both collaborators | Explicit joint agreement | No submission without both authors' approval |

No person may authorize attribution, authorship, or public statements on behalf of the other without explicit consent.

## 8. Classes of Change and Review Requirements

Every pull request shall be classified as one of the following.

### 8.1 Class A: Constitutional and scientific-authority changes

Class A includes:

- changes to thesis, scope, mandatory modules, nonclaims, or evidence levels;
- new physical models or major changes to equations;
- frozen conventions;
- publication claims;
- production benchmark criteria;
- licensing, attribution, or authorship policy;
- phase or release authorization.

Class A requires:

- a linked decision record;
- review by both collaborators when both are active;
- explicit scientific sign-off by Edgar;
- all required checks passing;
- no unresolved blocking comment.

### 8.2 Class B: Scientific implementation and evidence changes

Class B includes:

- theory chapters that enable implementation;
- model code, integrators, events, and diagnostics;
- tests, benchmarks, datasets, figures, and classifications;
- physics-to-software contracts;
- reproducibility scripts and numerical-methodology documentation.

Class B requires at least one approval from a non-author collaborator, relevant automated checks, and resolution of all scientific review comments.

### 8.3 Class C: Administrative and low-risk changes

Class C includes:

- typographical corrections that do not alter meaning;
- formatting, links, and repository metadata;
- issue templates and non-scientific workflow maintenance;
- dependency housekeeping that does not change scientific outputs.

A collaborator may merge Class C work after required checks pass. Any reviewer may reclassify a change as Class A or B if its impact is larger than stated.

## 9. Repository Access and Protection

### 9.1 Account roles

Edgar shall hold administrative ownership. Naomi should receive collaborator access appropriate to active development after acknowledging this charter. Administrative access shall be granted only if it becomes operationally necessary.

### 9.2 Protection of the default branch

After the bootstrap commit, the default branch `main` shall be protected with the following rules whenever supported by the hosting platform:

- pull requests required before merge;
- required status checks;
- stale approvals dismissed after material changes;
- force pushes prohibited;
- branch deletion prohibited;
- linear history required;
- unresolved review conversations prohibited at merge;
- direct pushes prohibited except for a documented repository-recovery emergency.

Emergency use shall be followed by a public incident note explaining why the normal process was not possible.

## 10. Git Workflow

### 10.1 Branch doctrine

The project shall use one stable branch and short-lived working branches.

- **`main`** — Stable, reviewed, and consistent with the current public status.
- **`foundation/...`** — Foundational governance or repository work.
- **`research/...`** — Literature maps, benchmark registries, and source audits.
- **`theory/...`** — Mathematical and physical development.
- **`feat/...`** — New software capability authorized by an approved contract.
- **`fix/...`** — Corrections to theory, software, evidence, or documentation.
- **`test/...`** — Validation and testing work.
- **`docs/...`** — Documentation that does not change scientific authority.
- **`release/...`** — Temporary release-preparation work when required.

Branch names shall be lowercase, hyphenated, and specific, for example:

```text
foundation/public-repository
research/kerr-source-map
theory/schwarzschild-effective-potential
feat/kepler-invariant-diagnostics
test/one-pn-precession-convergence
```

Long-lived personal branches are discouraged. Abandoned branches shall be closed or documented.

### 10.2 Commit doctrine

Commits shall be logically coherent and use an imperative summary. The preferred types are:

```text
theory:   add or revise physical derivations
research: add literature or benchmark evidence
feat:     add authorized scientific-software capability
fix:      correct theory, software, evidence, or documentation
test:     add or strengthen validation
refactor: reorganize without intended scientific change
docs:     improve explanatory or user documentation
ci:       modify automated checks
chore:    perform repository maintenance
```

Commits shall not claim validation or completion unless the associated evidence exists. Temporary work-in-progress commits may exist on branches but should be cleaned before merge.

### 10.3 Merge strategy

Squash merge shall be the default. The pull-request title and body therefore become part of the permanent scientific record and must accurately summarize the merged contribution.

When multiple people contributed directly, the squash commit shall preserve appropriate co-author trailers or equivalent attribution. Merge commits may be used only for a documented release or recovery reason.

## 11. Pull-Request Standard

Every Class A or B pull request shall include:

1. objective and change class;
2. scientific or operational motivation;
3. authoritative equations, assumptions, or decision records affected;
4. files and interfaces changed;
5. tests, derivations, or validation evidence added;
6. known limitations and unresolved risks;
7. public claims enabled, changed, or still blocked;
8. reproducibility instructions where applicable;
9. reviewer checklist;
10. explicit statement that AI-generated material, if used, was human-reviewed.

A pull request shall remain a draft while its central scientific content is knowingly incomplete. Review comments that affect correctness must be resolved in code or documentation, not merely acknowledged in conversation.

## 12. Issues, Milestones, and Project Tracking

### 12.1 Issues

An issue shall describe one reviewable problem, decision, or deliverable. Every substantive issue should include:

- phase and module;
- objective;
- dependencies;
- acceptance criteria;
- evidence required;
- owner and reviewer when assigned;
- blockers and non-goals.

Issues shall not be used to declare a scientific result without linking the merged evidence.

### 12.2 Milestones

GitHub milestones shall correspond to ratified project gates or major phase packages, not to arbitrary calendar periods. Completion percentage is not evidence of scientific readiness.

### 12.3 Project board

A single lightweight project board may use the states:

```text
Backlog -> Ready -> In Progress -> Review -> Blocked -> Done
```

An item enters `Done` only when its acceptance criteria are satisfied and its authoritative artifact is merged.

## 13. Decision Records

### 13.1 Record types

The repository shall maintain two forms of durable decision record:

- **Scientific Decision Record (SDR)** — Equations, conventions, model choices, benchmarks, scope interpretations, classification rules, and scientific claims.
- **Repository Decision Record (RDR)** — Architecture, tooling, licensing, workflow, release, and operational decisions.

### 13.2 Required fields

Every decision record shall contain:

1. identifier and title;
2. status: proposed, accepted, superseded, or rejected;
3. date and decision owners;
4. context and problem;
5. options considered;
6. decision and rationale;
7. evidence and references;
8. consequences and risks;
9. affected files or phases;
10. supersession relationship when applicable.

Accepted records shall never be silently rewritten to conceal prior reasoning. Corrections shall be made through a new record or a clearly documented amendment.

## 14. Master Orchestration and Specialized Work Sessions

### 14.1 Master orchestration

The project may use a master orchestration conversation to coordinate phase status, handoffs, ratifications, and next actions. This working channel does not supersede the repository. Decisions reached there shall be transcribed into a decision record, charter amendment, phase specification, or status file before they become authoritative.

### 14.2 Specialized sessions

Literature research, theoretical modules, numerical methods, software implementation, validation campaigns, and publication writing may be developed in separate specialized sessions. Each specialized session shall receive a written handoff containing:

- current ratified phase;
- objective and allowed scope;
- authoritative inputs;
- required deliverables;
- decisions it may propose;
- decisions it may not make;
- evidence standard;
- exit criteria.

Its closeout shall report:

- work completed;
- ratifiable findings;
- artifacts created;
- sources and evidence;
- unresolved questions;
- blockers;
- proposed next action.

No specialized session may independently expand the mandatory project scope.

## 15. Use of Artificial-Intelligence Tools

### 15.1 Permitted role

AI systems, including ChatGPT, Claude, coding assistants, and symbolic tools, may support:

- planning and structured drafting;
- literature-search strategy;
- algebraic and dimensional checks;
- software scaffolding and implementation support;
- test design and code review;
- language editing and documentation;
- repository maintenance and workflow execution.

### 15.2 Human accountability

AI output has no independent scientific authority. Every AI-assisted equation, citation, argument, code path, benchmark, and claim shall be reviewed by a human collaborator before merge. The human author who submits the pull request remains accountable for the material.

The following are prohibited:

- citing a source that has not been opened and verified;
- treating generated algebra as a derivation without independent checking;
- merging generated code whose interfaces, failure modes, and tests are not understood;
- allowing an AI system to invent numerical results or metadata;
- listing an AI system as an author or contributor equivalent to a human collaborator;
- uploading confidential, restricted, or improperly licensed material to an external system without authorization.

### 15.3 Disclosure

Substantive AI assistance shall be disclosed in the manner required by the publication venue or, in the absence of a venue requirement, in an appropriate acknowledgements or methodology note. Routine spelling, formatting, and code-completion assistance need not be itemized commit by commit.

## 16. Authorship, Attribution, and Contribution Records

### 16.1 Repository attribution

`AUTHORS.md` shall identify the human collaborators and their current roles. A separate contribution record shall document substantial work by module and release.

Repository access, commit count, line count, or administrative ownership shall not alone determine scholarly authorship.

### 16.2 Publication authorship

The author list and order of the final preprint shall be decided only after substantial work is complete. The decision shall consider contributions to:

- conceptualization;
- theoretical derivation;
- methodology;
- software;
- validation;
- investigation and results;
- visualization;
- writing and revision;
- project administration.

No preprint shall be submitted without both named human authors reviewing the final manuscript and explicitly approving submission and author order.

### 16.3 External contributors

Future contributors shall receive attribution appropriate to their documented contribution. External contribution does not automatically confer manuscript authorship or decision authority.

## 17. Licensing Doctrine

The project adopts a dual-license model:

- **Software license:** MIT License for original source code, tests, and scripts.
- **Written and visual material:** Creative Commons Attribution 4.0 International for the original monograph, documentation, diagrams, and figures, unless a file states otherwise.
- **Project-generated datasets:** Creative Commons Attribution 4.0 International by default, subject to any later dataset-specific requirements.

Third-party material retains its original license and may not be relicensed by this project. The repository shall not distribute copyrighted papers or book scans merely because they were used as references. The references directory shall store bibliographic metadata, links, provenance notes, and legally distributable materials only.

Both collaborators must consent before their original contribution is publicly distributed under a license not already accepted through this charter or a later contribution agreement.

## 18. Initial Repository Architecture

The repository shall begin with a theory-first structure. It shall not contain a fabricated software architecture before computational contracts exist.

```text
from-newton-to-kerr/
|-- README.md
|-- AUTHORS.md
|-- CONTRIBUTING.md
|-- CITATION.cff
|-- CHANGELOG.md
|-- LICENSE-CODE
|-- LICENSE-DOCS
|-- .gitignore
|-- .editorconfig
|
|-- governance/
|   |-- 00_Scientific_Constitution.tex
|   |-- 01_Project_Governance_and_Repository_Charter.tex
|   |-- decisions/
|   |   |-- scientific/
|   |   `-- repository/
|   `-- status/
|       `-- MASTER_STATUS.md
|
|-- monograph/
|   |-- main.tex
|   |-- frontmatter/
|   |-- chapters/
|   |-- appendices/
|   |-- figures/
|   `-- tables/
|
|-- references/
|   |-- bibliography.bib
|   |-- source_registry.md
|   `-- benchmark_registry.md
|
|-- research/
|   |-- literature_maps/
|   |-- equation_registry/
|   `-- notes/
|
`-- .github/
    |-- pull_request_template.md
    |-- ISSUE_TEMPLATE/
    `-- workflows/
```

The following shall remain absent until formally authorized:

```text
src/
tests/
notebooks/
results/
pyproject.toml
```

Directories shall be added when they contain an approved function and at least one meaningful artifact. Empty architectural theater is prohibited.

> **Operational amendment (`RDR-0001`; NTK-MASTER, 17 July 2026):** The
> directory tree above is preserved as ratified historical source wording.
> Under the ratified decision `RDR-0001`, the repository paths authorized for
> eventual canonical adoption are
> `governance/00_Scientific_Constitution_From_Newton_to_Kerr.md` and
> `governance/01_Project_Governance_and_Repository_Charter.md`; the historical
> `.tex` governance paths shown in the tree are superseded as target
> repository paths. Until every adoption condition is satisfied and the
> foundation contribution is merged through protected `main`, both Markdown
> files remain authorized drafts with no adopted canonical authority, and the
> original LaTeX inputs remain the current ratified source representations
> and immutable provenance inputs. Only the governance-file extensions and
> the exact authorized target paths are superseded by `RDR-0001` — no other
> element of the architecture doctrine changes. Empty directories are not
> created merely to imitate the historical tree; every committed directory
> must contain a meaningful artifact, exactly as the paragraph above
> requires. All forbidden Python paths (`src/`, `tests/`, `notebooks/`,
> `results/`, `pyproject.toml`) remain blocked.

## 19. Monograph and LaTeX Governance

### 19.1 Authoritative source

The LaTeX source in `monograph/` shall be authoritative. Generated PDFs are release artifacts and shall not replace source control of the underlying text, bibliography, figures, and tables.

### 19.2 Build doctrine

The initial repository shall define one reproducible LaTeX build command, preferably through `latexmk`. The exact TeX distribution and required packages shall be documented. A clean clone must be able to build the current governance and monograph documents using the documented toolchain.

Generated auxiliary files shall not be committed. Release PDFs may be attached to tagged releases or stored in a designated release-assets location if the repository policy later permits it.

> **Operational amendment (`RDR-0001`; NTK-MASTER, 17 July 2026):** Under the
> ratified decision `RDR-0001`, the clean-clone LaTeX build requirement now
> applies to the **monograph scaffold**. Governance-document LaTeX compilation
> is retired. During implementation, the authorized Markdown transpositions
> are subject to structural, link, identifier, and integrity checks; they
> become the canonical repository governance documents only after every
> `RDR-0001` adoption condition is satisfied and the foundation contribution
> is merged through protected `main`. The monograph LaTeX source remains
> authoritative, and generated PDFs remain release artifacts (`D0B-21` is
> unchanged). `D0B-22` is narrowed in scope to the monograph-scaffold LaTeX
> build. The monograph and the future preprint remain LaTeX works. Overleaf is
> an independent authoring and compilation environment; no automatic
> Overleaf–GitHub synchronization is required; transfers of monograph or
> preprint content are manual, reviewed, and version controlled; the merged
> GitHub source remains the durable canonical history; and Overleaf is not a
> continuous-integration dependency.

### 19.3 Writing standard

All formal material shall use strong academic English, with an internal minimum target comparable to IELTS Academic Band 7. Clarity and precision take precedence over ornate language. Technical terms, notation, capitalization, spelling conventions, and hyphenation shall remain consistent across the monograph, repository, and preprint.

## 20. Citation and Source Governance

Every substantive physical equation, benchmark, or literature claim shall have traceable source provenance. Bibliographic entries shall be verified against the original publication or an authoritative index.

The project shall distinguish:

- primary scientific sources;
- textbooks and monographs;
- numerical-method references;
- authoritative documentation;
- secondary explanatory material.

Secondary material may guide understanding but shall not replace primary or authoritative sources for critical equations and claims when such sources are available.

Source notes may summarize copyrighted work, but shall not reproduce substantial protected text or figures without permission.

## 21. Data, Figures, and Reproducibility

### 21.1 Generated evidence

Every production dataset or figure shall be linked to:

- the generating script or command;
- configuration and initial conditions;
- software and environment identity;
- integrator and tolerances;
- event and termination criteria;
- invariant or constraint diagnostics;
- source commit or release;
- a declared evidence level.

### 21.2 Repository size discipline

Large generated files shall not be committed by default. The project shall use release assets, external archival storage, or a later ratified large-file policy when necessary. Small trusted regression fixtures may be committed when their scientific purpose and provenance are clear.

### 21.3 Failure preservation

Scientifically informative failures shall be documented rather than hidden. A failed validation shall not be promoted as a result, but its configuration and diagnosis may be preserved when it prevents repeated mistakes or informs later methodology.

## 22. Security, Privacy, and Legal Hygiene

The repository shall never contain:

- passwords, API keys, access tokens, private keys, or recovery codes;
- private addresses, personal identifiers, or unrelated personal records;
- proprietary code or data without permission;
- copyrighted papers, books, or figures without a redistribution right;
- credentials embedded in notebook outputs, logs, or configuration files;
- confidential peer-review or unpublished third-party material.

A secret detected in Git history shall be revoked immediately and removed through an appropriate history-cleaning procedure. Merely deleting it in a later commit is insufficient.

## 23. Continuous Integration and Automated Checks

Automated checks shall grow with the project and shall not simulate capabilities that do not yet exist.

At repository foundation, the required checks should include:

- LaTeX compilation of governance documents and the monograph scaffold;
- detection of broken internal references where feasible;
- basic repository hygiene checks;
- validation that no forbidden generated files are tracked.

> **Operational amendment (`RDR-0001`; NTK-MASTER, 17 July 2026):** Under the ratified decision `RDR-0001`, governance-document LaTeX compilation is retired from the required checks. Markdown governance integrity checks (structure, stable identifiers, internal links, and repository hygiene) replace it. The monograph-scaffold LaTeX build remains required. The broken-link, repository-hygiene, and forbidden-generated-file checks in the list above survive unchanged. A passing continuous-integration workflow establishes only that the configured checks passed; it is not scientific validation.

When Python infrastructure is authorized, checks shall expand to include:

- supported Python-version matrix;
- unit and integration tests;
- formatting and linting;
- static typing;
- coverage reporting used as a diagnostic, not a substitute for scientific testing;
- deterministic benchmark and reproducibility checks where computationally practical.

A passing continuous-integration workflow means only that the configured checks passed. It does not independently establish physical correctness.

## 24. Versioning and Release Doctrine

### 24.1 Version sequence

The project shall use semantic-style versioning for public milestones. Before full completion, versions remain below `1.0.0`.

The first foundation tag shall be:

```text
v0.1.0-foundation
```

Later milestone tags may identify literature, conventions, theory, software, validation, and release-candidate states. The exact number shall reflect repository history rather than a fixed calendar.

### 24.2 Meaning of Version 1.0.0

`v1.0.0` is reserved for satisfaction of the full completion criteria in the Scientific Constitution. A polished README, successful demonstration, or partial Kerr implementation is not sufficient.

### 24.3 Release record

Every scientific release shall include:

- scope and evidence level;
- included and excluded capabilities;
- known limitations;
- environment and reproducibility instructions;
- principal artifact hashes when appropriate;
- contributor record;
- comparison with the preceding release.

## 25. Conflict Resolution

Scientific disagreement shall be resolved through evidence, not authority alone. The preferred sequence is:

1. state the disagreement precisely;
2. identify the governing equation, assumption, benchmark, or policy;
3. consult primary or authoritative sources;
4. construct an analytical check or minimal numerical experiment when appropriate;
5. document the alternatives and consequences;
6. record the resolution in the relevant pull request or decision record.

If a critical disagreement remains unresolved, the conservative action is to block the merge, retain the previous ratified state, and mark the issue as blocked. Schedule pressure is not a valid reason to suppress a correctness concern.

Interpersonal or attribution disputes shall be handled privately first, then documented only to the extent necessary for a fair repository record. Neither collaborator may erase the other's valid contribution history.

## 26. Repository Launch Package

The initial public repository shall contain, at minimum:

1. an accurate root README with current phase and nonclaims;
2. the ratified Scientific Constitution;
3. the approved Project Governance and Repository Charter;
4. `AUTHORS.md` and `CONTRIBUTING.md`;
5. code and documentation licenses;
6. `CITATION.cff`;
7. the initial theory-first directory structure;
8. a monograph scaffold that builds cleanly;
9. pull-request and issue templates;
10. a master status record;
11. branch-protection and merge settings;
12. a clean repository state and a documented bootstrap history.

The launch package shall not contain fabricated numerical results, placeholder claims of validation, copied literature PDFs, or an empty Python package.

## 27. Gate 0B Exit Criteria

Gate 0B is complete only when all of the following hold:

1. The project and repository names are confirmed.
2. The repository is public and owned by Edgar Axel Pérez Flores.
3. The Scientific Constitution is stored with ratified status and current metadata.
4. This charter is approved and stored in the repository.
5. Naomi has either acknowledged the collaboration terms or is not yet publicly listed as an active repository collaborator pending acknowledgement.
6. The dual-license policy is implemented.
7. The root README accurately describes the foundation state.
8. The initial directory structure contains meaningful artifacts only.
9. The LaTeX build succeeds from a clean clone.
10. The default branch protections and merge policy are configured.
11. The first foundation pull request is reviewed and merged.
12. The repository has no uncommitted, untracked, secret, or generated-file pollution.
13. The annotated tag `v0.1.0-foundation` is created and points to the approved foundation state.
14. A Gate 0B closeout report is returned to the master orchestration record.

Only after these criteria are satisfied may the master project authorize Phase 1 as an active repository phase.

> **Operational amendment (`RDR-0001`; NTK-MASTER, 17 July 2026):** Criterion 9 now means the **clean-clone monograph-scaffold LaTeX build**, per the `RDR-0001` supersession of the governance-document compilation requirement; Markdown governance integrity checks are separately required. Naomi Sánchez Torres's collaboration-terms acknowledgement is complete, satisfying the acknowledgement branch of criterion 5, while her GitHub invitation acceptance remains pending and confers no inferred access. The remaining criteria must still be satisfied. Gate 0B is **not complete**. Phase 1 is not automatically activated by this charter or by `D0B-30`; `NTK-MASTER` must ratify the Gate 0B closeout and explicitly authorize Phase 1.

## 28. Gate 0B Decision Register

The following decisions are proposed for ratification with Version 0.1.0 of this charter:

| ID | Decision |
| --- | --- |
| D0B-01 | The public repository shall be named `from-newton-to-kerr`. |
| D0B-02 | The future Python package name is reserved as `newton_to_kerr`. |
| D0B-03 | The repository shall be public from its first formal foundation release. |
| D0B-04 | Edgar Axel Pérez Flores shall own and administer the repository. |
| D0B-05 | Naomi Sánchez Torres shall be the confirmed scientific collaborator and co-developer, subject to acknowledgement of the collaboration terms. |
| D0B-06 | The repository, not any external conversation, shall be the durable documentary source of truth. |
| D0B-07 | The initial repository shall be theory-first and shall not contain an empty production Python architecture. |
| D0B-08 | Direct pushes to `main` shall be prohibited after bootstrap. |
| D0B-09 | Squash merge shall be the default merge strategy. |
| D0B-10 | Critical scientific and implementation changes require independent review. |
| D0B-11 | Constitutional and publication-authority changes require a decision record and Edgar's final scientific sign-off. |
| D0B-12 | No collaborator may authorize attribution or publication on behalf of the other. |
| D0B-13 | The project shall maintain Scientific Decision Records and Repository Decision Records. |
| D0B-14 | AI tools may assist but shall have no independent scientific or authorship authority. |
| D0B-15 | Every AI-assisted substantive contribution remains the responsibility of its human submitter. |
| D0B-16 | Code shall use the MIT License. |
| D0B-17 | Original written material, figures, and project-generated datasets shall use Creative Commons Attribution 4.0 International by default. |
| D0B-18 | Copyrighted literature files shall not be distributed unless redistribution is permitted. |
| D0B-19 | The root README shall always display the current phase, gate, authorization state, and major nonclaims. |
| D0B-20 | GitHub milestones shall correspond to ratified gates rather than arbitrary calendar periods. |
| D0B-21 | The monograph LaTeX source is authoritative; generated PDFs are release artifacts. |
| D0B-22 | The initial automated quality gate shall include a reproducible LaTeX build. |
| D0B-23 | `v1.0.0` is reserved for full scientific completion under the Scientific Constitution. |
| D0B-24 | The first public milestone tag shall be `v0.1.0-foundation`. |
| D0B-25 | Specialized work sessions may propose findings but may not silently alter global scope. |
| D0B-26 | Unresolved critical disagreement blocks merge and preserves the prior ratified state. |
| D0B-27 | Repository secrets, private information, and improperly licensed material are prohibited. |
| D0B-28 | Large generated data shall remain outside Git history unless a later policy authorizes its inclusion. |
| D0B-29 | Publication author order remains deferred until contributions can be evaluated. |
| D0B-30 | Completion of Gate 0B authorizes Phase 1, not production numerical implementation. |

> **Register amendment note (`RDR-0001`; NTK-MASTER, 17 July 2026):** The register above remains historically frozen in its original wording and order; the introductory sentence preserves its historical "proposed for ratification" phrasing, and the substantive Charter was subsequently ratified. `D0B-21` is reaffirmed without change. `D0B-22` survives with its LaTeX-build referent narrowed by `RDR-0001` to the monograph-scaffold build; its historical wording is untouched. `D0B-30` records the intended transition after Gate 0B but does not itself activate Phase 1: activation requires the Gate 0B closeout to be ratified by `NTK-MASTER` and Phase 1 to be explicitly authorized by `NTK-MASTER`. `RDR-0001` does not silently rewrite any `D0B` row.

## 29. Immediate Next Authorized Work

Upon approval of this charter, the next authorized work is a dedicated repository-foundation session with the objective:

> Create, configure, verify, and release the public `from-newton-to-kerr` repository in strict accordance with the Gate 0B launch package and exit criteria.

The repository-foundation session may:

- initialize the repository;
- create the approved files and directory structure;
- configure licenses, templates, branch protection, and LaTeX build checks;
- update the Scientific Constitution from draft metadata to ratified metadata;
- prepare and merge the foundation pull request;
- create the foundation tag and closeout record.

It may not:

- begin production physics code;
- introduce unratified scientific scope;
- fabricate benchmark results;
- pre-empt Phase 1 literature conclusions;
- assign the complete module-level division of work without later review.

> **Operational note (`RDR-0001`; NTK-MASTER, 17 July 2026):** The repository-foundation session described above is currently in progress. Repository creation, bootstrap, protection configuration, and the governance transposition work do not by themselves close Gate 0B. Phase 1 and production Python work remain blocked. Only the complete Gate 0B closeout, its ratification by `NTK-MASTER`, and `NTK-MASTER`'s explicit authorization can activate Phase 1.

## Approval Status

**Current status:** Gate 0B foundational draft for scientific-owner review and collaborator acknowledgement.

**Approval effect:** Edgar's ratification authorizes the dedicated public-repository foundation session. Naomi's acknowledgement is required before she is represented as having accepted the collaboration obligations or before substantive collaborative work is attributed to her under this charter.

**Scientific authorization after approval:** Repository foundation only. Phase 1 becomes active only after all Gate 0B exit criteria are satisfied. Production numerical implementation remains blocked.

> **Amendment note (`RDR-0001`; NTK-MASTER, 17 July 2026):** The three statements above are preserved verbatim from the ratified LaTeX source, whose declared source state is `Gate 0B Foundational Draft` dated 16 July 2026. The substantive Charter was subsequently ratified, and that ratified state is recorded in the master project record and in the metadata table of this file. Naomi Sánchez Torres has acknowledged the collaboration terms and is the confirmed Scientific Collaborator and Co-developer; a GitHub collaborator invitation has been sent to her, but acceptance and active repository access remain pending. Gate 0B remains in progress. This Markdown representation remains an authorized draft with no adopted canonical authority. Phase 1 remains blocked, and production numerical implementation remains blocked. This note changes no scientific substance.

| Edgar Axel Pérez Flores | Naomi Sánchez Torres |
| --- | --- |
| Scientific Lead and Repository Owner | Scientific Collaborator and Co-developer |
