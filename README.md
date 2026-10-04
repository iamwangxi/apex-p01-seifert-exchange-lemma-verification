# Seifert Theorem 5.1: paper verification

[中文说明](README.zh-CN.md)

**Result.** Within the scope of treating the complete statements of the cited external theorems as black boxes, checking their applicability, and using the accepted repairs for the target paper's own reasoning, Theorem 5.1(a)–(d) holds. The original proof requires corrections. No major flaw has been established by this verification.

## Target and version

The target is Apex Intelligence, *Contractibility of the Complex of Incompressible Seifert Surfaces: The Knot Case of Kakimizu’s Problem*, dated **11 September 2026**, the official competition PDF, **Theorem 5.1 (Incompressible exchange lemma), printed p. 13**. Its proof runs through §5 and the relevant material in §§3–4 and Appendices A–B.

- PDF identifier: `seifert-surfaces.pdf`.
- PDF SHA-256: `34f17d7d99780d3fd3626d9e5d7b35d6aa76661c404f191b6df341b300c0c06f`.
- Verification package: **v1.0, 4 October 2026**.
- Page references throughout this repository are **printed page numbers**, accompanied by theorem, lemma, section or equation identifiers. Extracted-text line numbers are not citation locators.

The PDF hash identifies the exact target even if the distribution filename changes. The target PDF is not redistributed here. Later versions do not retroactively supply arguments missing from this version.

## Statement being checked

For a non-trivial knot $K$, let $x,u,w$ be vertices of $IS(K)$ with

$$
\mathrm{dist}(x,u)=\mathrm{dist}(x,w)=1,
\qquad \mathrm{dist}(u,w)=2.
$$

Write $v\sim_{=}q$ for equality or adjacency. There are vertices $w_\uparrow,w_\downarrow$, chosen before any later common neighbour $z$, such that:

1. **(a)** Each output is equal or adjacent to each of $x,u,w$.
2. **(b)** Every $z$ equal or adjacent to both $u,w$ is equal or adjacent to both outputs.
3. **(c)** $g(w_\uparrow)+g(w_\downarrow)\le g(u)+g(w)$.
4. **(d)** If equality holds in (c), then $A(w_\uparrow)+A(w_\downarrow)<A(u)+A(w)$.

Here $A(v)$ is the infimum of relative area in the smooth neat vertex class with boundary a leaf of the fixed longitude foliation. The essential order is $\forall(x,u,w)\,\exists(w_\uparrow,w_\downarrow)\,\forall z$. There is no claim of a canonical choice, uniqueness, or simultaneous disjointness of all the classes involved.

## Scope and method

This is an offline, structured paper verification, not a formal proof certificate. The proof was checked in three parallel line-by-line passes, followed by an adversarial review that tried to refute their verdicts and a cross-model spot check of the key claims against the sources; where the adversarial review corrected a pass, its correction is used. This package consolidates the results.

The proof was divided into 87 input or inference steps. Checks covered hypotheses of external statements, smooth versus piecewise smooth categories, local elliptic arguments, legal competitors in area comparisons, quantitative support and gain bounds, and the order in which representatives, parameters and compression descendants are chosen. Local countermodels were used to test particular inferences; none is asserted to be a global counterexample to Theorem 5.1.

| Classification | Count |
|---|---:|
| Cited external result | 16 |
| Paper argument or substantive interface | 51 |
| Standard fact or calculation | 20 |
| **Total** | **87** |

| Verdict on the original step | Count |
|---|---:|
| Holds | 45 |
| Holds with repair | 37 |
| Unresolved | 3 |
| Fails in the specified reading/application | 2 |

These are verdicts on the original decomposed steps. They include conditional inferences and applicability checks of black-box statements. A repaired replacement does not turn the original sentence into a passed step.

## Corrections needed

