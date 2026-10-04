# Bibliography and source status

Version 1.0 · 4 October 2026. [Overview](../README.md) · [Open items](../proof/open-items.md)

This list covers the target and sources used in the verification or its stated proof-source limits. It is not a reproduction of the target paper's entire bibliography. “Checked” below reports the supplied verification records, not a new independent source audit during packaging. Links give recorded acquisition routes or bibliographic destinations; no network access was used to prepare this repository. No third-party full text or PDF is bundled.

Printed page numbers belong to the **specified edition**. Author/preprint pages are not journal pages. Candidate textbook pages inherited from the source checklist are explicitly unverified. R01–R11 are source identifiers; target reference numbers are separately identified.

## Target

**Apex Intelligence.** *Contractibility of the Complex of Incompressible Seifert Surfaces: The Knot Case of Kakimizu’s Problem*. Official competition version, dated 11 September 2026, 48 printed pages. Theorem 5.1, p. 13; proof in §5, pp. 13–19, with relevant §§3–4, pp. 6–12, Appendix A, pp. 23–28, and Appendix B, pp. 28–39.

Acquisition: supplied local copy of the official competition PDF. SHA-256: `34f17d7d99780d3fd3626d9e5d7b35d6aa76661c404f191b6df341b300c0c06f`. The supplied text hash is `54f60d38dd61a7ad2eaef2c376f17422cacd2a734c63d4cdad531d4b0ff34d91`. No official download URL was provided in the allowed records, so none is invented here. The exact PDF is identified by its hash and is not redistributed.

## R01 — Schultens, with Kapovich's appendix

**Jennifer Schultens.** *The Kakimizu complex is simply connected*, with an appendix by Michael Kapovich. *Journal of Topology* **3** (2010), no. 4, 883–900. Target reference **[17]**.

