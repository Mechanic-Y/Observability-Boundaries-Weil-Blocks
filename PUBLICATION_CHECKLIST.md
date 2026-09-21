# Publication Checklist — V1.0

## Phase 1 — GitHub preparation

- [x] V1.0 mathematical content frozen.
- [x] JA/EN synchronization audit passed.
- [x] Design v2 visual review passed.
- [x] Frozen PDF byte identity fixed.
- [x] Release asset SHA-256 values fixed.
- [x] GitHub/Zenodo publication scaffold prepared.
- [x] Create public repository `Mechanic-Y/Observability-Boundaries-Weil-Blocks`.
- [ ] Author-review the `publication-v1.0-review` branch and Draft PR.
- [ ] Merge the publication scaffold without regenerating frozen assets.
- [ ] Enable GitHub Pages from `main` / root.

## Phase 2 — Zenodo integration — HOLD UNTIL AUTHOR APPROVAL

- [ ] In Zenodo, open Profile -> GitHub.
- [ ] Click `Sync now`.
- [ ] Enable `Observability-Boundaries-Weil-Blocks`.
- [ ] Confirm `.zenodo.json` metadata before release.

## Phase 3 — GitHub Release — HOLD UNTIL AUTHOR APPROVAL

- [ ] Create tag `v1.0` from the publication-ready commit.
- [ ] Release title: `Observability Boundaries V1.0 — Frozen Bilingual Release`.
- [ ] Use `releases/v1.0/RELEASE_NOTES.md` as the release body.
- [ ] Attach the same three frozen public assets to the GitHub Release UI if desired.
- [ ] Do not alter the tagged repository snapshot after release.

## Phase 4 — Zenodo DOI

- [ ] Wait for Zenodo to ingest the GitHub Release.
- [ ] Verify title, creator, affiliation, version, resource type, license, keywords, and description.
- [ ] Record the assigned DOI.
- [ ] Update `README.md`, `index.html`, `CITATION.cff`, and `ZENODO_RELEASE_NOTES_v1.0.md` on `main` with the DOI.
- [ ] Do **not** regenerate the frozen PDFs merely to embed the DOI.
- [ ] Do **not** create a second GitHub Release for a DOI-only metadata edit.

## Phase 5 — Final public verification

- [ ] GitHub Release downloads open correctly.
- [ ] GitHub Pages download links open correctly.
- [ ] Zenodo DOI resolves.
- [ ] Zenodo record files match the intended release.
- [ ] `SHA256SUMS.txt` verifies all three public assets.
- [ ] GitHub README and Pages show the final DOI.
