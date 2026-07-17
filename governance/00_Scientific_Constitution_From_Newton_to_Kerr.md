# Scientific Constitution for From Newton to Kerr

*Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics*

| Field | Value |
| --- | --- |
| Document | Scientific Constitution for From Newton to Kerr |
| Scientific subtitle | Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics |
| Source version | 0.1.0 |
| Source date | 16 July 2026 |
| Declared source-state wording | `Phase 0 Foundational Draft` |
| Substantive governance state | RATIFIED |
| Transposition state | AUTHORIZED DRAFT |
| Canonical authority | NOT YET EFFECTIVE |
| Related repository decision | `RDR-0001` — RATIFIED |
| Source filename | `00_Scientific_Constitution_From_Newton_to_Kerr.tex` |
| Source SHA-256 | `6ac268e9d4772a8c6ff0a9a5d5c53752571126ea925b873f6907c3ee0d16bc46` |
| Scientific Lead and final signatory | Edgar Axel Pérez Flores |
| Scientific Collaborator and Co-developer | Naomi Sánchez Torres |
| Governing workstream | `[NTK-P00B]` Repository and Collaboration Foundation |

## Canonical-Format Amendment Note

This note is a format-governance notice authorized by `RDR-0001`. It is placed outside the frozen historical decision register and changes no scientific or governance substance.

- The substantive Scientific Constitution was already **ratified**; that ratification is recorded in the master project record and is presupposed, not re-performed, by this file.
- This file is an authorized Markdown transposition prepared to preserve the complete rendered substantive content of the ratified LaTeX source `00_Scientific_Constitution_From_Newton_to_Kerr.tex` under the ratified repository decision `RDR-0001`. Its semantic fidelity remains subject to the required human comparison, independent collaborator review, and final scientific sign-off.
- The canonical-format transition is **not yet effective**. This file has no adopted canonical authority merely because it exists.
- Until protected-`main` adoption, the original LaTeX input remains the **current ratified source representation** and an **immutable provenance input**, identified byte-exactly in `governance/provenance/ORIGINAL_RATIFICATION_INPUTS.md`.
- After protected-`main` adoption under the conditions of `RDR-0001`, this Markdown file becomes the **canonical repository governance instrument**, and the LaTeX source remains provenance evidence only, with no authority to override, reinterpret, or amend the Markdown canon.
- The historical Phase 0 decision register (`D0-01` through `D0-17`) is preserved below in its original wording, order, and historical meaning. It has not been retroactively rewritten.
- The historical authorization language in Section 20 and Approval Status is preserved verbatim, but it does not activate Phase 1 under the current repository-governance sequence. Phase 1 remains blocked until Gate 0B is fully completed, its closeout is ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1. Production Python work remains blocked.
- No scientific or governance substance is changed by this transposition. Any substantive divergence from the ratified source is by definition a conversion defect and must be corrected against the original.

## Abstract

This document defines the scientific identity, mandatory scope, theoretical doctrine, computational standards, validation requirements, publication architecture, and completion criteria of From Newton to Kerr. The project is conceived as a clean-start, Python-based study of orbital dynamics whose central purpose is to connect classical inverse-square motion, Hamiltonian mechanics, geometric numerical integration, nonlinear dynamics, weak-field relativistic corrections, and geodesic motion in Schwarzschild and Kerr spacetimes within a single invariant-driven framework. The project is not a collection of visual demonstrations, a generic $N$-body engine, or a numerical-relativity code. Its authority derives from explicit assumptions, complete derivations, model-appropriate numerical methods, analytical and convergence benchmarks, reproducible computational evidence, and carefully delimited public claims. This constitution is the controlling Phase 0 document. Later theory, software, figures, datasets, and publication materials must remain consistent with it or formally amend it through a recorded scientific decision.

## Contents

