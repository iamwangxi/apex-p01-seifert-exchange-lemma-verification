# Dependency map

Version 1.0 · 4 October 2026. [Step table](step-verification.md) · [Repairs](repairs.md) · [Open items](open-items.md)

First comes the seven-block overview, then a type legend and a subgraph for each block. Arrows run **from input to dependent step**. Solid arrows describe repaired local dependencies or applicability inputs to accepted complete external statements. Dashed arrows mark a printed-proof audit or an original unclosed existence route; they do not certify those branches. Block arrows aggregate dependencies, rather than asserting that every step in one block depends on every step in the other.

## Seven-block overview

```mermaid
flowchart TD
  B1["1 · D01–D11: setup and external inputs"]
  B2["2 · D12–D24: Appendix A and replacement supply"]
  B3["3 · D25–D36: rounding, push-off, disc swaps"]
  B4["4 · D37–D54: frontiers, compression, T0"]
  B5["5 · D55–D70: configurations and PDE tangencies"]
  B6["6 · D71–D82: T2 gain and fixed outputs"]
  B7["7 · D83–D87: T1 and assembly"]
  B1 -->|"complete E(ii), U; independent Hopf"| B2
  B1 -.->|"HS and Fin: internal existence route unclosed"| B2
  B1 --> B3
  B2 --> B3
  B2 --> B4
  B3 --> B4
  B2 --> B5
  B5 --> B6
  B3 --> B6
  B4 --> B6
  B5 --> B7
  B6 --> B7
  B4 -->|"T0 conclusions"| B7
```

## Type and edge legend

```mermaid
flowchart LR
  C["Cited · external statement"]:::cited
  P["Paper · construction or substantive interface"]:::paper
  S["Standard · fact or calculation"]:::standard
  O["Unresolved or limited-scope failure"]:::audit
  C -->|"accepted interface"| P
  O -.->|"proof audit or unclosed route"| P
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

Types are **16 Cited, 51 Paper, 20 Standard**, independent of verdict. Red dashed borders add warnings without changing a step's type. Verdicts are in the step table. Shared input nodes repeated in another block do not count as new steps. Conditional Appendix regularity arrows mean **given an A.1 minimizer**, not a completed existence proof.

## 1. Setup and external inputs (D01–D11)

```mermaid
flowchart TD
  D01["D01 · Collar geometry"]:::standard
  D02["D02 · Exterior irreducibility"]:::cited
  D03["D03 · Surface and vertex class"]:::standard
  D04["D04 · Neat isotopy extension"]:::cited
  D05["D05 · Fixed-boundary attainment"]:::cited
  D06["D06 · Complete relative attainment"]:::cited
  D07["D07 · Compactness and finite blocks"]:::cited
  D08["D08 · Universal disjointness"]:::cited
  D09["D09 · FHS boundary adaptation"]:::cited
  D10["D10 · Anderson direct application"]:::cited
  D11["D11 · Interior stability estimate"]:::cited
  D01 --> D05
  D02 --> D05
  D03 --> D05
  D01 --> D06
  D02 --> D06
  D03 --> D06
  D05 -.->|"external printed-proof audit"| D06
  D07 -.->|"external printed-proof audit"| D06
  D10 -.->|"external printed-proof audit"| D07
  D11 -.->|"external printed-proof audit"| D07
  D09 -.->|"external printed-proof audit"| D08
  class D09 audit
  class D10 audit
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

D05/D07 → D06 and D09 → D08 expand the printed proofs behind the complete E/U statements; D10/D11 → D07 audits Fin. The dashed branches remain incomplete at proof level. In the body, D06–D08 are used as accepted complete statement interfaces.

## 2. Appendix A and replacement supply (D12–D24)

