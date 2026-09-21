# Observability Boundaries for Near-Critical Weil Blocks

**A Finite-Dimensional Analysis of Off-Line Zero Collisions**

**Planned first release:** `v1.0`  
**Status:** FROZEN / author review before first GitHub Release and Zenodo archival  
**Author:** Yasuyuki Wakita (Mechanic-Y)  
**Affiliation:** Independent Researcher  
**Zenodo DOI:** not assigned yet — Zenodo integration will occur only after author approval

## Overview

This repository publishes the frozen bilingual V1.0 manuscript and reproducibility materials for *Observability Boundaries for Near-Critical Weil Blocks*.

The paper studies the local collision limit of a single off-line reflection pair in a fixed finite-dimensional zero-side matrix of Weil type. The main local statements separate exact negative detection from a vanishing geometric robustness margin and classify higher-order real-symmetric transverse-jet branches.

A representative higher-order asymptotic is

```text
lambda_-(delta) = -2 m ||w||^2 delta^(4q+2) + O(delta^(4q+4)),
q = 0,1,2,...
```

so the possible leading orders in the real-symmetric analytic model class are `2, 6, 10, 14, ...`.

> **Scope guardrail**  
> The proved results are restricted to a fixed finite-dimensional, fixed-collision-ordinate, single-pair local analysis. They do **not** prove the Riemann Hypothesis, do not establish a no-go theorem for the Alpöge–Furman method as a whole, do not solve general interacting multi-pair spectral interaction, and do not imply infinite-dimensional conclusions.

## Research Scope Map

| Layer | Content | Status |
|---|---|---|
| Single-pair local classification | collision expansion, negative branch, geometric margin, higher transverse jets | **FROZEN / proved under stated hypotheses** |
| Actual taper-family realization | non-vacuity of higher jet strata (`q >= 1`) | **Open — Track A** |
| Aggregate spectrum | interacting pair contributions beyond exact direct sum | **Open — Track B** |
| Changing dimension / operator limits | joint `d`, `t`, `delta` limits | **Open — Track C** |
| Prior art / numerical robustness | novelty audit and operational detector thresholds | **Open — Track D** |
| Publication Architecture | bilingual sync, code-to-paper audit, PDF integrity, SHA-256 manifests | **FROZEN provenance layer** |

## Frozen Public Assets

> **Review-stage note:** The binary release assets are intentionally held back during this author-review branch. No GitHub Release or Zenodo deposit has been triggered. Their byte-fixed SHA-256 values are already frozen and recorded below; the exact files will be placed/attached only after author approval.

Expected final public assets:

1. `Observability_Boundaries_V1.0_JA_FROZEN.pdf`
2. `Observability_Boundaries_V1.0_EN_FROZEN.pdf`
3. `Observability_Boundaries_V1.0_FROZEN.zip` — full frozen source/audit package

Canonical hashes:

- JA PDF: `f4d79a8a8ee98878471d9a998f9c47abd8c8b6d00a4d94087de83543a75b10ad`
- EN PDF: `9070f0b9e4bd05371c4ef425c092b5cf482e735c543f0e38e72057069740746a`
- Full Frozen ZIP: `d99fd0fe91fa91cde5538e650fce3e8cf77788f192095df2c392a6a67a7d82ed`

Integrity metadata already staged for review:

- [`releases/v1.0/MANIFEST_v1.0.md`](releases/v1.0/MANIFEST_v1.0.md)
- [`releases/v1.0/SHA256SUMS.txt`](releases/v1.0/SHA256SUMS.txt)
- [`paper/FROZEN_PACKAGE_MANIFEST_SHA256.txt`](paper/FROZEN_PACKAGE_MANIFEST_SHA256.txt) — internal manifest of the full frozen package

## Publication Architecture

The repository follows the same release discipline used in the ReIG publication workflow:

- frozen JA/EN manuscript pair;
- explicit scope and open-problem separation;
- code-to-paper provenance;
- independent cold-review history retained in audit records;
- byte-level PDF identity checks;
- SHA-256 release manifests;
- GitHub Release -> Zenodo archival workflow.

The frozen PDFs are treated as immutable byte sequences. The Zenodo DOI will be added to repository metadata after the DOI is assigned; the frozen PDFs themselves will not be regenerated merely to embed the DOI.

## Repository Structure

```text
Observability-Boundaries-Weil-Blocks/
├── README.md
├── LICENSE
├── CITATION.cff
├── .zenodo.json
├── index.html
├── ZENODO_RELEASE_NOTES_v1.0.md
├── PUBLICATION_CHECKLIST.md
│
├── releases/
│   └── v1.0/
│       ├── MANIFEST_v1.0.md
│       ├── SHA256SUMS.txt
│       ├── RELEASE_NOTES.md
│       └── release_assets/
│           └── README.md   # binaries added only after author approval
│
├── paper/
│   ├── audit/
│   └── FROZEN_PACKAGE_MANIFEST_SHA256.txt
│
└── docs/                  # optional future documentation
```

## Version and Freeze Policy

`v1.0` is the planned first public frozen release.

Any later change to mathematical content, frozen PDF bytes, or theorem statements requires a new version. Metadata-only updates after Zenodo DOI assignment may update the repository's `main` branch without modifying the `v1.0` release tag or frozen release assets.

## AI Assistance Notice

This publication package was prepared with assistance from ChatGPT (OpenAI) and additional AI-based cold-review workflows. All final decisions, mathematical claims, interpretations, and publication responsibility remain with the author, Yasuyuki Wakita / Mechanic-Y.

## Author

**Yasuyuki Wakita (脇田泰行)** — Mechanic-Y  
Independent Researcher

## License

MIT License. See [`LICENSE`](LICENSE).

## Links

- GitHub repository: `https://github.com/Mechanic-Y/Observability-Boundaries-Weil-Blocks`
- GitHub Pages: planned after author approval
- Zenodo DOI: assigned only after the first approved `v1.0` GitHub Release

## Provisional Citation (before DOI assignment)

```text
Wakita, Yasuyuki. (2026). Observability Boundaries for Near-Critical Weil Blocks:
A Finite-Dimensional Analysis of Off-Line Zero Collisions (Version 1.0).
Independent Researcher. GitHub release v1.0.
```

After Zenodo assigns the DOI, the DOI citation will be added here without modifying the frozen PDFs.
