# Open items and their effects

Version 1.0 · 4 October 2026. [Overview](../README.md) · [Step table](step-verification.md) · [Repairs](repairs.md)

The four items below concern different logical levels. No completed repair is claimed for them. Accepting the complete cited Schultens/Kapovich statements as black boxes leaves a usable repaired body proof; it does not independently validate the printed proofs behind those statements.

<a id="d09"></a>
## D09 — FHS adaptation to the relative isotopy comparison class

**Verdict: unresolved.** Freedman–Hass–Scott Theorem 6.2, printed p. 630, concerns closed, two-sided, least-area incompressible maps. Its least-area comparison is over homotopy classes of maps (definition p. 609). The boundary discussion is in §7, pp. 634–637. Schultens uses proper isotopy classes with boundary constrained to the leaf family $J$, and states the required relative disjointness result in Theorem 4 and Appendix Theorem 12 of the checked preprint.

The knot exterior satisfies the environmental conditions; the surfaces are two-sided and incompressible; leaves are equal or disjoint, and the local boundary cut-and-paste respects leaf constraints. These checks do not prove that every covering-space or product-region comparison in the adapted FHS proof remains inside the proper-isotopy-plus-$J$ comparison class. The full separation argument for common-leaf boundaries was not independently completed either.

**Effect:** independent verification of the printed derivation of universal disjointness $(U^*)$ remains incomplete. D08's applicability check of the complete Schultens statement remains valid within the declared black-box scope. The local no-disc-patch proof is not a replacement for universal disjointness. No counterexample to Schultens's statement is supplied.

**Needed to close:** a complete adaptation with every comparison class and boundary move justified, or a proved bridge from the relative isotopy minimum to a suitable homotopy minimum. Such a bridge cannot be assumed from incompressibility alone. FHS Theorem 7.2 (p. 635) and the unproved Existence Statement 7.3 (p. 636) do not automatically supply this result.

<a id="d10"></a>
## D10 — Kapovich's direct application of Anderson Theorem 3.1

**Verdict: the direct application fails.** Anderson Theorem 3.1, pp. 101–102, distinguishes the original surfaces $\widehat\Sigma_i$ from the fixed-$\varepsilon$ truncations $\Sigma_i=\widehat\Sigma_i\cap\Omega_{-\varepsilon}$. The controlled area, topology and convergence conclusions concern the truncations. The theorem requires a common $\varepsilon>0$, connected truncations of fixed topological type, and its convex-domain setting. Fixed topology of the full source surface does not supply fixed topology of its truncations. Strict convexity of the ambient boundary is not by itself the full defining-function hypothesis.

Kapovich Proposition 9 needs convergence of the whole surfaces up to their original boundary. The truncated conclusion does not give that output, even if additional convexity or truncation hypotheses could be supplied. This output mismatch is sufficient for the negative verdict; it does not depend on adopting the strongest possible interpretation of “strictly convex domain.”

**Effect:** the printed proof of Proposition 9 is not independently verified. Through Corollary 11, this also limits independent verification of $(E^*)$. It does not prove Anderson's theorem, Kapovich's proposition, or Theorem 5.1 false. The complete externally cited statements can still be used at the black-box level expressly allowed here.

**What the attempted repairs do and do not give:** Schoen's interior stability estimate can control an already separated interior region. A weak globally convex defining function can be made from a collar function: choose $q(0)=0$, $q'<0$, $q''\ge0$, flatten $q'$ to zero and extend $q$ as a negative constant. Then $\mathrm{Hess}(q(r))=q''dr^2+q'\mathrm{Hess}r\ge0$. Neither argument provides whole-surface boundary convergence. Local convex replacement domains still require control of sheet number, local topology, artificial-cap curves, boundary graphical convergence and multiplicity. Choosing caps using the desired boundary convergence would be circular.

Anderson Theorem 3.2 (p. 103) retains the convex-domain setting and requires a controlled boundary system; the new artificial cut arcs are not already such a system. Hass–Scott Lemmas 6.9–6.11 concern exact least-area discs, while the general stable minimal members of $M_a$ have not been shown to be locally such discs.

**Needed to close:** a boundary compactness/attainment argument for the actual general setting, including boundary graphs, sheets, multiplicity and isotopy-block control. Adding a page number is insufficient.

<a id="d12"></a>
## D12 — membership of the attained minimizer in Definition A.1

**Verdict: unresolved.** Hass–Scott Theorem 6.12, pp. 112–113, gives an attained minimum in its own piecewise smooth class, isotopic to the input relative to its boundary. It does not merely produce an unspecified weak limit. The present check nevertheless did not establish that its attained surface has every feature demanded by the competition paper's Definition A.1 and equation (27), p. 23: a finite singular graph, pieces $C^1$ on their closures, and the specified nondegenerate corner/tangent-ray structure.