```mermaid
flowchart TD
  D01["D01 · Collar geometry · shared"]:::standard
  D03["D03 · Surface and vertex class · shared"]:::standard
  D04["D04 · Neat isotopy extension · shared"]:::cited
  D05["D05 · Fixed-boundary attainment · shared"]:::cited
  D06["D06 · Complete relative attainment · shared"]:::cited
  D07["D07 · Compactness and finite blocks · shared"]:::cited
  D08["D08 · Universal disjointness · shared"]:::cited
  D12["D12 · Attained A.1 membership"]:::paper
  D13["D13 · Stationarity and conormals"]:::paper
  D14["D14 · Cross-edge regularity"]:::paper
  D15["D15 · Gradient and boundary regularity"]:::cited
  D16["D16 · Hopf boundary lemma"]:::cited
  D17["D17 · Hopf drift and curved balls"]:::paper
  D18["D18 · Interior vertex removal"]:::paper
  D19["D19 · Boundary vertex angle"]:::paper
  D20["D20 · Boundary graph smoothing"]:::paper
  D21["D21 · Properness and stability"]:::standard
  D22["D22 · Sliding attainment assembly"]:::paper
  D23["D23 · Independent neatness"]:::paper
  D24["D24 · Fix S, A, B"]:::paper
  D05 -.->|"membership unclosed"| D12
  D12 --> D13
  D13 --> D14
  D15 --> D14
  D01 --> D17
  D16 --> D17
  D14 --> D18
  D15 --> D18
  D12 --> D18
  D12 --> D19
  D14 --> D19
  D17 --> D19
  D19 --> D20
  D15 --> D20
  D18 --> D21
  D20 --> D21
  D12 --> D21
  D05 --> D22
  D12 -.->|"membership unclosed"| D22
  D18 --> D22
  D20 --> D22
  D21 --> D22
  D07 --> D22
  D04 --> D22
  D01 --> D23
  D16 --> D23
  D06 --> D23
  D22 -.->|"original route, unclosed"| D23
  D06 --> D24
  D22 -.->|"original route, unclosed"| D24
  D23 --> D24
  D08 --> D24
  D04 --> D24
  D03 --> D24
  class D12 audit
  class D22 audit
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

The accepted body path is D06 → independent D23 Hopf → D24. D12/D22 leave the internal existence route unclosed. D13–D21 regularity is conditional and cannot manufacture an A.1 minimizer. The D22 alternatives are shown only as the original route.

## 3. Rounding, push-off and disc swaps (D25–D36)

```mermaid
flowchart TD
  D02["D02 · Exterior irreducibility · shared"]:::cited
  D03["D03 · Surface and vertex class · shared"]:::standard
  D04["D04 · Neat isotopy extension · shared"]:::cited
  D06["D06 · Complete relative attainment · shared"]:::cited
  D22["D22 · Sliding attainment assembly · shared"]:::paper
  D23["D23 · Independent neatness · shared"]:::paper
  D25["D25 · Rounding profile and gain"]:::standard
  D26["D26 · Whole-circle safe coordinates"]:::paper
  D27["D27 · True area-density error"]:::standard
  D28["D28 · Admissible smooth rounding"]:::paper
  D29["D29 · Corner versus smooth isotopy"]:::paper
  D30["D30 · Leaf-compatible push-off"]:::paper
  D31["D31 · Finite push-off area cost"]:::standard
  D32["D32 · Intersection circles and discs"]:::standard
  D33["D33 · Separate innermost families"]:::paper
  D34["D34 · Empty-side ball placement"]:::paper
  D35["D35 · Smooth swap competitors"]:::paper
  D36["D36 · Two-circle gain inequality"]:::paper
  D03 --> D26
  D25 --> D27
  D26 --> D27
  D25 --> D28
  D26 --> D28
  D27 --> D28
  D28 --> D29
  D04 --> D29
  D23 --> D30
  D28 --> D30
  D29 --> D30
  D30 --> D31
  D03 --> D32
  D32 --> D33
  D32 --> D34
  D33 --> D34
  D02 --> D34
  D28 --> D34
  D29 --> D34
  D34 --> D35
  D28 --> D35
  D29 --> D35
  D06 --> D35
  D22 -.->|"original route, unclosed"| D35
  D33 --> D36
  D35 --> D36
  class D22 audit
  class D29 audit
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

D29 uses tame corner transport and positive-width smooth endpoint comparison. D35 additionally needs the slightly larger smooth three-ball of R05. R03 supplies the same four-sector widths and common gain to frontiers and disc swaps.

## 4. Frontiers, compression and T0 (D37–D54)

