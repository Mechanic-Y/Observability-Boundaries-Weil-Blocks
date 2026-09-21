# Publication Checklist — V1.0

## Phase 1 — GitHub preparation

- [x] V1.0 mathematical content frozen.
- [x] JA/EN synchronization audit passed.
- [x] Design v2 visual review passed.
- [x] Frozen PDF byte identity fixed.
- [x] Release asset SHA-256 values fixed.
- [x] GitHub/Zenodo publication scaffold prepared.
- [x] Create public repository `Mechanic-Y/Observability-Boundaries-Weil-Blocks`.
- [x] Author-review the `publication-v1.0-review` branch and Draft PR.
- [x] Stage canonical JA/EN PDFs and full Frozen ZIP on the review branch without changing bytes.
- [x] Merge the publication scaffold without regenerating frozen assets.
- [x] Enable GitHub Pages from `main` / root.

## Phase 2 — Zenodo integration — COMPLETED

- [x] In Zenodo, open Profile -> GitHub.
- [x] Click `Sync now`.
- [x] Enable `Observability-Boundaries-Weil-Blocks`.
- [x] Confirm `.zenodo.json` metadata before release.

## Phase 3 — GitHub Release — COMPLETED

- [x] Create tag `v1.0` from the publication-ready commit.
- [x] Release title: `Observability Boundaries V1.0 — Frozen Bilingual Release`.
- [x] Use `releases/v1.0/RELEASE_NOTES.md` as the release body.
- [x] Attach the same three frozen public assets to the GitHub Release UI.
- [x] Do not alter the tagged repository snapshot after release.

## Phase 4 — Zenodo DOI

- [x] Wait for Zenodo to ingest the GitHub Release.
- [ ] Final post-publication metadata spot-check: title, creator, affiliation, version, resource type, license, keywords, and description.
- [x] Record the assigned DOI: `10.5281/zenodo.22877149`.
- [x] Update `README.md`, `index.html`, `CITATION.cff`, and `ZENODO_RELEASE_NOTES_v1.0.md` on `main` with the DOI.
- [x] Do **not** regenerate the frozen PDFs merely to embed the DOI.
- [x] Do **not** create a second GitHub Release for a DOI-only metadata edit.

## Phase 5 — Final public verification

- [ ] GitHub Release downloads open correctly.
- [ ] GitHub Pages download links open correctly.
- [x] Zenodo DOI resolves.
- [ ] Zenodo record files match the intended release.
- [ ] `SHA256SUMS.txt` verifies all three public assets.
- [x] GitHub README and Pages show the final DOI.