Finite seams in members of a construction sequence do not by themselves prove this structure for its limit. Conversely, failure to find an identical printed definition does not prove the two classes incompatible or Hass–Scott's theorem false.

**Effect:** the original Appendix A existence route cannot feed its attained minimizers into the conditional regularity argument of Proposition A.5 without an additional membership/comparison-class bridge. D13–D21 can hold conditionally without closing D12. The independent body replacement in [R01](repairs.md#r01) avoids this target-paper membership issue, but does not prove it.

**Needed to close:** a precise inclusion theorem for the attained output, or a separate attainment and isotopy/comparison-class argument. The special rounding of transverse creases in [R03](repairs.md#r03) does not cover all A.1 vertices and boundary corners, and cannot silently prove equality of the auxiliary piecewise smooth and smooth infima.

<a id="d22"></a>
## D22 — assembly of Theorem A.6

**Verdict: unresolved.** The assembly in Theorem A.6, p. 27, is conditionally sound if a genuine smooth stable fixed-boundary minimizing sequence has been supplied. One then uses $M_a$ compactness, open-and-closed isotopy blocks, area continuity and extension of nearby neat isotopies. The original supply passes through D12, which is still unclosed. Expanding the compactness black box also encounters D10.

**Effect:** Appendix A's stronger attainment claim for its defined piecewise smooth comparison class is not certified. The body actually invokes A.6/A.7 (§5 opening, p. 13, and the double-graph uses, pp. 18–19); this is a real source issue in the original route. Replacing those calls by complete E(ii) plus independent Hopf supplies their body uses, not a proof of A.6.

**Needed to close:** supply the required sequence in the asserted comparison class and justify its attainment. Conditional regularity cannot be run backwards to create a minimizer. Compactness alone does not prove nonemptiness.

<a id="textbooks"></a>
## Original books and chapters not compared

| Source | Nodes and actual use | Outstanding source check / limit |
|---|---|---|
| Gilbarg–Trudinger, 2nd ed. (1983) | D15/D16/D57/D58/D67 and local regularity: gradient Hölder estimates with bounded sources, Schauder, Hopf, Lax–Milgram, scaled supremum estimates, strong maximum principle, linear Dirichlet comparison | Original pages and exact versions not compared. Candidate locators are recorded as **unverified** in the bibliography. D58 has a small-domain barrier backup; reflected equations also admit direct Laplace regularity. |
| Vekua (1962) | D65/D66: similarity factorization with $p>2$, continuous bounded exponential factor and finite-order gradient zeros | Original Chapter III not compared. [R08](repairs.md#r08) gives a standard local Cauchy-transform factorization, without claiming an original-page check. |
| Wall (2016) | D04 and positive-width/positive-parameter neat isotopy extension; relative-collar extensions for disc moves | Theorem 2.4.6 and the needed boundary/relative versions not compared against the book. Uses are restricted to compact smooth neat tracks; vector-field adaptations are stated. No true corner is a smooth endpoint. |
| Schoen (1983) | D11: interior stable-minimal-surface curvature estimates in the printed compactness proof | Original chapter, theorem number and exact constant dependencies not compared. Only interior estimates at positive boundary distance are used; no boundary compactness follows. |

These are source-verification debts, not demonstrated counterexamples. They are distinct from the substantive unclosed bridges D09/D10/D12/D22.

## Edition and extraction limits

- Schultens/Kapovich: the checked source is **arXiv:0707.3926v4**. Theorems 2/4, Proposition 9, Corollaries 10/11 and Theorem 12 were checked there. The journal Appendix A numbering and pagination were not independently compared page by page.
- Hildebrandt–von der Mosel: the checked author version, dated 21 November 2005, supplies Theorem 4.1 and its boundary conclusion, pp. 18 and 22; there is no separate full journal-version comparison.
- FHS: the acquired scan has no text layer. Its working text is OCR; formulas require the scan image. The supplied records include image checks of the key statements, not certification of every OCR symbol.
- Kakimizu: the supplied targeted review checked pp. 225 and 228. The irreducibility citation is no longer a missing-source item. Theorem A's connectedness is background for later applications, not an additional predecessor of this exchange proof.

## Boundary of the conclusion

The two failures in the original step table are D10's **direct application** and D29's **smooth corner-endpoint reading**. D29 has a usable replacement; D10 has no completed independent boundary-compactness replacement in these records. The three unresolved original steps are D09, D12 and D22. None of these facts alone supplies a counterexample satisfying all global hypotheses and contradicting Theorem 5.1(a)–(d). The conditional repaired body conclusion and these unresolved items must be reported together.