**Checked edition:** [arXiv:0707.3926v4](https://arxiv.org/abs/0707.3926v4), already available locally. Working text SHA-256: `0551e173a34d142294490f8027ecf72d013e3a925517305cdf2a7dcf4f7b002c`.

| Checked preprint location | Use |
|---|---|
| Definition 3, p. 3 | Relative least area over the proper isotopy class with boundary in $J$ |
| Theorem 2, p. 4 | Relative least-area representative: D06 / complete E(ii) |
| Theorem 4, p. 4 | Arbitrary chosen relative minima are disjoint or coincide if the classes admit disjoint representatives: D08 / $(U^*)$ |
| Appendix setup, pp. 18–19 | Smooth proper embedded stable members, nonempty boundary, one source boundary over each ambient boundary, compact curve family |
| Proposition 9, p. 19 (setup begins p. 18) | Compactness of $M_a$; printed-proof issue D10 |
| Corollary 10, p. 19 | Finitely many open-and-closed isotopy blocks |
| Corollary 11, p. 20 | Attainment, including its whole proper-class “in particular” clause |
| Boundary adaptation and Theorem 12, p. 20 | FHS adaptation / disjointness; D09 remains unclosed at proof level |

The competition paper cites journal Appendix Proposition A.1, Corollaries A.3/A.4 and Theorem A.5. Their correspondence with preprint Proposition 9, Corollaries 10/11 and Theorem 12 is recorded in the supplied materials; journal numbering/text/pages were not independently compared. Do not attach preprint p. 20 to the journal citation as a checked journal page. The original nonemptiness proof also returns to Hass–Scott; accepting Corollary 11 does not certify that return.

## R02 — Hass–Scott

**Joel Hass and Peter Scott.** *The existence of least area surfaces in 3-manifolds*. *Transactions of the American Mathematical Society* **310** (1988), no. 1, 87–114. Target **[6]**.

Acquired from the AMS free historical journal archive, [DOI 10.1090/S0002-9947-1988-0965747-6](https://doi.org/10.1090/S0002-9947-1988-0965747-6). PDF SHA-256: `aaf1544f16de6c03203a8b56357ebc595241ca6b3dfd6714cfea6464a6a304f5`.

Checked: smooth-category convention p. 89; homogeneous regularity p. 109; the three sufficiently-convex conditions p. 110; Theorem 6.12, pp. 112–113; related Theorem 5.1, pp. 106–107, and Lemmas 6.9–6.11, p. 112 and following discussion. The fixed-boundary attained surface lies in that source's piecewise smooth class. The precise bridge to the target's Definition A.1 is D12, not a consequence of adding these page numbers.

## R03 — Gilbarg–Trudinger

**David Gilbarg and Neil S. Trudinger.** *Elliptic Partial Differential Equations of Second Order*. 2nd ed., Grundlehren der mathematischen Wissenschaften **224**, Springer, Berlin, 1983. Target **[4]**.

**Original book not compared.** Used at standard-statement level. Acquisition route: publisher electronic book or library copy; no legal free complete copy was obtained in the recorded work.

| Required result | Candidate locator, **not original-page verified** |
|---|---|
| Hopf boundary-point lemma, D16 | Lemma 3.4, p. 34 |
| Lax–Milgram, D57 | Theorem 5.8, p. 83 |
| Supremum estimate with an $L^2$ term, D58 | Theorem 8.15, p. 189 |
| Comparison with the sign-dependent alternative | Theorem 8.16, p. 191; not substituted for 8.15 |
| Strong maximum principle after removing the zero-order term, D67 | Theorem 8.19, p. 198 |
| Interior gradient regularity and Schauder, D15 | Chapters 6/8; precise bounded-source version still to identify |
| Linear local/flat-boundary regularity and $L^p$ Dirichlet inverse | Exact appropriate results still to identify |
| Nondivergence uniqueness used in the boundary repair | Theorem 9.5, p. 225; candidate locator from the comparative material |

These locators are leads for later source checking, not a claim that the original pages were read. The repair states the actual analytic hypotheses and gives a barrier backup for positivity.

## R04 — Hildebrandt–von der Mosel

**Stefan Hildebrandt and Heiko von der Mosel.** *Conformal representation of surfaces, and Plateau’s problem for Cartan functionals*. *Rivista di Matematica della Università di Parma* (7) **4*** (2005), 1–43. Target **[9]**; the volume's star is retained from the supplied bibliography.

**Checked edition:** author version dated 21 November 2005, acquired from the [RWTH author publication page / recorded PDF](https://instmath.rwth-aachen.de/~heiko/veroeffentlichungen/cartan.pdf). PDF SHA-256: `136ffb0ad864e22d75aa8113987ad61de15aada16f3ef1161ff3c99356fe063a`.

Checked Theorem 4.1, case $m=1$, p. 18, and the boundary nondegeneracy/completion argument p. 22, including visual page checks in the supplied record. This supplies a $C^{1,\alpha}$ closed-boundary diffeomorphism for the stated metric and Jordan-boundary hypotheses. Only a local compact patch away from the Möbius pole is used for bi-Lipschitz bounds. No separate full journal comparison was made.

## R05 — Vekua

**Ilia N. Vekua.** *Generalized Analytic Functions*. Pergamon Press, Oxford, 1962. Target **[18]**.

**Original book not compared.** Acquisition route: authorized publisher archive or library copy; no legal free complete English edition was obtained. Standard similarity principle used for D65; a local Cauchy-transform derivation is supplied in the repairs.

Candidate Chapter III locators, **unverified against the book**: §1 equation (1.5), p. 131; standing condition (1.10), p. 137; §4.1 Basic Lemma, p. 144, formula (4.3), p. 146; §4.2 Theorem 3.5, pp. 146–147, inequalities (4.15), p. 152. These are source-checking leads. The equation includes the complex conjugate term; extracted-text loss of its overline is not a demonstrated error in the target PDF.

## R06 — Wall

**C. T. C. Wall.** *Differential Topology*. Cambridge University Press, Cambridge, 2016. Target **[20]**.

**Original book not compared.** Theorem 2.4.6, candidate p. 52, is used at standard-statement level for compact smooth neat embedding isotopies and ambient extension preserving the ambient boundary setwise. Relative-collar uses require the explicit vector-field adaptations in the repairs. Acquisition route: Cambridge Core or a library copy; no complete authorized open copy obtained. The theorem is never used to make a true corner into a smooth isotopy endpoint.

## R07 — Kakimizu

**Osamu Kakimizu.** *Finding disjoint incompressible spanning surfaces for a link*. *Hiroshima Mathematical Journal* **22** (1992), no. 2, 225–236. Target **[10]**.

Acquisition: journal PDF supplied by the human director; bibliographic route [DOI 10.32917/hmj/1206392900](https://doi.org/10.32917/hmj/1206392900). PDF SHA-256: `eb195635ce7ddb1c74caccae36d4493e875773f29de0f013eb91f5471c10b36c`.

Targeted source check: p. 225, spanning surfaces, ambient equivalence and $IS(L)$ vertex/simplex conventions; p. 228, §2 around Theorem 2.1, irreducibility of a non-split link exterior. A knot is non-split; its single boundary component and exclusion of closed components make the spanning surface connected. Add **[10, p. 228]**, not Theorem A as a substitute locator for irreducibility. Theorem A, p. 226, gives connectedness and was additionally checked as background; it is not a predecessor needed here. Proposition 3.1(1), p. 231, is a distance-convention lead, not claimed as an additional targeted page check.

## R08 — Freedman–Hass–Scott (FHS)

**Michael Freedman, Joel Hass and Peter Scott.** *Least area incompressible surfaces in 3-manifolds*. *Inventiones Mathematicae* **71** (1983), no. 3, 609–642. Target **[3]**. Schultens's bibliography uses a title variant; this entry uses the journal title in the supplied acquisition record.

Acquired from the Göttingen digitization centre GDZ, volume identifier `PPN356556735_0071`, article `LOG_0034`; bibliographic route [DOI 10.1007/BF02095997](https://doi.org/10.1007/BF02095997). PDF SHA-256: `1b7427a870cf32e90054ce6ea122340bfbaaa4ab71341c5be3ac01fb0808a3e5`.

**OCR warning:** this is a scan without a text layer. The working text was produced by macOS Vision OCR at 300 dpi (35 scanned pages). Prose and theorem statements were readable; formulas may contain recognition errors. The supplied verification checked key statements against images. No OCR text or scan is redistributed here.

Checked: least-area comparison definition p. 609; Theorem 6.2 p. 630; boundary modifications §7, pp. 634–637; Theorem 7.2 p. 635; Existence Statement 7.3 p. 636, expressly unproved in that source. D09 records the unresolved full adaptation to proper isotopy with $J$-leaf boundary constraints. This source's Theorem 5.1 is not the target Theorem 5.1.

## R09 — Anderson

**Michael T. Anderson.** *Curvature estimates for minimal surfaces in 3-manifolds*. *Annales scientifiques de l’École Normale Supérieure*, série 4, **18** (1985), 89–105. A reference in Kapovich's appendix, not target [3].

Acquired from [NUMDAM, article ASENS_1985_4_18_1_89_0](https://www.numdam.org/item/ASENS_1985_4_18_1_89_0/); [DOI 10.24033/asens.1485](https://doi.org/10.24033/asens.1485). PDF SHA-256: `7ef07d96262cb11312540a3b41ddf0086c38948fe0db815e74de9f3db0271db4`.

Checked: defining-function setting near Lemma 1.2 p. 93; Theorem 2.2 pp. 98–99; Theorem 3.1 and proof pp. 101–102 (including the fourth proof paragraph); Theorem 3.2 p. 103. The original/truncated surface distinction was visually checked. D10's failed direct application is an output/hypothesis mismatch, not a refutation of this theorem.

## R10 — Schoen

**Richard Schoen.** *Estimates for stable minimal surfaces in three dimensional manifolds*. In *Seminar on Minimal Submanifolds*, Annals of Mathematics Studies **103**, Princeton University Press, Princeton, NJ, 1983, 111–126. Referenced in Kapovich's appendix, not target [20].

**Original chapter not compared.** The interior stable-minimal-surface curvature estimate is used at standard-statement level for D11. A specific theorem number and exact original pages remain unverified; 111–126 is the chapter range, not a verified pinpoint. Acquisition route: authorized publisher/library or author copy; no legal free full chapter obtained. No boundary estimate is attributed to this source here.

## R11 — Hatcher's three-manifold notes

**Allen Hatcher.** *Notes on Basic 3-Manifold Topology*. Cornell University, online notes; copy acquired on 4 October 2026. Acquisition: [author's recorded PDF](https://pi.math.cornell.edu/~hatcher/3M/3Mfds.pdf). PDF SHA-256: `c8add1a8633f36cb50de313f8f340a3f2b63b5548077d6e30f9c51a073398ff6`.

Checked edition: the acquired copy states the smooth category at printed p. 1; p. 20 (proof of Lemma 1.10) gives the same-boundary-disc isotopy fact in a three-ball; **Corollary 3.3, printed p. 59**, gives the compression-disc/$\pi_1$-injectivity interface for two-sided surfaces. The checklist's candidate p. 48 is not the pagination of this acquired copy. These are not Hatcher's *Algebraic Topology*; the two books must not be conflated.

## Context only — Przytycki–Schultens

**Piotr Przytycki and Jennifer Schultens.** *Contractibility of the Kakimizu complex and symmetric Seifert surfaces*. *Transactions of the American Mathematical Society* **364** (2012), no. 3, 1489–1508. Target **[16]**.

Acquisition: already available local copy; possible routes recorded in the checklist are the AMS archive and author copies. Working text SHA-256: `6f68b786bc43f1ae73a4e6907723862168618bbd8e10328b4b864b535af71154`. Theorem 1.1, Theorem 1.5, Proposition 4.4 and the remaining-questions discussion are contextual locators; no independently verified printed pinpoint pages are claimed in the supplied final records. This is not a predecessor of D87 and is not used to prove the general-genus exchange construction.

## Verification-record provenance

The private working records are not bundled and no local machine paths are exposed. The package is based on the supplied Chinese records, all v1.0: synthesis; adversarial review; final Claude cross-model review; routes one, two and three; targeted Kakimizu 1992 review; dependency map; required-source checklist; acquisition log. Priority is **final conclusion and adversarial corrections over corrected route/synthesis wording**, with the detailed route arguments retained where compatible. This bibliography reflects the acquisition log and completed route checks rather than the checklist's “not acquired” placeholders.

Other optional sources in the exploratory checklist, and sources for later-version global category bridges, are not used as accepted inputs in this package. There is no claim that they were checked or that later-version proofs were independently certified.