```mermaid
flowchart TD
  D02["D02 · Exterior irreducibility · shared"]:::cited
  D03["D03 · Surface and vertex class · shared"]:::standard
  D04["D04 · Neat isotopy extension · shared"]:::cited
  D06["D06 · Complete relative attainment · shared"]:::cited
  D08["D08 · Universal disjointness · shared"]:::cited
  D22["D22 · Sliding attainment assembly · shared"]:::paper
  D24["D24 · Fix S, A, B · shared"]:::paper
  D28["D28 · Admissible smooth rounding · shared"]:::paper
  D29["D29 · Corner versus smooth isotopy · shared"]:::paper
  D30["D30 · Leaf-compatible push-off · shared"]:::paper
  D31["D31 · Finite push-off area cost · shared"]:::standard
  D32["D32 · Intersection circles and discs · shared"]:::standard
  D36["D36 · Two-circle gain inequality · shared"]:::paper
  D37["D37 · Wall-deleted cyclic strip"]:::standard
  D38["D38 · Opposite frontier sectors"]:::paper
  D39["D39 · Smooth coarse frontiers"]:::paper
  D40["D40 · One boundary per frontier"]:::paper
  D41["D41 · Whole-frontier Euler account"]:::standard
  D42["D42 · No discarded spheres"]:::paper
  D43["D43 · Two-scale avoidance"]:::paper
  D44["D44 · Finite genus-lowering compression"]:::standard
  D45["D45 · Clean specified compressing discs"]:::paper
  D46["D46 · Specified descendant adjacency"]:::paper
  D47["D47 · T0 positive common width"]:::standard
  D48["D48 · T0 excludes disc patches"]:::paper
  D49["D49 · Genus inequality and fixed outputs"]:::paper
  D50["D50 · Adjacency to three inputs"]:::paper
  D51["D51 · Outputs before common neighbour"]:::paper
  D52["D52 · Equality excludes compression"]:::standard
  D53["D53 · Whole-frontier area partition"]:::standard
  D54["D54 · Strict area budget in T0"]:::paper
  D03 --> D37
  D24 --> D37
  D37 --> D38
  D38 --> D39
  D28 --> D39
  D29 --> D39
  D30 --> D39
  D37 --> D40
  D38 --> D40
  D39 --> D40
  D38 --> D41
  D32 --> D42
  D38 --> D42
  D40 --> D42
  D39 --> D43
  D29 --> D43
  D04 --> D43
  D03 --> D44
  D02 --> D45
  D03 --> D45
  D04 --> D45
  D45 --> D46
  D24 --> D47
  D28 --> D47
  D36 --> D48
  D47 --> D48
  D40 --> D49
  D41 --> D49
  D42 --> D49
  D48 --> D49
  D44 --> D49
  D39 --> D50
  D46 --> D50
  D49 --> D50
  D08 --> D51
  D06 --> D51
  D22 -.->|"original route, unclosed"| D51
  D43 --> D51
  D46 --> D51
  D49 --> D51
  D44 --> D52
  D49 --> D52
  D38 --> D53
  D24 --> D53
  D28 --> D54
  D30 --> D54
  D31 --> D54
  D47 --> D54
  D52 --> D54
  D53 --> D54
  NP["No-disc-patch premise: D48 / D79 / D85 by case"]:::paper
  NP --> D42
  class D22 audit
  class D29 audit
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

D42 has the separate no-disc-patch premise established by D48, D79 or D85 in its configuration. D43/D51 use two scales; D45/D46 preserve specified descendants. D54 uses D52’s genus-equality/no-compression branch.

## 5. Configurations and elliptic tangencies (D55–D70)

```mermaid
flowchart TD
  D01["D01 · Collar geometry · shared"]:::standard
  D15["D15 · Gradient and boundary regularity · shared"]:::cited
  D23["D23 · Independent neatness · shared"]:::paper
  D24["D24 · Fix S, A, B · shared"]:::paper
  D55["D55 · Exhaustive configurations"]:::standard
  D56["D56 · Full double-graph linearization"]:::standard
  D57["D57 · Small-domain weak solution"]:::cited
  D58["D58 · Scaled supremum estimate"]:::cited
  D59["D59 · Positive h and bounded Dh"]:::paper
  D60["D60 · Zero-order removal and normalization"]:::standard
  D61["D61 · Boundary isothermal coordinates"]:::cited
  D62["D62 · Weak density transformation"]:::standard
  D63["D63 · Weak odd reflection"]:::paper
  D64["D64 · Sobolev entry to similarity"]:::standard
  D65["D65 · Similarity factorization"]:::cited
  D66["D66 · Critical-point isolation"]:::paper
  D67["D67 · Strong maximum principle"]:::cited
  D68["D68 · Interior sign change"]:::paper
  D69["D69 · No-critical open collar"]:::paper
  D70["D70 · Finite interior tangencies"]:::standard
  D01 --> D55
  D24 --> D55
  D24 --> D56
  D23 --> D56
  D56 --> D59
  D57 --> D59
  D58 --> D59
  D15 --> D59
  D59 --> D60
  D60 --> D61
  D60 --> D62
  D61 --> D62
  D62 --> D63
  D62 --> D64
  D63 --> D64
  D64 --> D65
  D59 --> D66
  D61 --> D66
  D65 --> D66
  D24 --> D66
  D59 --> D68
  D60 --> D68
  D67 --> D68
  D66 --> D68
  D66 --> D69
  D55 --> D70
  D66 --> D70
  D69 --> D70
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