- [Canonical-Format Amendment Note](#canonical-format-amendment-note)
- [Abstract](#abstract)
- [1. Purpose and Authority of This Constitution](#1-purpose-and-authority-of-this-constitution)
- [2. Project Identity](#2-project-identity)
  - [2.1 Formal identity](#21-formal-identity)
  - [2.2 Positioning statement](#22-positioning-statement)
  - [2.3 Strategic academic objective](#23-strategic-academic-objective)
- [3. Central Scientific Thesis](#3-central-scientific-thesis)
- [4. Research Questions and Working Hypotheses](#4-research-questions-and-working-hypotheses)
  - [4.1 Primary research questions](#41-primary-research-questions)
  - [4.2 Working hypotheses](#42-working-hypotheses)
- [5. Mandatory Scientific Spine](#5-mandatory-scientific-spine)
  - [5.1 M1: Kepler problem and central-force foundations](#51-m1-kepler-problem-and-central-force-foundations)
  - [5.2 M2: Geometric numerical integration laboratory](#52-m2-geometric-numerical-integration-laboratory)
  - [5.3 M3: Circular restricted three-body problem](#53-m3-circular-restricted-three-body-problem)
  - [5.4 M4: First post-Newtonian test-particle bridge](#54-m4-first-post-newtonian-test-particle-bridge)
  - [5.5 M5: Schwarzschild geodesic dynamics](#55-m5-schwarzschild-geodesic-dynamics)
  - [5.6 M6: Kerr geodesic dynamics](#56-m6-kerr-geodesic-dynamics)
  - [5.7 M7: Curated relativistic orbit atlas](#57-m7-curated-relativistic-orbit-atlas)
- [6. Explicit Exclusions and Nonclaims](#6-explicit-exclusions-and-nonclaims)
- [7. Global Mathematical and Physical Conventions](#7-global-mathematical-and-physical-conventions)
  - [7.1 Relativistic conventions](#71-relativistic-conventions)
  - [7.2 Units and nondimensionalization](#72-units-and-nondimensionalization)
  - [7.3 Initial-value formulation](#73-initial-value-formulation)
- [8. Theory-First Development Doctrine](#8-theory-first-development-doctrine)
  - [8.1 Theory-readiness gate](#81-theory-readiness-gate)
- [9. Physics-to-Software Contract](#9-physics-to-software-contract)
- [10. Numerical Doctrine](#10-numerical-doctrine)
  - [10.1 Model-appropriate integration](#101-model-appropriate-integration)
  - [10.2 Error observables](#102-error-observables)
  - [10.3 No universal tolerance](#103-no-universal-tolerance)
  - [10.4 Singularities and coordinate boundaries](#104-singularities-and-coordinate-boundaries)
- [11. Validation and Evidence Doctrine](#11-validation-and-evidence-doctrine)
  - [11.1 Evidence hierarchy](#111-evidence-hierarchy)
  - [11.2 Required validation layers](#112-required-validation-layers)
  - [11.3 Classification validation](#113-classification-validation)
- [12. Product Architecture](#12-product-architecture)
  - [12.1 Comprehensive technical monograph](#121-comprehensive-technical-monograph)
  - [12.2 Python repository](#122-python-repository)
  - [12.3 Preprint-style paper](#123-preprint-style-paper)
  - [12.4 Public datasets and figures](#124-public-datasets-and-figures)
- [13. Writing and Communication Standard](#13-writing-and-communication-standard)
- [14. Publication and Novelty Doctrine](#14-publication-and-novelty-doctrine)
- [15. Project Phases and Hard Dependencies](#15-project-phases-and-hard-dependencies)
- [16. Collaboration Boundary for Phase 0](#16-collaboration-boundary-for-phase-0)
- [17. Risk and Feasibility Control](#17-risk-and-feasibility-control)
  - [17.1 Scope inflation](#171-scope-inflation)
  - [17.2 Theory without completion](#172-theory-without-completion)
  - [17.3 Code without scientific authority](#173-code-without-scientific-authority)
  - [17.4 Visual-first bias](#174-visual-first-bias)
  - [17.5 Unfounded publication expectations](#175-unfounded-publication-expectations)
- [18. Definition of Full Project Completion](#18-definition-of-full-project-completion)
- [19. Phase 0 Decision Register](#19-phase-0-decision-register)
- [20. Immediate Next Authorized Work](#20-immediate-next-authorized-work)
- [Approval Status](#approval-status)

## 1. Purpose and Authority of This Constitution

This constitution establishes the binding scientific doctrine of From Newton to Kerr. Its function is not to provide all derivations or implementation details. Its function is to determine what the project is, what it is not, what must be completed, what evidence is required, and in what order the work may advance.

The constitution governs four authoritative project products:

1. a comprehensive LaTeX technical monograph;
2. a validated and reproducible Python scientific repository;
3. a curated body of figures, benchmark tables, and orbit-classification datasets;
4. a concise preprint-style paper suitable in form and technical standard for public dissemination and potential submission to arXiv.

Any future change to the scientific thesis, mandatory model set, conventions, validation requirements, or publication claims must be recorded in a versioned decision register. Silent scope expansion is prohibited.

## 2. Project Identity

### 2.1 Formal identity

**Project name:** From Newton to Kerr

**Scientific subtitle:** Hamiltonian Structure, Numerical Fidelity, and Relativistic Orbital Dynamics

**Primary implementation language:** Python only

**Primary written language:** English only

**Scientific domain:** analytical mechanics, Hamiltonian systems, nonlinear dynamics, numerical analysis, scientific computing, and general-relativistic test-particle dynamics

**Core collaborators:** Edgar Axel Pérez Flores and Naomi Sánchez Torres

### 2.2 Positioning statement

The project shall be presented as:

> A theory-first computational physics study of how symmetries, invariants, phase-space structure, and numerical reliability evolve across a controlled hierarchy of orbital models, from the Kepler problem to geodesic motion in Kerr spacetime.

The project shall not be presented as a general-purpose astrophysical simulator, a full numerical-relativity calculation, or evidence of new relativistic phenomena unless a later literature and novelty audit supports a more specific claim.

### 2.3 Strategic academic objective

The project shall demonstrate independent command of advanced theoretical and computational physics at a level appropriate for a strong transition from undergraduate engineering physics toward graduate study in theoretical physics. It must provide visible evidence of competence in:

- variational, Lagrangian, and Hamiltonian mechanics;
- dynamical systems, integrability, and chaos;
- numerical ODE integration and geometric numerical analysis;
- dimensional analysis and nondimensionalization;
- general-relativistic geodesic dynamics;
- reproducible scientific software and evidence-based validation;
- technical writing in strong academic English.

This academic objective does not replace the scientific objective. The project must remain scientifically coherent even when read by a person who has no knowledge of the authors' CVs.

## 3. Central Scientific Thesis

The provisional central thesis is:

> Orbital dynamics from Newtonian gravity to Kerr geodesics can be studied within a coherent Hamiltonian and invariant-driven framework in which the credibility of every numerical result is determined jointly by the physical model, its symmetries and constraints, the geometry of phase space, the integration method, and explicit convergence and classification evidence.

The project therefore follows the chain

$$
\text{physical model}
\longrightarrow
\text{variational or Hamiltonian structure}
\longrightarrow
\text{symmetries and invariants}
\longrightarrow
\text{numerical representation}
\longrightarrow
\text{validation}
\longrightarrow
\text{orbit classification}.
$$

The scientific value of the project will not be measured by the number of implemented models. It will be measured by the depth and traceability of this chain.

## 4. Research Questions and Working Hypotheses

### 4.1 Primary research questions

- **RQ1.** How do symmetries, first integrals, and phase-space structure organize orbital motion across the Kepler, circular restricted three-body, post-Newtonian, Schwarzschild, and Kerr models?
- **RQ2.** How do model-appropriate numerical integrators differ in long-time phase, invariant, and constraint fidelity, and which diagnostics most reliably distinguish a physical dynamical effect from a numerical artifact?
- **RQ3.** Under what controlled limits do Newtonian, first post-Newtonian, and Schwarzschild orbital predictions agree, and how can the transition between these regimes be demonstrated numerically without conflating approximation error and integration error?
- **RQ4.** How do black-hole spin, orbital orientation, and the Carter constant reshape accessible regions, turning-point structure, and orbit classes in Kerr spacetime?
- **RQ5.** Can mathematically explicit, invariant-aware, and event-based criteria produce reproducible orbit-classification maps that remain stable under numerical refinement?

### 4.2 Working hypotheses

The following hypotheses guide the design but are not public conclusions until validated:

- **H1.** For separable classical Hamiltonians, structure-preserving methods will exhibit bounded long-time invariant error more consistently than standard explicit methods at comparable computational cost, although no method will be declared universally superior.
- **H2.** In the weak-field and slow-motion regime, first post-Newtonian and Schwarzschild results will converge toward Newtonian predictions in a manner consistent with the chosen expansion parameter and numerical tolerances.
- **H3.** Kerr spin will produce quantitatively distinct prograde and retrograde orbital boundaries and precessional behavior consistent with known analytical limits.
- **H4.** Orbit classifications based on effective potentials, turning points, horizon or escape events, and conserved-quantity diagnostics will be more reproducible than labels assigned from trajectory appearance alone.

## 5. Mandatory Scientific Spine

The project adopts a gravitational and Hamiltonian spine. Every mandatory module must support the central thesis and create a necessary dependency for later work.

### 5.1 M1: Kepler problem and central-force foundations

The first mandatory model is the Newtonian two-body problem reduced to relative motion. It shall include:

- center-of-mass reduction and reduced mass;
- effective radial dynamics;
- bound and unbound conic sections;
- energy, angular momentum, and Runge–Lenz structure;
- circular and eccentric orbit benchmarks;
- scattering and turning-point analysis;
- dimensional and dimensionless formulations.

The Coulomb problem may appear as a mathematically parallel example or appendix, but it is not a separate mandatory production module. This decision preserves conceptual breadth without weakening the gravitational narrative.

### 5.2 M2: Geometric numerical integration laboratory

The Kepler model shall be used to establish the numerical doctrine. Required methods include:

- classical fourth-order Runge–Kutta as a transparent explicit baseline;
- a high-order adaptive SciPy solver as a reference method;
- symplectic Euler;
- Störmer–Verlet or leapfrog splitting where the Hamiltonian is separable;
- at least one time-reversible or implicit reference method if justified by the final computational specification.

Required comparisons include observed order, phase error, invariant error, reversibility, computational cost, and long-time qualitative fidelity.

### 5.3 M3: Circular restricted three-body problem

The circular restricted three-body problem is the mandatory nonlinear and nonintegrable bridge. It shall include:

- rotating-frame equations and effective potential;
- Jacobi integral;
- Lagrange points and local stability;
- Hill regions and zero-velocity curves;
- event-based Poincaré sections;
- selected finite-time chaos indicators;
- transit, bounded, escape, and collision-related regimes.

A generic arbitrary-$N$ Newtonian engine is not required for the first complete release. This exclusion prevents a large software branch from competing with the central relativistic goal.

### 5.4 M4: First post-Newtonian test-particle bridge

The project shall implement one carefully sourced first post-Newtonian model for a test particle in a central gravitational field. The formulation must be chosen to connect cleanly with the weak-field expansion of Schwarzschild dynamics. Required outputs include:

- derivation or documented derivational chain;
- domain of validity in powers of $v/c$ and $GM/(rc^2)$;
- numerical recovery of periapsis precession;
- comparison with the analytical leading-order precession;
- explicit Newtonian-limit tests;
- comparison with Schwarzschild results in an overlapping regime.

The project shall not implement a general relativistic two-body post-Newtonian hierarchy in the first release.

### 5.5 M5: Schwarzschild geodesic dynamics

The Schwarzschild module shall treat timelike and null geodesics. Because spherical symmetry permits planar reduction, the equatorial representation is sufficient without loss of generality for the orbital plane. Mandatory content includes:

- metric, action or Hamiltonian, and constants of motion;
- normalization constraint;
- radial effective potentials and turning points;
- circular-orbit conditions and stability;
- photon sphere and innermost stable circular orbit benchmarks;
- bound, scattering, capture, plunge, and zoom–whirl examples;
- weak-field comparison with Newtonian and first post-Newtonian motion.

### 5.6 M6: Kerr geodesic dynamics

Kerr is the culminating mandatory model. Development shall proceed in two controlled stages:

- (a) equatorial timelike and null geodesics, used to validate spin-dependent circular-orbit, capture, and prograde–retrograde behavior;
- (b) selected generic geodesics using the Carter constant and separated radial and polar dynamics.

The generic stage is mandatory for full project completion because it demonstrates genuine understanding of Kerr integrability beyond equatorial visualization. However, it shall use a curated set of representative families and low-dimensional parameter slices rather than an unbounded search of the full initial-condition space.

### 5.7 M7: Curated relativistic orbit atlas

The final atlas shall be scientifically curated rather than maximally large. Mandatory atlas products are:

- Schwarzschild classification maps in conserved-quantity or turning-point variables;
- equatorial Kerr maps at selected spin values;
- selected generic Kerr slices in $(\mathcal{E},L_z,Q)$ at fixed dimensionless spin;
- representative trajectories for every declared class;
- convergence and invariant metadata linked to each production result.

A brute-force seven-dimensional atlas over all initial data is explicitly rejected as neither necessary nor proportionate for the first complete project.

## 6. Explicit Exclusions and Nonclaims

The following are outside the mandatory scope:

- legacy MATLAB preservation, migration, or comparison;
- a generic production-level arbitrary-$N$ body engine;
- self-consistent relativistic many-body gravity;
- numerical solution of the Einstein field equations;
- binary black-hole numerical relativity;
- gravitational radiation reaction or waveform generation;
- magnetohydrodynamics, accretion-disk physics, or radiative transfer;
- full observational ray tracing;
- astrophysical parameter inference;
- claims of discovering a new relativistic effect;
- claims that one numerical method is universally superior;
- claims that visually plausible trajectories are physically validated.

Optional extensions may be considered only after the complete mandatory spine has reached publication-grade evidence.

## 7. Global Mathematical and Physical Conventions

### 7.1 Relativistic conventions

Unless formally amended, the project shall use:

- metric signature $(-,+,+,+)$;
- explicit $G$ and $c$ in primary theoretical derivations;
- Greek indices for spacetime components and Latin indices for spatial components when ambiguity is possible;
- Einstein summation only after it has been declared in the relevant chapter;
- proper time $\tau$ for timelike geodesics;
- an affine parameter $\lambda$ for null geodesics;
- Mino time only as a derived computational parameter for generic Kerr motion, with the mapping to physical or affine parameters retained;
- Kerr dimensional spin parameter

  $$
  a=\frac{J}{Mc},
  $$

  and dimensionless spin

  $$
  \chi=\frac{cJ}{GM^2}=\frac{ac^2}{GM},
  \qquad |\chi|\leq 1
  $$

  for the black-hole domain considered by the project.

### 7.2 Units and nondimensionalization

Geometric units may be used in solver equations only after the dimensional theory and the mapping to solver variables have been written explicitly. Every model shall provide:

1. dimensional variables and constants;
2. characteristic length, time, mass, and momentum scales;
3. dimensionless variables;
4. dimensionless evolution equations;
5. a reversible mapping between stored numerical results and physical units.

Setting $G=c=M=1$ without this mapping is prohibited in the monograph and production metadata.

### 7.3 Initial-value formulation

Every model shall define admissible initial data in one or more of the following forms:

- coordinates and velocities;
- coordinates and canonical momenta;
- conserved quantities plus phase information;
- turning-point or orbital-element data.

Constraint equations, branch choices, sign conventions, and physically forbidden states must be explicit. Initial conditions that violate a model constraint shall be rejected rather than silently corrected.

## 8. Theory-First Development Doctrine

No production physics module may be implemented before its theoretical package is complete. Each mandatory theoretical chapter shall contain:

1. physical problem and motivation;
2. assumptions and domain of validity;
3. configuration and phase spaces;
4. action, Lagrangian, or Hamiltonian;
5. complete derivation of the governing equations;
6. symmetries, constraints, and conserved quantities;
7. dimensional analysis and nondimensionalization;
8. initial-value formulation;
9. analytical limits or exact benchmark solutions;
10. singularities, coordinate pathologies, and admissible events;
11. numerical observables and classification criteria;
12. validation targets;
13. scientific nonclaims;
14. literature provenance.

Short Python or symbolic scripts may be used during theoretical development to verify algebra, limits, derivatives, tensor identities, or series expansions. Such scripts are verification instruments, not production solvers.

### 8.1 Theory-readiness gate

A module is theory-ready only when:

- all symbols are defined;
- equations are dimensionally consistent;
- assumptions and validity limits are explicit;
- the numerical state is identifiable;
- initial data can be constructed without hidden choices;
- invariants and constraints are defined;
- benchmark values or limiting cases are registered;
- event and classification conditions are mathematically stated;
- references are verified;
- an independent review finds no unresolved foundational contradiction.

## 9. Physics-to-Software Contract

The theory-to-code transition shall occur through a written computational contract for each model. A contract must define at least:

- model identifier and theory source;
- state vector and independent variable;
- right-hand side or Hamiltonian flow;
- parameter set and units;
- initial-data constructors;
- constraints and invariants;
- valid numerical methods;
- event functions and termination rules;
- classification logic;
- analytical and literature benchmarks;
- metadata and serialization requirements;
- expected failure states.

No code implementation may silently reinterpret a symbol, change a model equation, soften a singularity, or alter an event threshold relative to its contract.

## 10. Numerical Doctrine

### 10.1 Model-appropriate integration

The project rejects the idea that one integrator must be used for every model.

For separable Newtonian Hamiltonians, explicit symplectic splitting methods shall be compared with conventional and adaptive Runge–Kutta methods. For nonseparable relativistic Hamiltonians, a high-order adaptive method may serve as the primary reference, provided that constraints and invariants are monitored. Implicit midpoint, Hamiltonian splitting, or other geometric methods may be added only when their formulation and solver behavior are independently validated.

The project shall never label a method “symplectic” merely because it behaves well in a plot. The mathematical map must satisfy the relevant structural definition.

### 10.2 Error observables

Where applicable, every numerical study shall measure:

$$
\begin{aligned}
\Delta E(t) &= E(t)-E(0),\\
\Delta L(t) &= L(t)-L(0),\\
\Delta C(t) &= C(t)-C(0),
\end{aligned}
$$

where $C$ denotes an appropriate constraint or additional first integral. The reported metric may be absolute, relative, normalized, or component-wise, but its definition must be explicit.

Additional observables shall include, when relevant:

- phase error;
- trajectory error against an exact or reference solution;
- observed convergence order;
- time-reversal error;
- turning-point displacement;
- event-time error;
- classification stability under refinement;
- computational cost.

### 10.3 No universal tolerance

No single global invariant tolerance shall be imposed on all models. Tolerances must be frozen per benchmark before production results are generated. They must be justified by resolution, method order, integration duration, floating-point precision, and the scientific quantity being measured.

### 10.4 Singularities and coordinate boundaries

The project shall not silently regularize singular forces or coordinate boundaries. Allowed responses include:

- mathematically defined event termination;
- a documented coordinate transformation;
- an analytically justified regularization;
- a separate modified model whose physical meaning is explicitly stated.

Numerical clipping without a model declaration is prohibited.

## 11. Validation and Evidence Doctrine

### 11.1 Evidence hierarchy

Every result shall carry one of the following evidence states:

- **E0 — Derived.** The equations and assumptions are documented, but no implementation claim is enabled.
- **E1 — Implemented.** The code exists and passes local unit tests, but scientific accuracy is not yet established.
- **E2 — Benchmark validated.** The implementation reproduces one or more analytical or trusted reference benchmarks within frozen tolerances.
- **E3 — Convergence validated.** Resolution or tolerance studies establish the expected convergence behavior and rule out a single-resolution coincidence.
- **E4 — Production authorized.** The model, configuration, metadata, and classification logic are approved for project results.
- **E5 — Publication grade.** The result is reproducible from a clean environment, independently reviewed, fully traceable, and suitable for the monograph or preprint.

Only E5 results may appear as primary scientific evidence in the final preprint.

### 11.2 Required validation layers

1. symbolic or algebraic checks where appropriate;
2. unit tests for formulas and transformations;
3. analytical benchmark recovery;
4. convergence studies with at least three resolutions when meaningful;
5. cross-method or cross-formulation comparison;
6. long-time invariant or constraint monitoring;
7. regression tests for trusted results;
8. clean-environment reproducibility.

### 11.3 Classification validation

An orbit class is valid only if:

- its mathematical definition is explicit;
- event and tolerance rules are frozen;
- the class is stable under a declared refinement study;
- invariants or constraints remain within the accepted evidence envelope;
- ambiguous and unresolved cases are retained as such rather than forced into a label.

## 12. Product Architecture

### 12.1 Comprehensive technical monograph

The monograph is the complete scientific record. It shall contain the full theoretical, mathematical, numerical, computational, and validation development. It has no artificial page limit. Its purpose is completeness and traceability, not journal compression.

The provisional structure is:

- **Part I:** Scientific and Mathematical Foundations
- **Part II:** Classical Integrable and Nonintegrable Dynamics
- **Part III:** Post-Newtonian and Relativistic Orbital Dynamics
- **Part IV:** Computational Methodology and Validation
- **Part V:** Scientific Results and Orbit Atlas
- **Part VI:** Synthesis, Limitations, and Future Work

Detailed derivations, symbolic identities, benchmark tables, and extended convergence studies may be placed in appendices without being removed from the authoritative record.

### 12.2 Python repository

The repository shall contain the authoritative executable implementation. Notebooks may support exploration and tutorials, but production equations, diagnostics, events, and classifications must live in importable modules under a modern `pyproject.toml`-based package.

All public-facing repository content shall be written in English, including README files, documentation, docstrings, scientific comments, figure labels, captions, tables, issue templates, and pull-request descriptions.

### 12.3 Preprint-style paper

The final paper shall not be a shortened copy of every monograph chapter. It shall defend one coherent central contribution supported by selected results. The target is approximately 18–22 pages of main scientific narrative, with bibliography and technical appendices excluded from the target when necessary.

A provisional title is:

> *From Newton to Kerr: Invariant-Driven Numerical Dynamics and Reproducible Orbit Classification*

The title, contribution claim, and paper structure shall remain provisional until the literature and novelty audit and the first production results are complete.

### 12.4 Public datasets and figures

Every public figure or dataset must be reproducible from a versioned configuration and must store or expose:

- software version or commit;
- Python and dependency environment;
- physical and dimensionless parameters;
- initial conditions;
- integrator and tolerance settings;
- termination reason;
- invariant or constraint diagnostics;
- classification and evidence state.

## 13. Writing and Communication Standard

All formal project materials shall use strong academic English. The minimum target is equivalent to IELTS Academic Band 7, with an aspirational standard of Band 7.5–8.0 for the monograph, preprint, and main public documentation.

The writing shall prioritize:

- precise claims;
- explicit assumptions;
- complete sentences and coherent transitions;
- consistent notation;
- restrained use of jargon;
- distinction between derivation, observation, interpretation, and speculation;
- captions that explain the scientific content of a figure rather than merely naming it.

Inflated claims, vague adjectives, and portfolio-oriented language shall not appear in the scientific paper. Scientific quality must be visible from the work itself.

## 14. Publication and Novelty Doctrine

The project is authorized to claim, once validated:

- a transparent implementation of established classical and relativistic orbital models;
- a consistent invariant-driven validation framework;
- reproducible comparisons across Newtonian, post-Newtonian, Schwarzschild, and Kerr regimes;
- mathematically explicit orbit-classification procedures;
- open educational and scientific software of demonstrable technical depth.

The project is not authorized to claim new physics, a new spacetime solution, a new relativistic phenomenon, or a universally superior algorithm without a dedicated literature comparison and specific evidence.

Potential publication value may arise from methodological synthesis, unusually transparent validation, a reproducible cross-regime comparison, a curated classification atlas, or a novel combination of these elements. The final claim shall be chosen after the evidence exists.

## 15. Project Phases and Hard Dependencies

| Phase | Name | Required outcome |
| --- | --- | --- |
| 0 | Scientific Constitution | Approved thesis, scope, questions, exclusions, products, standards, and completion criteria. |
| 1 | Literature and Benchmark Cartography | Verified source map, equation provenance, benchmark registry, and novelty audit. |
| 2 | Global Conventions | Frozen notation, units, dimensional maps, coordinate conventions, and initial-value doctrine. |
| 3 | Complete Theoretical Development | Theory-ready chapters for every mandatory model. |
| 4 | Computational Specification | Physics-to-software contracts, benchmark tolerances, event logic, and metadata standards. |
| 5 | Python Infrastructure | Package, tests, typing, linting, continuous integration, configuration, and reproducibility foundation. |
| 6 | Sequential Implementation | Model implementation in dependency order from Kepler to Kerr. |
| 7 | Validation Campaigns | E2–E4 evidence for all mandatory models and E5 evidence for final results. |
| 8 | Scientific Results | Approved comparative studies, curated orbit maps, and final figures. |
| 9 | Monograph Freeze | Integrated and internally consistent theory, methods, evidence, and results. |
| 10 | Preprint and Public Release | Concise paper, clean-clone reproducibility, release archive, and public repository. |

The following dependency rules are mandatory:

- no production model code before the scientific constitution and literature map;
- no implementation before the relevant theory-readiness gate;
- no parameter sweep before single-trajectory convergence and event validation;
- no Kerr production study before Schwarzschild and the Kerr limiting cases pass;
- no flagship visualization before the underlying result reaches E4;
- no preprint figure before the underlying result reaches E5;
- no public novelty claim before the literature audit is complete.

## 16. Collaboration Boundary for Phase 0

Edgar Axel Pérez Flores is the scientific lead and primary theoretical author. He shall retain final responsibility for the consistency of the hard theoretical framework, public scientific claims, and the relation between derivation and implementation.

Naomi Sánchez Torres is the confirmed scientific collaborator and co-developer. She shall have a substantive role in the computational realization, review, validation, and documentation of the project.

The exact division of modules, code ownership, chapter authorship, review duties, and author order is intentionally not fixed by this constitution. Those decisions require a separate collaboration charter after the scientific work breakdown and dependency graph are approved.

Regardless of the later division, every critical physics module shall have:

- one primary author or implementer;
- one independent reviewer;
- a documented resolution of scientific disagreements;
- preserved contribution records.

## 17. Risk and Feasibility Control

### 17.1 Scope inflation

The main risk is not insufficient ambition but uncontrolled breadth. The following controls are adopted:

- a generic $N$-body engine is excluded;
- Coulomb dynamics is secondary rather than a parallel project branch;
- the relativistic atlas uses curated slices rather than exhaustive high-dimensional searches;
- optional advanced integrators are blocked until the baseline methods are validated;
- new physical modules require a formal scope amendment.

### 17.2 Theory without completion

A second risk is producing an extensive theoretical document without reaching validated code. To prevent this, the theory shall be developed in model packages, each ending in a physics-to-software contract and benchmark registry. A chapter is not complete merely because its derivation is long.

### 17.3 Code without scientific authority

A third risk is implementing equations whose assumptions, branches, or constraints are unclear. No such implementation may advance beyond E1.

### 17.4 Visual-first bias

Animations and three-dimensional trajectories may be created for internal exploration, but they shall not become flagship outputs until classification, convergence, and invariant evidence are available.

### 17.5 Unfounded publication expectations

The project shall be developed to arXiv-ready technical standards. Whether it should actually be submitted as a preprint will be decided only after the novelty audit, full internal review, and completion of publication-grade results.

## 18. Definition of Full Project Completion

The project is complete only when all of the following conditions hold:

1. The scientific constitution and decision register are current.
2. The literature map and equation-provenance registry are complete.
3. The comprehensive monograph contains the full derivational and computational record.
4. Every mandatory model has a physics-to-software contract.
5. The Python package installs and runs from a clean environment.
6. All mandatory analytical benchmarks pass within frozen tolerances.
7. Convergence and invariant evidence exist for every primary result.
8. Schwarzschild and Kerr limiting cases are recovered.
9. Generic Kerr motion includes verified Carter-constant behavior.
10. The curated orbit atlas is reproducible and contains explicit unresolved states.
11. Figures and datasets contain complete metadata.
12. The final preprint presents one coherent contribution without unsupported claims.
13. Both collaborators have reviewed the scientific and computational record.
14. A versioned public release can regenerate every principal result.

A visually polished repository without these conditions is not considered a completed project.

## 19. Phase 0 Decision Register

The following decisions are frozen by Version 0.1.0 of this constitution:

| ID | Decision |
| --- | --- |
| D0-01 | The project is a clean-start Python project; the former MATLAB work is outside scope. |
| D0-02 | The scientific spine is gravitational, Hamiltonian, and invariant-driven. |
| D0-03 | Coulomb dynamics is optional supporting material, not a mandatory production branch. |
| D0-04 | A generic arbitrary-$N$ body engine is excluded from the first complete release. |
| D0-05 | The CR3BP is the mandatory nonlinear and chaotic classical model. |
| D0-06 | The post-Newtonian bridge is a single carefully sourced test-particle 1PN model. |
| D0-07 | Schwarzschild timelike and null geodesics are mandatory. |
| D0-08 | Kerr equatorial and selected generic geodesics are mandatory for full completion. |
| D0-09 | The relativistic atlas will use curated low-dimensional slices, not an exhaustive high-dimensional sweep. |
| D0-10 | The project will use model-appropriate integrators rather than a universal solver. |
| D0-11 | No production implementation may precede theory readiness and a computational contract. |
| D0-12 | The full monograph has no artificial page limit. |
| D0-13 | The final preprint will target approximately 18–22 pages of main narrative. |
| D0-14 | All formal artifacts will be written in strong academic English. |
| D0-15 | The exact division of work between Edgar and Naomi is deferred to a separate collaboration charter. |
| D0-16 | Only E5 results may serve as primary evidence in the final preprint. |
| D0-17 | arXiv-ready quality is mandatory; actual submission remains evidence-dependent. |

## 20. Immediate Next Authorized Work

Upon approval of this constitution, the next authorized phase is:

> **Phase 1 — Literature and Benchmark Cartography**

Its first deliverables shall be:

1. a source-quality policy;
2. a chapter-by-chapter literature map;
3. an equation-provenance registry;
4. an analytical benchmark registry;
5. a preliminary novelty and publication-positioning audit;
6. a bibliography architecture for the monograph and preprint.

No production solver implementation is authorized by this Phase 0 document.

> **Operational amendment (`RDR-0001`; NTK-MASTER, 17 July 2026):** The Phase 1 authorization language above is preserved as part of the historical ratified source. Under the current repository-governance sequence, Phase 1 remains blocked until Gate 0B is fully completed, its closeout is ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1. Production Python architecture and implementation remain blocked.

## Approval Status

**Current status:** Foundational draft for scientific-owner review.

**Approval effect:** Approval freezes the scientific identity and mandatory scope defined above and authorizes Phase 1. It does not yet authorize production implementation or assign the module-level division of work.

> **Amendment note (`RDR-0001`; NTK-MASTER, 17 July 2026):** The two statements above are preserved verbatim from the ratified LaTeX source, whose declared source state is `Phase 0 Foundational Draft` dated 16 July 2026. The substantive Constitution was subsequently ratified, and that ratified state is recorded in the master project record and in the metadata table of this file. The historical Phase 1 authorization wording does not activate Phase 1 under the current repository-governance sequence: Phase 1 remains blocked until Gate 0B closes, its closeout is ratified by `NTK-MASTER`, and `NTK-MASTER` explicitly authorizes Phase 1. This note changes no scientific substance.

| Edgar Axel Pérez Flores | Naomi Sánchez Torres |
| --- | --- |
| Scientific Lead | Scientific Collaborator |
