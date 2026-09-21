# MANIFEST — v1.0

**Release:** Observability Boundaries for Near-Critical Weil Blocks  
**Version:** `v1.0`  
**Prepared:** 2026-09-21  
**Author:** Yasuyuki Wakita / Mechanic-Y  
**Repository:** `Mechanic-Y/Observability-Boundaries-Weil-Blocks`

## Publication principle

This release publishes the frozen bilingual V1.0 paper and its reproducibility package. Mathematical scope remains the fixed finite-dimensional single-pair local classification. Open Tracks A-D are research agenda items and are not promoted to theorem status.

## Public release assets

| # | File | Layer | Status | Size bytes | SHA256 |
|---:|---|---|---|---:|---|
| 1 | `Observability_Boundaries_V1.0_JA_FROZEN.pdf` | paper / Japanese | public / frozen | 393756 | `f4d79a8a8ee98878471d9a998f9c47abd8c8b6d00a4d94087de83543a75b10ad` |
| 2 | `Observability_Boundaries_V1.0_EN_FROZEN.pdf` | paper / English | public / frozen | 228684 | `9070f0b9e4bd05371c4ef425c092b5cf482e735c543f0e38e72057069740746a` |
| 3 | `Observability_Boundaries_V1.0_FROZEN.zip` | source + audit provenance | public / frozen package | 891786 | `d99fd0fe91fa91cde5538e650fce3e8cf77788f192095df2c392a6a67a7d82ed` |

## Integrity rule

The two PDFs and the frozen ZIP are byte-fixed release artifacts. Do not regenerate them in-place after the `v1.0` tag is published. Any change to these files requires a new version.

The Zenodo DOI is intentionally not embedded into the frozen PDF bytes. After DOI assignment, only repository metadata such as README, Pages, CITATION, and Zenodo notes may be updated on the main branch.

## Release actions

1. Author-review and approve the publication branch before any Zenodo action.
2. Merge the publication-ready snapshot.
3. Enable the repository in Zenodo's GitHub integration.
4. Create GitHub Release `v1.0` from the approved frozen publication commit.
5. Confirm Zenodo ingestion and metadata.
6. Record the assigned DOI in README, Pages, CITATION, and Zenodo release notes without altering the frozen release assets or tag.