D63 is used only for the boundary case; D64 supplies the Sobolev entry before D65. D66 isolates tangencies, not the whole intersection. D69 gives a no-critical open collar, not a positive gradient bound up to the boundary.

## 6. T2 uniform gain and fixed outputs (D71–D82)

```mermaid
flowchart TD
  D04["D04 · Neat isotopy extension · shared"]:::cited
  D06["D06 · Complete relative attainment · shared"]:::cited
  D08["D08 · Universal disjointness · shared"]:::cited
  D22["D22 · Sliding attainment assembly · shared"]:::paper
  D24["D24 · Fix S, A, B · shared"]:::paper
  D26["D26 · Whole-circle safe coordinates · shared"]:::paper
  D28["D28 · Admissible smooth rounding · shared"]:::paper
  D29["D29 · Corner versus smooth isotopy · shared"]:::paper
  D31["D31 · Finite push-off area cost · shared"]:::standard
  D36["D36 · Two-circle gain inequality · shared"]:::paper
  D39["D39 · Smooth coarse frontiers · shared"]:::paper
  D40["D40 · One boundary per frontier · shared"]:::paper
  D41["D41 · Whole-frontier Euler account · shared"]:::standard
  D42["D42 · No discarded spheres · shared"]:::paper
  D43["D43 · Two-scale avoidance · shared"]:::paper
  D44["D44 · Finite genus-lowering compression · shared"]:::standard
  D46["D46 · Specified descendant adjacency · shared"]:::paper
  D52["D52 · Equality excludes compression · shared"]:::standard
  D53["D53 · Whole-frontier area partition · shared"]:::standard
  D56["D56 · Full double-graph linearization · shared"]:::standard
  D66["D66 · Critical-point isolation · shared"]:::paper
  D68["D68 · Interior sign change · shared"]:::paper
  D69["D69 · No-critical open collar · shared"]:::paper
  D70["D70 · Finite interior tangencies · shared"]:::standard
  D71["D71 · Fixed sign arc and r1"]:::paper
  D72["D72 · Actual smooth perturbation"]:::paper
  D73["D73 · Noncollapsing circles"]:::paper
  D74["D74 · Collapsed-ball quotient length"]:::standard
  D75["D75 · Uniform good-region length"]:::paper
  D76["D76 · Buffered angle lower bound"]:::paper
  D77["D77 · Whole-intersection safe tube"]:::paper
  D78["D78 · Exact smooth width platform"]:::paper
  D79["D79 · Gain fixed before t"]:::paper
  D80["D80 · Positive-parameter output classes"]:::paper
  D81["D81 · Fixed descendants for later z"]:::paper
  D82["D82 · T2 four-clause completion"]:::paper
  D69 --> D71
  D56 --> D72
  D66 --> D72
  D69 --> D72
  D70 --> D72
  D71 --> D72
  D24 --> D72
  D72 --> D73
  D66 --> D73
  D68 --> D73
  D69 --> D73
  D73 --> D74
  D70 --> D74
  D71 --> D75
  D72 --> D75
  D74 --> D75
  D66 --> D76
  D69 --> D76
  D72 --> D76
  D74 --> D76
  D26 --> D77
  D72 --> D77
  D76 --> D77
  D28 --> D78
  D77 --> D78
  D75 --> D78
  D36 --> D79
  D75 --> D79
  D76 --> D79
  D77 --> D79
  D78 --> D79
  D72 --> D79
  D72 --> D80
  D04 --> D80
  D29 --> D80
  D39 --> D80
  D44 --> D80
  D80 --> D81
  D43 --> D81
  D46 --> D81
  D08 --> D81
  D06 --> D81
  D22 -.->|"original route, unclosed"| D81
  D79 --> D82
  D80 --> D82
  D39 --> D82
  D40 --> D82
  D41 --> D82
  D42 --> D82
  D44 --> D82
  D46 --> D82
  D52 -->|"bookkeeping argument reuse"| D82
  D53 -->|"bookkeeping argument reuse"| D82
  D31 --> D82
  class D22 audit
  class D29 audit
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

D75 needs only D74, the quotient-length part of B.4. D77 independently supplies local geometry; D28 enters D78’s rounding interface rather than proving D77’s uniform tube. R10 recomputes every cap and gain, fixing ε* before t; R11 completes D80’s smooth class comparison.

## 7. T1 and theorem assembly (D83–D87)

```mermaid
flowchart TD
  D24["D24 · Fix S, A, B · shared"]:::paper
  D28["D28 · Admissible smooth rounding · shared"]:::paper
  D31["D31 · Finite push-off area cost · shared"]:::standard
  D36["D36 · Two-circle gain inequality · shared"]:::paper
  D39["D39 · Smooth coarse frontiers · shared"]:::paper
  D40["D40 · One boundary per frontier · shared"]:::paper
  D41["D41 · Whole-frontier Euler account · shared"]:::standard
  D42["D42 · No discarded spheres · shared"]:::paper
  D43["D43 · Two-scale avoidance · shared"]:::paper
  D44["D44 · Finite genus-lowering compression · shared"]:::standard
  D45["D45 · Clean specified compressing discs · shared"]:::paper
  D46["D46 · Specified descendant adjacency · shared"]:::paper
  D49["D49 · Genus inequality and fixed outputs · shared"]:::paper
  D50["D50 · Adjacency to three inputs · shared"]:::paper
  D51["D51 · Outputs before common neighbour · shared"]:::paper
  D52["D52 · Equality excludes compression · shared"]:::standard
  D53["D53 · Whole-frontier area partition · shared"]:::standard
  D54["D54 · Strict area budget in T0 · shared"]:::paper
  D55["D55 · Exhaustive configurations · shared"]:::standard
  D56["D56 · Full double-graph linearization · shared"]:::standard
  D66["D66 · Critical-point isolation · shared"]:::paper
  D68["D68 · Interior sign change · shared"]:::paper
  D70["D70 · Finite interior tangencies · shared"]:::standard
  D73["D73 · Noncollapsing circles · shared"]:::paper
  D74["D74 · Collapsed-ball quotient length · shared"]:::standard
  D76["D76 · Buffered angle lower bound · shared"]:::paper
  D77["D77 · Whole-intersection safe tube · shared"]:::paper
  D78["D78 · Exact smooth width platform · shared"]:::paper
  D80["D80 · Positive-parameter output classes · shared"]:::paper
  D81["D81 · Fixed descendants for later z · shared"]:::paper
  D82["D82 · T2 four-clause completion · shared"]:::paper
  D83["D83 · T1 interior perturbation"]:::paper
  D84["D84 · T1 good-region interfaces"]:::paper
  D85["D85 · T1 gain and no patches"]:::paper
  D86["D86 · T1 four-clause completion"]:::paper
  D87["D87 · Conditional theorem assembly"]:::paper
  D55 --> D83
  D56 --> D83
  D66 --> D83
  D68 --> D83
  D70 --> D83
  D24 --> D83
  D83 --> D84
  D73 -->|"interior-only argument reuse"| D84
  D74 -->|"interior-only argument reuse"| D84
  D76 -->|"interior-only argument reuse"| D84
  D77 -->|"interior-only argument reuse"| D84
  D84 --> D85
  D28 --> D85
  D36 --> D85
  D78 -->|"ball-only platform reuse"| D85
  D83 --> D85
  D85 --> D86
  D80 --> D86
  D81 --> D86
  D39 --> D86
  D40 --> D86
  D41 --> D86
  D42 --> D86
  D43 --> D86
  D44 --> D86
  D45 --> D86
  D46 --> D86
  D52 -->|"bookkeeping argument reuse"| D86
  D53 -->|"bookkeeping argument reuse"| D86
  D31 --> D86
  D24 --> D87
  D49 --> D87
  D50 --> D87
  D51 --> D87
  D54 --> D87
  D55 --> D87
  D81 --> D87
  D82 --> D87
  D86 --> D87
  classDef cited fill:#e8f1ff,stroke:#265b99,color:#152238
  classDef paper fill:#fff1dd,stroke:#946000,color:#322200
  classDef standard fill:#edf5ed,stroke:#427044,color:#163518
  classDef audit stroke:#ad2929,stroke-width:3px,stroke-dasharray:5 3
```

D84 uses the interior-only versions of diameter, quotient, angle and tube arguments. D85 uses newly unified gains/platforms. D86 retains genus equality before the area step. D87 is the conditional repaired conclusion, not independent certification of all cited printed proofs.

## Choice order and scope

Fixed minima → fixed perturbation scheme → diameter and ball scales → good-region length → buffered local geometry → common caps/platform → fixed ε* → small-parameter threshold → t → bad-region floor → rounding → finite push-off cost → push-off time. The coarse output classes and specified compression descendants are fixed before any later z; after z, the parameter and both geometric scales may change within those same classes.

The later-neighbour representatives need not retain the area branch's quantitative gain. No edge runs from the desired no-disc-patch conclusion back to the width or competitor construction. Appendix A membership/sequence debts and external printed-proof issues are retained in the open-items file.
