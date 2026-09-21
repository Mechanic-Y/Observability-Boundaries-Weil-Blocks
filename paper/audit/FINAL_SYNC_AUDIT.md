# Observability Boundaries V1.0 — JA↔EN Final Synchronization and Code-to-Paper Audit

**Status:** PASS  
**Date:** 2026-09-21 (JST)

## 1. Audited files

- JA: `Observability_Boundaries_V1.0_JA_Publication_Candidate.md`
- EN: `Observability_Boundaries_V1.0_EN_Publication_Candidate.md`

SHA-256:

- JA: `49b39e9e619cf3037aed459074871990b1e223d8799390780ad658de9acdf88b`
- EN: `9a2ec60e78884c027882a13c1ce4902ad63cc9896fa5985aea4c7b6c32542ab8`

## 2. Structural synchronization

| Item | Result |
|---|---|
| Equation tags | PASS — 70 / 70, identical tag set, no duplicates |
| Headings | PASS — 97 / 97 |
| Markdown tables | PASS — 5 / 5 |
| References | PASS — 9 / 9 |
| New bridge equations | PASS — (2.8g) through (2.8l) present in both |
| Version residue | PASS — no stale `Version 0.4` in EN |
| OB-1 framing | PASS — `Expansion 3.1` / `展開3.1`; no stale Theorem 3.1 reference |
| OB-2 framing | PASS — `Observation 4.1` / `観察4.1`; no stale Proposition 4.1 reference |

## 3. V1.0 publication-patch semantic gates

| Topic | Result |
|---|---|
| reflection pair vs global quartet | PASS — both texts identify the block orbit as `rho -> 1 - conj(rho)` and do not collapse the full quartet |
| transpose / Weil bridge | PASS — both texts reproduce the `paperFT_fk` + Schwarz symmetry + real `tau_l` reduction to the transpose-type entry |
| load-bearing sign | PASS — both texts explicitly distinguish the construction from a same-argument Hermitian product `u u*` |
| aggregate scope | PASS — pair decomposition alone gives no theorem for the spectrum of full aggregate `blockA`; uncontrolled effect named `spectral interaction` |
| OB-1 positioning | PASS — quadratic starting order treated as even-analytic, explicit coefficient retained as substantive content |
| OB-2 positioning | PASS — downgraded to an elementary continuity observation |
| parity scope | PASS — `2,6,10,...` explicitly restricted to the real-symmetric analytic model class |
| `lambda_+` justification | PASS — Weyl perturbation bound added in both |
| `x0=0, h'=0` clarification | PASS — exact `diag(delta^4,-delta^6)` example and coefficient `-m/18` present in both |
| Bombieri positioning | PASS — off-line/negative-inertia correspondence described as known background; no historical-priority claim for Theorem 5.5 |
| fixed-positive-depth caveat | PASS — Abstract states that the collision-limit result does not exclude positive separation away from zero |

## 4. Code-to-paper audit for the new load-bearing bridge

Pinned source: `anthropics/formal-math @ fbdc36bbf17d20af3fd0447c6d1a8a02773c9844`

### `Zeta23/Hypotheses/GzGp.lean`

Confirmed:

- `paperFT_fk`: `h_{f_k}(z) = phiHat(z - tau_k)`.
- `GzGp.phiHat_conj`: `phiHat(conj z) = conj(phiHat z)`; this is the Schwarz symmetry used in the paper.
- `Gz_eq_W`: its `rw` chain uses `paperFT_fk`, realness of `tau_l`, `map_sub`, `phiHat_conj`, and `conj_conj` to reduce the conjugated Weil summand to the transpose-type zero-side product.

### `Zeta23/ZeroSide.lean`

Confirmed:

- the paper block structure uses the involution `sigma = (rho -> 1 - conj rho)`, preserving ordinate;
- `blockA = sum m_rho u_rho u_rho^T` explicitly says “transpose, NOT conjugate-transpose”;
- `pair_term` proves `m(uu^T + ubar ubar^T) = 2m(xx^T - yy^T)`;
- `blockA_decomp` sums these pair contributions in the actual zero-side decomposition.

### duplicate-name note

The snapshot contains other theorems named `phiHat_conj`, including a Params-level wrapper in `Zeta23/Taper.lean`. V1.0 intentionally cites `GzGp.phiHat_conj` in `Zeta23/Hypotheses/GzGp.lean` because that is the lemma used directly by the `Gz_eq_W` proof chain.

## 5. Research-Agenda Integration Audit

| Track | Scope | Result |
|---|---|---|
| A — actual taper family | theorem applicability separated from higher-stratum non-vacuity; `q>=1` realizability open | PASS |
| B — aggregate spectral interaction | aggregate extension kept separate from proved single-pair results | PASS |
| C — finite-to-infinite limits | joint `d`, `t`, and `delta` limits explicitly open | PASS |
| D — prior art / numerical robustness | novelty audit and operational detector robustness separated from theorem claims | PASS |
| genericity wording | “generic” means only local jet nondegeneracy, not statistical/arithmetic genericity over zeta zeros | PASS |
| Failure Ledger wording | publication text uses “external cold review”; model-specific provenance may remain internal | PASS |

Priority is **Track A -> Track B -> Track C**, with Track D in parallel. The theorem set of V1.0 is unchanged.

**Verdict: PASS — V1.0 JA and EN are synchronized at the mathematical-claim, scope, and load-bearing code-bridge levels.**