- Replace the body's calls to **Theorem A.6 and Lemma A.7** by the complete **E(ii)** already cited in §3: Schultens Theorem 2 / Kapovich Appendix Corollary 11 in the checked preprint, followed by an **independent Hopf transversality argument**. The body actually calls Appendix A; this is a replacement route, not a claim that Appendix A was never used.
- **D29:** retain the negative verdict only for the smooth ambient-isotopy reading of a genuine corner endpoint. Use tame isotopy to transport the corner object's topology, and smooth isotopy only between positive-width smooth endpoints. The paper's piecewise smooth convention prevents a blanket rejection under every category reading.
- **D28/D35:** use smooth positive widths, actual geometric support bounds and four-sector common data; certify the smooth disc-swap competitors inside a **slightly larger smooth three-ball**.
- **D43/D80/D81:** shrink both rounding and push-off scales, compare positive-parameter smooth tracks, and transport **preselected compression descendants**. Output classes remain fixed before $z$.
- **D77–D79:** obtain uniform data only on a buffered good region; unify the gain coefficient and all width caps, fix $\varepsilon_*$ first, and choose $t$ afterwards.
- Add **[10, p. 228]** for irreducibility of the knot exterior. Additional local analytic, category and citation corrections are detailed in [repairs.md](proof/repairs.md).

## Limits and open matters

**D09** (the FHS adaptation) and **D10** (Kapovich's direct use of Anderson Theorem 3.1 beyond its truncated-surface conclusion) limit the independent verification of the cited literature's printed proofs. They do not establish that the published statements are false. **D12 and D22** leave Appendix A's internal existence route unclosed; the replacement route does not prove that appendix or equality of the smooth and auxiliary piecewise smooth infima.

Gilbarg–Trudinger, Vekua, Wall and Schoen 1983 were used at the level of standard textbook statements without comparison against the original books/chapters. The checked Schultens source is arXiv:0707.3926v4, not a page-by-page comparison with the journal version. FHS text is OCR and may misrecognise formulas. See [open-items.md](proof/open-items.md) and [bibliography.md](sources/bibliography.md).

The result does not certify all 87 steps independently, the target paper as a whole, Theorems A/C/D, Appendix C, or any later version's new existence proof. It is not certification by a human expert.

## Repository guide

| File | Purpose |
|---|---|
| [README.zh-CN.md](README.zh-CN.md) | Corresponding Chinese overview |
| [proof/dependency-map.md](proof/dependency-map.md) | Seven-block overview and detailed Mermaid subgraphs; black-box and unresolved branches distinguished |
| [proof/step-verification.md](proof/step-verification.md) | All 87 steps: type, competition-version locator, verdict, reason and repair link |
| [proof/repairs.md](proof/repairs.md) | Full English repair arguments and unified quantitative interfaces |
| [proof/open-items.md](proof/open-items.md) | Unclosed proof routes and source-verification limits, with their effects |
| [sources/bibliography.md](sources/bibliography.md) | Source editions, checked results/pages, acquisition provenance and OCR status |
| [LICENSE](LICENSE) | CC BY 4.0 scope and attribution |
| [MANIFEST.sha256](MANIFEST.sha256) | SHA-256 of every other file in this package |

Mermaid diagrams use GitHub's native Markdown rendering. On macOS, integrity can be checked from the repository root with `shasum -a 256 -c MANIFEST.sha256`; systems with GNU coreutils can use `sha256sum -c MANIFEST.sha256`. The manifest checks bytes, not mathematical correctness.

## AI disclosure

GPT-6.1 Sol performed the step decomposition, the line-by-line checks and an adversarial review, and drafted this package, in OpenAI Codex under human direction; Claude planned the process, checked key claims against the sources and reviewed the final text. No human expert has certified the work.

## License

Original repository prose is licensed under **CC BY 4.0**, to the extent applicable rights exist. Attribute it to the **apex-p01-seifert-exchange-lemma-verification contributors**, link the license and indicate changes; include the repository URL and version when available. The target paper and third-party publications retain their own rights and are not included in this grant. See [LICENSE](LICENSE).
