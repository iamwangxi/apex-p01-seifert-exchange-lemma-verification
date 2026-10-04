# Step-by-step verification

Version 1.0 · 4 October 2026. [Overview](../README.md) · [Dependency map](dependency-map.md) · [Repairs](repairs.md) · [Open items](open-items.md)

Exactly 87 original input/inference steps: **Cited 16** (external result), **Paper 51** (paper argument/construction or substantive interface), **Standard 20** (standard fact/calculation). Types describe provenance, not confidence. Verdicts: **Holds 45**, **Holds with repair 37**, **Unresolved 3**, **Fails 2**. Holds includes conditional local inferences and black-box applicability checks. D10 fails only as a direct application; D29 fails only in the smooth corner-endpoint reading. A repaired replacement does not retroactively pass the original sentence.

Competition locators are printed pages and identifiers. D09–D11 audit the literature underlying §3; they are not direct upstream applications by the target proof. The links give their external locators. On passed rows, repair links also serve as reasoning/interface-check links. Unresolved rows link to open items because no complete repair exists.

| Step | Type | Competition-version location | Verdict | Brief reason | Repair / check |
|---|---|---|---|---|---|
| <a id="d01"></a>D01 | Standard | §3 pp. 6–7, (2)–(3) | Holds | Inward Hessian and convexity signs agree; the collar does not give global strict convexity. | [R01](repairs.md#r01) |
| <a id="d02"></a>D02 | Cited | §3 p. 7; §4 p. 8, [10] | Holds | Kakimizu p. 228 supports irreducibility; orientability excludes two-sided projective planes. | [R01](repairs.md#r01) |
| <a id="d03"></a>D03 | Standard | §4 pp. 8, 10–11 | Holds | A connected single-longitude surface has χ=1−2g; two-sided incompressibility gives π₁-injectivity. | [R01](repairs.md#r01) |
| <a id="d04"></a>D04 | Cited | §4 p. 8, [20, Thm. 2.4.6] | Holds | Compact smooth neat tracks extend preserving ambient boundary setwise; Wall's book remains unchecked. | [R01](repairs.md#r01) |
| <a id="d05"></a>D05 | Cited | §3 p. 7, Thm. 3.2(i) | Holds | Hass–Scott 6.12 applies in its own piecewise smooth class, without proving A.1 membership. | [R01](repairs.md#r01) |
| <a id="d06"></a>D06 | Cited | §3 p. 7, Thm. 3.2(ii) | Holds | The complete Schultens statement supplies smooth proper minima over the whole leaf-boundary class. | [R01](repairs.md#r01) |
| <a id="d07"></a>D07 | Cited | §3 p. 7, Thm. 3.3 | Holds | The cited statements apply; independent verification of their printed proof is limited by D10. | [R01](repairs.md#r01) |
| <a id="d08"></a>D08 | Cited | §3 p. 7, Thm. 3.1 | Holds | The arbitrary-minimizer quantifier and application hypotheses are satisfied. | [R01](repairs.md#r01) |
| <a id="d09"></a>D09 | Cited | §3 p. 7, Thm. 3.1 source; §5 p. 19 | Unresolved | The full homotopy-minimum to leaf-constrained proper-isotopy adaptation remains unverified. | [Open D09](open-items.md#d09) |
| <a id="d10"></a>D10 | Cited | §3 p. 7, Thm. 3.3 source | Fails (limited scope) | Anderson 3.1 controls truncations, not the whole-boundary convergence needed by Kapovich. | [Open D10](open-items.md#d10) |
| <a id="d11"></a>D11 | Cited | §3 p. 7, Thm. 3.3 source | Holds | The standard Schoen estimate addresses interior singularities only; the original chapter is unchecked. | [R01](repairs.md#r01) |
| <a id="d12"></a>D12 | Paper | Appendix A p. 23, Def. A.1, (27) | Unresolved | The attained HS output is not proved to have A.1's precise finite-piece and corner structure. | [Open D12](open-items.md#d12) |
| <a id="d13"></a>D13 | Paper | Appendix A pp. 23–24, Lem. A.2 | Holds | Given an A.1 minimizer, interior variations and open-edge flux limits give minimal pieces and opposite conormals. | [R02](repairs.md#r02) |
| <a id="d14"></a>D14 | Paper | Appendix A p. 24, Lem. A.3 | Holds with repair | Weak gluing and gradient lifting must retain height, spatial and lower-order terms. | [R02](repairs.md#r02) |
| <a id="d15"></a>D15 | Cited | Appendix A pp. 24, 26, [4] | Holds with repair | Solution Hölder continuity is insufficient; difference quotients and a boundary W²,⁴ entry repair the step. | [R02](repairs.md#r02) |
| <a id="d16"></a>D16 | Cited | Appendix A p. 25, Lem. A.4, [4, Lem. 3.4] | Holds | Signs and boundary-point conditions are valid at standard-statement level; the original GT page is unchecked. | [R01](repairs.md#r01) |
| <a id="d17"></a>D17 | Paper | Appendix A pp. 24–25, Lem. A.4 | Holds with repair | Minimal immersion bounds the drift; the genuine curved sectors need an interior tangent ball. | [R02](repairs.md#r02) |
| <a id="d18"></a>D18 | Paper | Appendix A pp. 25–26, Prop. A.5 | Holds with repair | A proper connected punctured projection truncation must precede the degree-one and removable-point arguments. | [R02](repairs.md#r02) |
| <a id="d19"></a>D19 | Paper | Appendix A p. 26, Prop. A.5 | Holds with repair | Apply Hopf on the real curved graph before the half-circle constraint concludes total angle π. | [R02](repairs.md#r02) |
| <a id="d20"></a>D20 | Paper | Appendix A p. 26, Prop. A.5 | Holds with repair | Continuous-coefficient Dirichlet comparison gives W²,⁴, then gradient Hölder and boundary Schauder. | [R02](repairs.md#r02) |
| <a id="d21"></a>D21 | Standard | Appendix A p. 26, Prop. A.5 | Holds | Properness is input; interior variation and H¹₀ density give fixed-boundary stability conditionally. | [R02](repairs.md#r02) |
| <a id="d22"></a>D22 | Paper | Appendix A p. 27, Thm. A.6 | Unresolved | The conditional assembly works, but the actual smooth minimizing sequence still depends on D12. | [Open D22](open-items.md#d22) |
| <a id="d23"></a>D23 | Paper | Appendix A pp. 27–28, Lem. A.7; §5 p. 13 | Holds with repair | Hopf on a smooth proper minimum's curved half-neighbourhood gives neatness and may follow D06 directly. | [R01](repairs.md#r01) |
| <a id="d24"></a>D24 | Paper | §4 p. 9, Lem. 4.3(2); §5 p. 17 | Holds | E*, independent Hopf and U* fix one S missing A and B; distance 2 forces A∩B nonempty. | [R01](repairs.md#r01) |
| <a id="d25"></a>D25 | Standard | Appendix B pp. 28–29 | Holds | Endpoint matching and nonnegative density saving give a common positive coefficient for four sectors. | [R03](repairs.md#r03) |
| <a id="d26"></a>D26 | Paper | Appendix B p. 29 | Holds with repair | Exact straightening needs an injective whole-circle tube excluding other sheets, with local data. | [R03](repairs.md#r03) |
| <a id="d27"></a>D27 | Standard | Appendix B p. 30, (31)–(34) | Holds with repair | The metric error must include both two-dimensional integrals and the F_s term. | [R03](repairs.md#r03) |
| <a id="d28"></a>D28 | Paper | §5 pp. 14–15, Lem. 5.4; Appendix B pp. 30–31 | Holds with repair | Smooth widths, actual support, common sector caps and already-neat boundary inputs complete the construction. | [R03](repairs.md#r03) |
| <a id="d29"></a>D29 | Paper | §5 pp. 14–15, Lem. 5.4(3)/(5); Appendix B p. 29 | Fails (limited scope) | A true corner cannot be a smooth endpoint; tame transport and positive smooth endpoints replace that reading. | [R03](repairs.md#r03) |
| <a id="d30"></a>D30 | Paper | §5 p. 15, Lem. 5.5; Appendix B p. 31 | Holds with repair | A leaf-projectable boundary field with positive normal component enters the open region at positive time. | [R04](repairs.md#r04) |
| <a id="d31"></a>D31 | Standard | Appendix B p. 31, Lem. 5.5 proof | Holds | The tangential-divergence Jacobian bound gives finite O(σ) cost after rounding is fixed. | [R04](repairs.md#r04) |
| <a id="d32"></a>D32 | Standard | §5 pp. 15–16, Lem. 5.6 Step 0 | Holds | Compact transversality gives finite internal circles; uniqueness and π₁-injectivity give discs on both sides. | [R05](repairs.md#r05) |
| <a id="d33"></a>D33 | Paper | §5 p. 16, Lem. 5.6 Step 1 | Holds | Separate inclusion-minimal choices make both patch families nonempty; no common innermost circle is required. | [R05](repairs.md#r05) |
| <a id="d34"></a>D34 | Paper | §5 p. 16, Lem. 5.6 Step 2 | Holds with repair | The connected remainder attached to the ambient boundary lies outside the original corner ball. | [R05](repairs.md#r05) |
| <a id="d35"></a>D35 | Paper | §5 pp. 15–16, Lem. 5.6, (16)–(17) | Holds with repair | Round original sheets and certify two smooth disc endpoints in a slightly larger smooth ball; reverse cost is e. | [R05](repairs.md#r05) |
| <a id="d36"></a>D36 | Paper | §5 p. 17, Lem. 5.6 Step 3, (14) | Holds | Separate disc-area minima give φ(a)≤φ(b), hence G(a)+G(b)≤e. | [R05](repairs.md#r05) |
| <a id="d37"></a>D37 | Standard | §4 p. 12, Lem. 4.9 proof | Holds with repair | Integer stacking proves wall separation; projection is injective only after the two S walls are deleted. | [R06](repairs.md#r06) |
| <a id="d38"></a>D38 | Paper | §4 p. 12, Lem. 4.9 proof | Holds | Opposite sectors allocate all four rays and every input patch exactly once. | [R06](repairs.md#r06) |
| <a id="d39"></a>D39 | Paper | §4 p. 12, Lem. 4.9 proof | Holds with repair | Round in closed regions, then push into opposite open regions inside the injective strip; compare positive scales. | [R06](repairs.md#r06) |
| <a id="d40"></a>D40 | Paper | §4 p. 12, Lem. 4.9 proof | Holds | Boundary-annulus order gives one longitude and one component with boundary per frontier. | [R06](repairs.md#r06) |
| <a id="d41"></a>D41 | Standard | §4 pp. 9–10, Lem. 4.4; p. 12, (7) | Holds | Closed-circle cuts and gluing have zero χ correction; the identity precedes discarding components. | [R06](repairs.md#r06) |
| <a id="d42"></a>D42 | Paper | §4 p. 12, Lem. 4.9 proof | Holds | A seam-free sphere is an impossible input component; an innermost seam gives a forbidden disc patch. | [R06](repairs.md#r06) |
| <a id="d43"></a>D43 | Paper | §4 pp. 11–12, Lem. 4.9(2) | Holds with repair | After Z, shrink rounding and push-off while comparing smooth classes only at positive widths. | [R07](repairs.md#r07) |
| <a id="d44"></a>D44 | Standard | §4 p. 10, Lem. 4.4 | Holds | Each essential compression preserves the longitude and strictly lowers integer genus, ensuring finite termination. | [R06](repairs.md#r06) |
| <a id="d45"></a>D45 | Paper | §4 p. 10, Lem. 4.5 | Holds with repair | The disc's remaining annulus must also lie outside the ball; cleaning then preserves the specified sequence. | [R07](repairs.md#r07) |
| <a id="d46"></a>D46 | Paper | §4 p. 10, Cor. 4.6 | Holds | Transport and clean each preselected step to preserve the final class; pairwise evidence suffices. | [R07](repairs.md#r07) |
| <a id="d47"></a>D47 | Standard | §5 p. 17, T0 proof | Holds | Compact nonempty transverse circles give positive angle/length bounds and an admissible constant width. | [R12](repairs.md#r12) |
| <a id="d48"></a>D48 | Paper | §5 p. 17, T0 proof | Holds | e=0 contradicts two positive disc gains; exclude patches before using frontiers. | [R12](repairs.md#r12) |
| <a id="d49"></a>D49 | Paper | §5 p. 17, clause (c) | Holds | Whole-frontier χ and discarded χ≤0, followed by preselected compressions, give (c). | [R12](repairs.md#r12) |
| <a id="d50"></a>D50 | Paper | §5 p. 17, clause (a) | Holds | Specified-descendant robustness separately against S, A and B proves pairwise (a). | [R07](repairs.md#r07) |
| <a id="d51"></a>D51 | Paper | §5 p. 17, clause (b) | Holds with repair | U*, two-scale avoidance and specified-disc transport preserve ∃ outputs ∀z. | [R07](repairs.md#r07) |
| <a id="d52"></a>D52 | Standard | §5 pp. 17–18, equality branch | Holds | Equality forces discarded χ sum and compression decrease to be zero; no genuine compression remains. | [R06](repairs.md#r06) |
| <a id="d53"></a>D53 | Standard | §5 p. 18, equality branch | Holds | Complete frontiers partition the inputs off measure-zero seams; area equality precedes discarding closed parts. | [R12](repairs.md#r12) |
| <a id="d54"></a>D54 | Paper | §5 p. 18, clause (d) | Holds | Fix gain, then finite cost, then σ; empty compressions make competitors members of the output classes. | [R12](repairs.md#r12) |
| <a id="d55"></a>D55 | Standard | §5 p. 18, T0/T1/T2 split | Holds | Equal/disjoint leaves and interior transversality/tangency exhaust the cases, including already-treated T0. | [R12](repairs.md#r12) |
| <a id="d56"></a>D56 | Standard | §5 pp. 18–19, Prop. 5.7, (21)–(23) | Holds with repair | Linearize height and gradient together; flatten B before perturbing the difference as a height. | [R08](repairs.md#r08) |
| <a id="d57"></a>D57 | Cited | Appendix B p. 31, [4, Thm. 5.8] | Holds | Poincaré makes the bounded bilinear form coercive despite unsigned c; GT original page unchecked. | [R08](repairs.md#r08) |
| <a id="d58"></a>D58 | Cited | Appendix B pp. 31–32, [4, Thm. 8.15] | Holds | Retain the L² term and scale c by R²; GT original page unchecked, with a barrier backup. | [R08](repairs.md#r08) |
| <a id="d59"></a>D59 | Paper | Appendix B pp. 31–32 | Holds with repair | Small-domain positivity and smaller-patch derivative regularity are separate; avoid artificial half-disc corners. | [R08](repairs.md#r08) |
| <a id="d60"></a>D60 | Standard | Appendix B p. 32, (36) | Holds | Division by h removes zero order; determinant normalization adds its derivative to drift. | [R08](repairs.md#r08) |
| <a id="d61"></a>D61 | Cited | Appendix B p. 32, [9, Thm. 4.1] | Holds | The checked author-version boundary diffeomorphism applies; bi-Lipschitz claims stay local away from the pole. | [R08](repairs.md#r08) |
| <a id="d62"></a>D62 | Standard | Appendix B pp. 32–33 | Holds | Change variables without differentiating DF; conformality and determinant one give identity principal matrix. | [R08](repairs.md#r08) |
| <a id="d63"></a>D63 | Paper | Appendix B p. 33 | Holds with repair | Zero-trace combined tests justify reflection; its drift only needs to be bounded. | [R08](repairs.md#r08) |
| <a id="d64"></a>D64 | Standard | Appendix B p. 33, before factorization | Holds with repair | First prove V∈W²,p and w∈W¹,p for p>2 using local Laplace regularity. | [R08](repairs.md#r08) |
| <a id="d65"></a>D65 | Cited | Appendix B p. 33, [18, Ch. III] | Holds | The conjugate equation and standard similarity hypotheses hold; original Vekua pages unchecked. | [R08](repairs.md#r08) |
| <a id="d66"></a>D66 | Paper | §5 p. 19, Prop. 5.7; Appendix B pp. 32–33 | Holds with repair | Positive h and bounded Dh recover df; propagate coincidence; isolation is among tangencies, not all intersections. | [R08](repairs.md#r08) |
| <a id="d67"></a>D67 | Cited | Appendix B p. 32, [4, Thm. 8.19] | Holds | Use the standard principle on v=f/h without zero order, not on the original unsigned-c equation. | [R08](repairs.md#r08) |
| <a id="d68"></a>D68 | Paper | Appendix B p. 32, (24) | Holds | A nonchanging sign gives a zero extremum of v, forces coincidence and contradicts distinct classes. | [R08](repairs.md#r08) |
| <a id="d69"></a>D69 | Paper | Appendix B p. 33, Prop. 5.7(2) proof | Holds | A finite boundary cover gives df≠0 on the whole open collar without a boundary-uniform positive bound. | [R08](repairs.md#r08) |
| <a id="d70"></a>D70 | Standard | Appendix B p. 33, Prop. 5.7(3) proof | Holds | Tangencies are a closed discrete subset of a compact region separated from the boundary. | [R08](repairs.md#r08) |
| <a id="d71"></a>D71 | Paper | Appendix B p. 33, Lem. B.1 | Holds with repair | Taylor bounds work with max{1,Λ}, correcting the Λ=0 denominator before t. | [R09](repairs.md#r09) |
| <a id="d72"></a>D72 | Paper | Appendix B p. 34, T2 perturbation | Holds with repair | Keep F_t=f+ςtχ throughout the collar; fixed transition-band control gives transversality and the same class. | [R09](repairs.md#r09) |
| <a id="d73"></a>D73 | Paper | Appendix B p. 34, Lem. B.2 | Holds with repair | Through-arcs and Jordan-disc extrema exclude collapse in three cases without a boundary-uniform gradient bound. | [R09](repairs.md#r09) |
| <a id="d74"></a>D74 | Standard | Appendix B pp. 34–35, Cor. B.4(1) | Holds | Quotient distance loses at most ball-diameter sum, without bounding circle entry/exit counts. | [R09](repairs.md#r09) |
| <a id="d75"></a>D75 | Paper | Appendix B pp. 34–35, Lem. B.3 | Holds with repair | Actual F_t, quotient length, band crossing and essential projection give a fixed positive good length. | [R09](repairs.md#r09) |
| <a id="d76"></a>D76 | Paper | Appendix B p. 35, Cor. B.4(2) | Holds | A compact thick transverse set transfers two-sided angle bounds to the protected good region. | [R10](repairs.md#r10) |
| <a id="d77"></a>D77 | Paper | Appendix B pp. 35–36, Cor. B.4(3) | Holds with repair | Buffered single-arc charts exclude foreign branches/sheets; only good-region local data are uniform. | [R10](repairs.md#r10) |
| <a id="d78"></a>D78 | Paper | Appendix B p. 37, (44) | Holds with repair | Fixed q and a t-dependent positive floor satisfy every pointwise cap with an exact good-region platform. | [R10](repairs.md#r10) |
| <a id="d79"></a>D79 | Paper | Appendix B p. 36, T2 no-patch argument | Holds with repair | Unify β and caps, construct widths for every small t, then compare fixed ε* against e(t). | [R10](repairs.md#r10) |
| <a id="d80"></a>D80 | Paper | Appendix B p. 36, class comparison | Holds with repair | Pair isotopy needs coherent common-positive-width smooth tracks, followed by endpoint width interpolation. | [R11](repairs.md#r11) |
| <a id="d81"></a>D81 | Paper | Appendix B p. 36, clause (b) | Holds with repair | Choose outputs/sequences first; later t, width and push-off changes only realize the same classes. | [R07](repairs.md#r07) |
| <a id="d82"></a>D82 | Paper | Appendix B pp. 36–37, T2 conclusion | Holds with repair | Unified constants close the budget; (d) stays in the genus-equality/no-compression branch. | [R12](repairs.md#r12) |
| <a id="d83"></a>D83 | Paper | Appendix B pp. 37–38, T1 setup | Holds with repair | Flatten B, use constant cores, keep boundary fixed and intersection away from it; e≥0 tends to zero. | [R09](repairs.md#r09) |
| <a id="d84"></a>D84 | Paper | Appendix B p. 38, Lem. B.5 | Holds with repair | Verify diameter, quotient length, angles, full tubes and boundary safety after deleting collar conditions. | [R10](repairs.md#r10) |
| <a id="d85"></a>D85 | Paper | Appendix B pp. 38–39, T1 no-patch argument | Holds with repair | Ball-only exact platforms and unified gain fix ε* before t; e→0 excludes patches. | [R10](repairs.md#r10) |
| <a id="d86"></a>D86 | Paper | Appendix B p. 39, T1 conclusion | Holds with repair | Fixed classes, two scales, specified descendants and the equality-branch area budget give every clause. | [R12](repairs.md#r12) |
| <a id="d87"></a>D87 | Paper | Thm. 5.1 p. 13; §5 pp. 17–19; Appendix B pp. 36–39 | Holds | Complete E*/U*, standard analysis and accepted replacements give (a)–(d) in the original quantifier order. | [R12](repairs.md#r12) |
