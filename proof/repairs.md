# Repairs and corrected proof interfaces

Version 1.0 · 4 October 2026. [Overview](../README.md) · [87-step table](step-verification.md) · [Open items](open-items.md) · [Sources](../sources/bibliography.md)

These are the accepted local repairs and their common interfaces, consolidated from the supplied verification records with the adversarial corrections taking precedence. They give a **conditional repaired body proof** of Theorem 5.1(a)–(d). They are not a certification of Appendix A's existence route or of the printed proofs of all external statements. No completed repair for D09/D10/D12/D22 is claimed; their effects are in [open-items.md](open-items.md).

## Notation and reading order

Let $M=E(K)$, with the fixed relative metric and longitude-leaf family $J$. Fix minima $S\in x$, $A\in w$, $B\in u$. In the perturbation arguments $A_0=A$, $[A_t]=w$, and $e(t)=\operatorname{Area}(A_t)-\operatorname{Area}(A_0)\ge0$. A “neat” surface is smooth and proper, transverse to the ambient boundary. Isotopy extension preserves $\partial M$ **setwise** unless a relative-collar condition is expressly imposed.

To avoid confusing a minimum surface $B$ with a rounded frontier, rounded frontiers below are denoted $\widehat T$. The positive auxiliary PDE solution is $h$; the actual perturbed graph difference is $F_t$. The common gain coefficient is always $\beta$, replacing the incompatible numerical uses of $g_0$ in the separate route computations.

| Repair | Main nodes |
|---|---|
| [R01](#r01) Supply, category and independent Hopf | D01–D08, D11, D16, D23–D24 |
| [R02](#r02) Conditional Appendix A regularity | D13–D23 |
| [R03](#r03) Rounding, support, common caps and D29 | D25–D29 |
| [R04](#r04) Leaf-compatible push-off and cost | D30–D31 |
| [R05](#r05) Disc swaps and smooth competitor certification | D32–D36 |
| [R06](#r06) Cover, frontiers, Euler characteristic and compression | D37–D42, D44, D49, D52–D53 |
| [R07](#r07) Two scales and specified descendants | D43, D45–D46, D50–D51, D81 |
| [R08](#r08) Full elliptic/tangency argument | D56–D70 |
| [R09](#r09) Perturbation, diameter and good-region length | D71–D75, D83–D84 |
| [R10](#r10) Buffered tubes, exact platform and unified gain | D76–D79, D84–D85 |
| [R11](#r11) Positive-parameter smooth output classes | D80–D81 |
| [R12](#r12) T0/T1/T2 and all four conclusions | D47–D55, D82–D87 |
| [R13](#r13) Correction index and citation precision | Editorial and source-locator corrections |

<a id="r01"></a>
## R01 — Replace the body's Appendix A calls by complete E(ii) and independent Hopf

**Competition locators:** §3, pp. 6–8, equations (2)–(3), Theorems 3.1–3.3 and Remark 3.4; Lemma 4.3, p. 9; §5 opening p. 13 and double-graph inputs pp. 18–19. **External locators:** Schultens preprint Theorems 2/4, p. 4; Appendix setup pp. 18–19; Corollary 11 and Theorem 12, p. 20.

### Environmental and class conditions

In the inward collar $g=dr^2+\phi(r)^2g_T$, $\phi=1-r$, a vector $v=a\partial_r+X$ satisfies

$$
\operatorname{Hess}r(v,v)=\phi\phi'|X|_{g_T}^2\le0.
$$

With the paper's convention $II(X,Y)=\langle\nabla_XY,\partial_r\rangle$, at $r=0$ one has $II=g_T$, trace 2. This supplies the local strictly convex barrier, not a globally strictly convex defining function on the knot exterior. Extending the same collar to negative $r$ supplies a smooth isometric exterior extension and uniform local geometry on compact charts.

The exterior is compact and orientable. Kakimizu p. 228 records irreducibility for a non-split link exterior; a knot is non-split. Alternatively an embedded sphere in $S^3$ has a ball side disjoint from the connected tubular neighbourhood of the knot. Orientability excludes a two-sided projective plane, since a global normal together with ambient orientation would orient it. Thus $M$ is $P^2$-irreducible.

The source is compact, connected, orientable, incompressible and has one longitudinal boundary. It is two-sided, with $\chi=1-2g$; the compression-disc/$\pi_1$ interface is Hatcher Corollary 3.3, p. 59. A boundary longitude can first be isotoped to a $J$-leaf by the torus curve classification and a collar extension of its velocity field. For the compact family of boundary curves, choose longitude coordinates or constant speed with a fixed starting point: arbitrary reparametrizations are not themselves a compact family. Boundary reparametrizations extend along the source collar and the surface space is quotiented by reparametrization. The single ambient boundary torus corresponds to the single source boundary. No minimal-genus or extra boundary-incompressibility hypothesis is added.

### Black boxes actually accepted

**$(E^*)$:** the complete smooth proper relative-attainment statement, over the whole proper isotopy class with boundary in $J$, including Corollary 11's final clause. This is E(ii) already cited in competition Theorem 3.2, not merely a minimum within a space of stable minimal surfaces.

**$(U^*)$:** arbitrary chosen incompressible relative minima in classes with disjoint representatives are disjoint or coincide. Distinct connected vertex classes exclude coincidence. Its universal quantifier allows representatives to be fixed one class at a time before any pair is examined.

For the source-audit and conditional Appendix branch, two further statement interfaces are recorded. Hass–Scott Theorem 6.12 attains the fixed-boundary infimum in its own piecewise smooth class; compact smooth exterior extension supplies homogeneous regularity, and the collar satisfies all three sufficiently-convex conditions. This does not give the target's A.1 membership. Kapovich Proposition 9 / Corollary 10 supply compactness of area-bounded stable embedded minimal surfaces of fixed connected source type with nonempty boundary and the prescribed compact boundary family, and finitely many open-and-closed isotopy blocks. Stability here is fixed-boundary stability. Compactness gives neither nonemptiness nor only finitely many individual surfaces. The repaired body, after accepting complete E(ii), does not separately reprove attainment through these interfaces.

The environmental and source conditions just listed satisfy these statements. Their printed proofs are not independently certified: D09 concerns the FHS adaptation; D10 concerns the compactness input to Corollary 11; nonemptiness also returns to Hass–Scott's fixed-boundary output. See [the open items](open-items.md).

### Independent Hopf argument

Let $\Sigma$ be any smooth proper minimal surface supplied by $(E^*)$. Near a boundary point use its tangent-plane graph over the actual curved smooth planar half-neighbourhood. The projected boundary is smooth with nonzero tangent, so the domain has an interior tangent ball. Put $u=r|_\Sigma$. Properness gives $u>0$ in the interior and $u=0$ on its boundary. Minimality gives

$$
\Delta_\Sigma u=\operatorname{tr}_{T\Sigma}\operatorname{Hess}r\le0.
$$

The smooth induced operator is uniformly elliptic locally with bounded drift. Apply the boundary-point lemma to $-u$, or the equivalent minimum form for $u$. The outward derivative is negative, so $du\ne0$ at the boundary. Thus $dr|_{T\Sigma}\ne0$, and $\Sigma$ is transverse to $\partial M$: it is neat.

This argument uses neither Definition A.1 nor (27), Proposition A.5 nor Theorem A.6. It supplies the smooth graphs, transverse graph direction and boundary smoothness needed by the body's calls on pp. 18–19. The correct correction is **replace those calls**, because the original body really does call A.6/A.7; it is not accurate to say the body never depends on Appendix A.

### Smooth proper classes and fixed representatives

If a compact smooth proper track has nontransverse intermediate members, arrange it to be neat. In source-collar coordinates $(s,u)$, add $\epsilon(t)u\chi(u)$ to its ambient inward coordinate. At $u=0$ the original inward derivative is nonnegative. Choose $\epsilon(t)>0$ over potentially non-neat parameters and zero near the already-neat endpoints. A sufficiently small compact-track $C^1$ perturbation preserves embedding, properness, boundary curves and endpoints, and makes the inward derivative positive. Standard compact neat isotopy extension now gives smooth ambient isotopy preserving $\partial M$ setwise. This does not assert the same for arbitrary topological tracks.

Choose $S,A,B$ by $(E^*)$, then Hopf. Apply $(U^*)$ to $(S,A)$ and $(S,B)$: the **same fixed** $S$ misses both. If $A\cap B=\varnothing$, $u,w$ would be equal or adjacent, contrary to distance 2. Hence their intersection is nonempty. Their areas equal $A(w),A(u)$, and later minima $Z$ use exactly the same interface.

<a id="r02"></a>
## R02 — Conditional regularity within Appendix A

**Competition locators:** Definition A.1 and (27), p. 23; Lemmas A.2–A.4, pp. 23–25; Proposition A.5, pp. 25–26; Theorem A.6, p. 27; Lemma A.7, pp. 27–28.

Everything here assumes an attained minimizer with the A.1 piece structure. It does **not** close D12. The conditional assembly of A.6 additionally assumes a genuine smooth stable minimizing sequence and the declared compactness statement; it does **not** close D22.

### Stationarity and crossing an open edge

Compactly supported ambient flows preserve the competition class. First variation vanishes. Fields supported away from seams give minimality of each interior piece. Exhaust an open edge by inner collars, excluding vertices and the actual boundary; the flux limit gives opposite conormals. The pieces therefore share a tangent plane and form a $C^1$ graph across the edge. Integrating on the two sides cancels interface flux, giving the graph equation weakly across it.

Write its area integrand as $L(x,z,p)$, $a^i=L_{p_i}$, $b=-L_z$. The equation is $\partial_i a^i(x,u,Du)+b(x,u,Du)=0$. On a compact bounded graph range, $A^{ij}=a^i_{p_j}$ is symmetric uniformly positive. Difference-quotient energy tests with cutoff first give $u\in W^{2,2}_{\rm loc}$, absorbing all height, spatial and lower-order terms by Young's inequality. For $w_k=D_ku$, the full differentiated equation is

$$
\partial_i\bigl(A^{ij}D_jw_k+a^i_z w_k+a^i_{x_k}\bigr)
+b_{p_j}D_jw_k+b_z w_k+b_{x_k}=0.
$$

Its coefficients and bounded-source terms are controlled on the compact range. The two-dimensional bounded-source local Hölder estimate gives $w_k\in C^{0,\alpha}$; a sign on the zero-order coefficient is not needed for this local regularity estimate. Quasilinear Schauder and bootstrapping then give smoothness. Hölder continuity of the solution alone is not a substitute for this gradient step. The exact GT bounded-source version remains a book-check item.

### Boundary $C^1$ to smoothness

Suppose $u\in C^1(\overline H)$, smooth minimal in the interior, with smooth true boundary and smooth boundary height $\varphi$. Expand

$$
A^{ij}D_{ij}u=f_0,
\qquad f_0=-b-\sum_i a^i_{x_i}-\sum_i a^i_zD_iu.
$$

The principal matrix is continuous uniformly elliptic and $f_0$ continuous bounded; gradient Hölder continuity is not yet assumed. Choose a smooth capped domain matching the true boundary near the point; keep its artificial cap away. Let $w=\chi(u-\varphi)$, with cutoff vanishing near that cap. It has zero boundary values and

$$
Lw=\chi(f_0-L\varphi)+2A^{ij}(D_i\chi)D_j(u-\varphi)
 +(u-\varphi)L\chi=:H_0,
$$

continuous bounded. Flatten and scale a sufficiently small boundary chart. The operator is a constant positive matrix plus a small continuous perturbation; flattening drift scales as $O(\rho)$. The constant-coefficient smooth-domain Dirichlet inverse $L^4\to W^{2,4}\cap W^{1,4}_0$ is bounded. Choose the perturbation norm below half the inverse threshold; a Neumann series gives a strong solution $v$ of $Lv=H_0$.

In dimension two, $v\in C^{1,1/2}$. The original $w$ is continuous on the closure and locally $W^{2,4}$ inside. Nondivergence comparison/uniqueness with zero zero-order term, applied on inner domains and then by boundary continuity, gives $w=v$. This does not presuppose global $W^{2,4}$ regularity of $w$. The coefficients are now Hölder, so boundary Schauder and bootstrap give $C^\infty$. The small radius can depend on the given $C^1$ modulus; there is no uniform-gradient circularity. Exact Dirichlet and uniqueness references remain to be compared with GT.

### Bounded Hopf drift and genuine curved sectors

For a merely $C^1$ minimal graph $\Phi=(x^1,x^2,w)$, blindly expanding its induced Laplacian would introduce unknown second derivatives. Instead the minimal immersion equation gives, in the interior,

$$
\Delta_W\Phi^a=-h^{ij}\widetilde\Gamma^a_{bc}(\Phi)
 \partial_i\Phi^b\partial_j\Phi^c.
$$

For $a=1,2$, $\Phi^a=x^a$, so

$$
\Delta_W=h^{ij}\partial_{ij}+\beta^a\partial_a,
\quad \beta^a=-h^{ij}\widetilde\Gamma^a_{bc}(\Phi)
 \partial_i\Phi^b\partial_j\Phi^c.
$$

Only first derivatives and the smooth ambient connection occur; the drift extends boundedly to the boundary and the principal matrix is uniformly elliptic. Thus the Hopf use for $r\circ\Phi$ is legitimate once the interior-ball condition is supplied.

For a curved sector of opening greater than $\pi$, choose a strictly smaller straight sector still of opening greater than $\pi$; the $C^2$ bounding arcs differ from their tangent rays by $O(|x|^2)$. Small enough radii place that sector inside the true domain, where a tangent disc fits. At opening exactly $\pi$, combine the opposite-ray arcs as a $C^{1,1}$ graph $y=f(x)$, $|f(x)|\le Cx^2$. A disc centred at $(0,\rho)$ of radius $\rho$ has lower boundary

$$
y=\rho-\sqrt{\rho^2-x^2}\ge x^2/(2\rho).
$$

Choose $1/(2\rho)>C$ and keep the whole disc in the chart. It touches only at the origin and otherwise lies inside. The true domain need not be contained in its straight tangent cone.

### Interior vertex and removable point

After the open-edge repair, all finite sectors have a common tangent plane $T$. Shrink until their tangent planes remain within a fixed small angle of $T$, and projected edge tangents are nonzero. Projection is a local diffeomorphism off the vertex. Take a small closed topological-disc neighbourhood whose outer boundary projects away from zero. The finite $C^2$ projected edges have strictly increasing radial distance near the vertex; shrinking all finite sectors together makes the preimage of a sufficiently small closed base disc another connected disc assembled in their cyclic order.

Projection on the punctured truncation is now a **proper** local diffeomorphism onto the punctured base disc, hence a finite covering. Over each base point, distinct preimages have distinct real heights. Height ordering gives continuous global sections and forbids monodromy swapping their order. A degree greater than one would disconnect the punctured source; connectedness forces degree one. Values and gradients extend continuously at the vertex, giving a $C^1$ graph. A cutoff about the missing point has bounded-flux error $O(\delta)\to0$; the weak equation extends, and the interior gradient repair regularizes it. Properness and connectedness are established before the degree argument.

### Boundary vertex, angle and stability

Choose an oriented sweep of the common tangent plane. Adjacent conormals are opposite; all sector angles are positive; the two actual boundary rays are opposite. The total angle is a positive odd multiple of $\pi$. Choose the first cumulative angle at least $\pi$. If it is below $2\pi$, the finite rays keep their strict order at small radii and their glued sectors form one graph with two genuine curved outer arcs. If it reaches $2\pi$, the last sector alone has opening in $(\pi,2\pi)$. At opening $\pi$, use the preceding curved-disc argument.

Apply Hopf on this graph, using properness to keep its interior in $\operatorname{Int}M$, to obtain a nonzero $dr|_T$. **Only now** does $r(tv)=t,dr(v)+o(t)\ge0$ confine all tangent directions to a closed half-circle, forcing total angle $\pi$. The actual projected boundary has nonzero smooth tangent and the full graph is $C^1$, so the boundary repair applies. One must not assume total angle at most $\pi$ before Hopf.

Properness is inherited from the input, not proved from this regularity argument. For a smooth fixed-boundary area minimum, compactly supported interior variations give stability; density in $H^1_0$ extends the second-variation inequality. This is Dirichlet stability, not free-boundary stability. Given the missing sequence and compactness, the A.6 assembly by finite open-and-closed isotopy blocks and area continuity is sound. It still leaves [D12](open-items.md#d12) and [D22](open-items.md#d22) open. For any independently supplied smooth proper minimum, R01's Hopf argument gives neatness without this existence chain.

<a id="r03"></a>
## R03 — Exact rounding, common quantitative caps and the corrected D29

**Competition locators:** Lemma 5.4, pp. 14–15; Appendix B rounding proof, pp. 28–31, equations (31)–(35).

### Profile and whole-circle coordinates

Fix an odd smooth profile derivative $\zeta$, with $0\le\zeta\le1$ on $[0,1]$, $\zeta(0)=0$, and $\zeta=1$ near 1. Put

$$
c_0=1-\int_0^1\zeta(t)dt>0,
\quad \Theta(t)=c_0+\int_0^t\zeta(\tau)d\tau.
$$

On $[-1,1]$, $\Theta$ is even, positive, at most 1, and matches $|t|$ near the endpoints to all orders. For $t\ge0$, $\Theta(t)-t=\int_t^1(1-\zeta)\ge0$. The changed part lies in the closed wedge; it is incorrect to claim strict separation throughout the entire strip, since the profile agrees with the old graph near its edges.

Define

$$
g(m)=\int_{-1}^1\left(\sqrt{1+m^2}-\sqrt{1+m^2\Theta'(\tau)^2}\right)d\tau.
$$

It is positive for $m>0$, continuous and nondecreasing: the integrand is nonnegative, strictly positive near zero, and its derivative has the sign obtained from monotonicity of $u/\sqrt{1+m^2u}$ for $0\le u\le1$.

For the transverse angle $\alpha$, set $\theta=\min\{\alpha,\pi-\alpha\}$. The complementary wedge slopes are $m$ and $1/m$, both between $\tan(\theta/2)$ and $\cot(\theta/2)$. Use the **single common coefficient**

$$
\beta(\theta)=\tfrac14g(\tan(\theta/2)),
\quad Q(\theta)=\csc(\theta/2),\quad M_\theta=\cot(\theta/2).
$$

For $0<\theta\le\pi/2$, $\beta$ is positive, continuous, nondecreasing and at most one. Then $g(m)\ge4\beta$ in every sector. Different sectors need a common guaranteed lower bound, not equal actual gains.

Along each oriented intersection circle, a smooth periodic normal frame comes from its wedge bisector and the ambient orientation. Start with a normal exponential tube and use the two smooth sheet-defining functions fibrewise to straighten the sheets exactly. Their normal Jacobian is invertible; quantitative inverse-function estimates give whole-circle coordinates $\Xi(s,\xi_1,\xi_2)$, normalized so $\Xi^*g(s,0)=I$, in which the corner graph is $\xi_1=m(s)|\xi_2|$. This uses globally compatible defining functions rather than gluing unrelated local charts.

Choose a positive safety radius $R(s)$ so the full tube is injective and contains no input sheets except the designated collars, with room for isotopy support. Let $K(s)\ge1$ control $|m'|$ and $\|\Xi^*g(s,\xi)-I\|\le K(s)|\xi|$. These are **local** data. Uniformity on a later parameter family is supplied independently by R10, not inferred from this rounding lemma.

### Two-dimensional density estimate

For positive smooth width $\eta$, put $F=m\eta\Theta(\xi_2/\eta)$, $\tau=\xi_2/\eta$. Then

$$
F_{\xi_2}=m\Theta'(\tau),\quad
F_s=\eta m'\Theta+m\eta'(\Theta-\tau\Theta'),
\quad F_s^2\le2\eta^2K^2+8m^2(\eta')^2.
$$

The old graph's integrated Euclidean density is $2\eta\sqrt{1+m^2}+E_1$, $0\le E_1\le(m')^2\eta^3$. The new one is at most $\eta\int\sqrt{1+m^2\Theta'^2}+\eta\max F_s^2$. Discarding the nonnegative old error gives Euclidean gain at least $\eta[g(m)-2\eta^2K^2-8m^2(\eta')^2]$.

The relative error of a two-dimensional density is at most twice the ambient metric norm error when the latter is at most $1/8$, independently of slope. Under the caps below, each of the two integrated densities is at most $3\eta Q$, and the changed part has coordinate radius at most $Q\eta$. Thus their total metric loss is at most $12K\eta^2Q^2$. The actual slice gain is at least

$$
\eta\left[g(m)-2\eta^2K^2-8m^2(\eta')^2-12K\eta Q^2\right].
\tag{R3.1}
$$

This is an area-density estimate including $F_s$, not just a transverse-arc-length estimate.

### Common caps, regularity and actual support

The corner object is already smooth proper neat away from its interior crease. Rounding cannot create external neatness. Put $0<d\le\min\{1,\operatorname{dist}(s,\partial M)\}$. For all four used sectors, take a common minimum of $R,d$ and common maximum of $K$. Define

$$
E=\min\left\{\frac{R}{32Q},\frac{d}{64Q},\frac1{32KQ},
\sqrt{\frac{\beta}{8K^2}},\frac{\beta}{48KQ^2},1\right\},
\qquad H=\frac{\sqrt\beta}{8M_\theta}.
\tag{R3.2}
$$

Use $\eta\in C^\infty$, $0<\eta\le E$, $|\eta'|\le H$. The three losses in R3.1 are at most $\beta/4,\beta/8,\beta/4$, so

$$
\text{slice gain}\ge\tfrac{27}{8}\beta\eta\ge\beta\eta,
\qquad G(\gamma)=\int_\gamma\beta(\theta)\eta,ds>0.
\tag{R3.3}
$$

The changed portion has coordinate radius $\le Q\eta$, geometric distance $\le2Q\eta$; isotopy/certification support can be kept within $16Q\eta$. These constants have been included in the safety caps. Width $\eta$ is a coordinate half-width, **not** geometric radius $\eta$. For example, the core height is $mc_0\eta$, exceeding $\eta$ if $mc_0>1$. Also a merely $C^1$, non-$C^2$ width makes this core non-$C^2$; endpoint matching alone cannot give a smooth surface. Use smooth widths in the body proof.

For fixed compact transverse input, a small positive constant width suffices. If an existence formulation for arbitrary $C^1$ input widths is retained, first shrink within strict margins and approximate in $C^1$. The excess margin in R3.3 allows a sufficiently close smooth approximation to preserve the required gain relative to the original width, as well as support and derivative constraints.

An optional geometric-radius formulation is obtained with

$$
q_{\rm geom}=\sqrt{1+m^2}+\sqrt{1+m^{-2}},\quad Q\le q_{\rm geom}\le2Q,
\quad w=\eta/(32q_{\rm geom}).
$$

This smooth quantity is unchanged by $m\leftrightarrow1/m$. Require

$$
\eta\le\min\{32q_{\rm geom}E,,16q_{\rm geom}^2H/|q_{\rm geom}'|\},
\quad |\eta'|\le16q_{\rm geom}H,
$$

reading the zero-derivative denominator as infinity. Then $w\le E$, $|w'|\le H$, and support $16Qw\le\eta/2$. Shrink and smoothly approximate $w$ with $w/2\le\widetilde w\le w$ within strict caps. R3.3 still gives gain at least $\beta\eta/(64Q)$. This optional formulation changes the gain coefficient as well as the unit of width. The rest of this document uses the coordinate-width formulation R3.2 consistently.

### D29: two different isotopy statements

A smooth diffeomorphism has invertible derivative. It takes a genuine corner's two distinct tangent half-planes to two distinct half-planes, not one smooth tangent plane. Therefore D29 fails **under the smooth ambient-isotopy reading**. The paper also declares piecewise smooth isotopy for piecewise smooth objects in Definition A.1, p. 23; that convention means the argument does not refute every reasonable reading of the original rounding clause.

Use the following replacement:

1. A corner and its rounding are related by a locally flat/tame ambient isotopy. In each fibre, interpolate graph heights and extend the displacement by a strictly increasing vertical homeomorphism with cutoff, using the safety margin. This transports topology, Euler characteristic, balls and complementary regions; it is not claimed to be a smooth diffeotopy.
2. In the **same charts and same labelled resolution**, positive smooth widths $\eta_0,\eta_1$ are compared by $\eta_u=(1-u)\eta_0+u\eta_1$. Size and absolute-derivative constraints are convex. On the compact parameter interval the width stays positive, so the profile gives a smooth neat embedding family, fixed near the true boundary. Extend its velocity by a tubular field and cutoff to a smooth ambient isotopy. Zero width is never an endpoint.

The first clause supplies corner-region transport; the second supplies fixed smooth coarse classes. R05 separately certifies disc-swap competitors in their original smooth vertex class. Changing $t$ also needs R11's coherent positive-parameter track, not just this fixed-chart interpolation.

<a id="r04"></a>
## R04 — Positive push-off with leaf boundary and finite area cost

**Competition locators:** Lemma 5.5, p. 15, proof p. 31.

Fix a rounded smooth neat frontier $\widehat T\subset\overline U$. Let $\nu$ point into the chosen region $U$, and let $n$ be the ambient outer normal. Near the ambient boundary start with

$$
X_0=\nu-\psi(r)\langle\nu,n\rangle n.
$$

Neatness and compactness give $1-\langle\nu,n\rangle^2\ge c>0$ there; after shrinking the collar, $\langle X_0,\nu\rangle\ge c$. The field is tangent to $\partial M$.

Around the boundary leaf choose foliation-product coordinates $(s,v)$, leaves $v=\mathrm{constant}$. Such a local product is compatible with the closed embedded leaves: a nonidentity return map on a transverse interval would have iterates accumulating at a fixed leaf and prevent the corresponding leaf being an embedded closed circle. Take $Y=\pm\partial_v$ toward $U$, with a positive normal lower bound, extend slightly into the collar, and interpolate with $X_0$ by nonnegative partition weights. Positivity is retained. Extend and cut off the field away from $S$ and other designated obstacles.

At unchanged frontier contacts the field points strictly into $U$; the changed core is already inside. Compactness gives $\sigma_0>0$ so the flow satisfies $T(\sigma)\subset U$ for $0<\sigma\le\sigma_0$. At zero time the surface is only required to lie in $\overline U$. The flow preserves embedding, neatness and the endpoint leaf condition. The original PDF's closed-region overline is correct; it must not be turned into a claimed open-region inclusion at zero time.

After fixing this rounded surface and field, put $K_1=\sup\|\nabla X\|$. The two-dimensional Jacobian satisfies

$$
|\partial_\sigma\log J_\sigma|\le2K_1,
\quad |\operatorname{Area}(T(\sigma))-\operatorname{Area}(\widehat T)|
\le C\sigma,
\quad C=2K_1e^{2K_1\sigma_0}\operatorname{Area}(\widehat T)<\infty.
$$

The constant may depend on $t$ and the chosen width. The order is **rounding, then finite $C$, then $\sigma$**; no uniform cost bound as $t\to0$ is required.

<a id="r05"></a>
## R05 — Disc swaps certified in a slightly larger smooth three-ball

**Competition locators:** Lemma 5.6, pp. 15–17, equations (14), (16)–(17). **External locator:** Hatcher, Lemma 1.10 proof, p. 20, same-boundary discs in a three-ball.

Let the transverse inputs be $A$ and $B$, with disjoint leaf boundaries; $B$ is minimal, $A$ is in the class of a minimum $A_0$, and $e=\operatorname{Area}(A)-\operatorname{Area}(A_0)\ge0$. Their compact intersection is a finite union of interior circles. A disc patch must have an intersection circle as its boundary: a seam-free spanning disc would be the whole connected input and is excluded by the non-trivial-knot hypothesis.

A simple interior circle bounds at most one disc on a connected surface with boundary. If it bounds a disc on either input, $\pi_1$-injectivity implies that it is contractible on the other and also bounds a disc there. Let $\mathcal D$ be this finite nonempty disc-circle family when any disc patch exists. Write

$$
\mathcal A=\{\gamma\in\mathcal D:\operatorname{Int}D_A(\gamma)\cap B=\varnothing\},
\quad \mathcal B=\{\gamma\in\mathcal D:\operatorname{Int}D_B(\gamma)\cap A=\varnothing\}.
$$

Each family is nonempty by selecting an inclusion-minimal disc on its own side. The selected circles need not be the same or simultaneously innermost on both sides.

For $\gamma\in\mathcal A$, put $D=D_A(\gamma)$, $D'=D_B(\gamma)$. Their union is an embedded locally flat interior corner sphere. A qualitative rounding and irreducibility, followed by tame region transport, give a ball $Q_0$ with this exact corner boundary. The connected remainder $B_\gamma\setminus\gamma$ does not meet that sphere and connects to $\partial B\subset\partial M$; it lies outside $Q_0$. In particular $\operatorname{Int}Q_0\cap B=\varnothing$. Other pieces of $A$ inside the ball do not affect this one-sided operation.

The exact corner replacement $B_0=B_\gamma\cup D$ is embedded and has

$$
\operatorname{Area}(B_0)=\operatorname{Area}(B)-\operatorname{Area}(D')+\operatorname{Area}(D).
$$

**Do not describe $B_0$ as a smooth-isotopy image.** Directly round its original two sheets using R03's common four-sector width to obtain a smooth competitor $B''$. Do not introduce a thin smooth neck and then assume its curvature remains uniformly bounded.

To certify $B''\in[B]$, enlarge the ball to a smooth ball $R$ covering the entire rounding support. Near the seam, straighten the two sphere rays angularly and make the remainder ray normal to the resulting line; the straightening is smooth off the zero-radius crease and locally flat at it. An outer collar, pulled back, follows the remainder's annular collar. Choose its positive width near the seam to cover the full change tube; away from the seam shrink it to avoid the compact separated remainder. The safe tube excludes all other $B$ sheets. Thickening $Q_0$ in this collar gives a slightly larger region with smooth outer sphere, away from the angular singularity; any remote joins can be smoothed without touching the input. Irreducibility identifies this interior thickening as a smooth three-ball $R$.

Inside $R$, the old $B$ and new $B''$ are proper smooth discs $E_0,E_1$. They have the same boundary $\delta\subset\partial R$ and agree on its small collar; outside $R$ the surfaces agree. Hatcher's smooth-category disc-isotopy fact gives an isotopy relative to $\delta$. Freeze a smaller common collar and extend the remaining velocity field by a tubular cutoff vanishing near $\partial R$. Integrating and extending by identity outside $R$ gives a smooth ambient isotopy preserving $\partial M$ pointwise. This establishes the competitor's actual smooth vertex class.

The ball **must be slightly larger**: fixed-width rounding may enter a sector outside the original empty ball. In a normal slice where that ball occupies $x\ge0,y\ge0$ and the replacement turns from the negative horizontal ray to the positive vertical ray, a smoothing following that corner crosses $x<0,y>0$. A construction confined to the original quadrant would need a different routing and lose the fixed-width gain. This is a local certification obstruction, not a global theorem counterexample.

R03 now yields

$$
\operatorname{Area}(D_B(\gamma))+G(\gamma)\le\operatorname{Area}(D_A(\gamma))
\quad(\gamma\in\mathcal A).
$$

Reverse the one-sided construction for $\gamma\in\mathcal B$. Use the minimality of **$A_0$**, not of the perturbed $A$, to obtain

$$
\operatorname{Area}(D_A(\gamma))+G(\gamma)\le\operatorname{Area}(D_B(\gamma))+e.
$$

Choose $a\in\mathcal A$ minimizing its $A$-disc area and $b\in\mathcal B$ minimizing its $B$-disc area. If the other circle's disc is not a patch, its interior contains an inclusion-minimal patch disc. Therefore $\operatorname{Area}D_A(a)\le\operatorname{Area}D_A(b)$ and $\operatorname{Area}D_B(b)\le\operatorname{Area}D_B(a)$. For $\phi=\operatorname{Area}D_A-\operatorname{Area}D_B$,

$$
G(a)\le\phi(a)\le\phi(b)\le e-G(b),
\qquad G(a)+G(b)\le e.
\tag{R5.1}
$$

No frontier or no-disc-patch conclusion was used to construct the competitors or their widths. This is the common gain interface used in all configurations.

<a id="r06"></a>
## R06 — Frontiers, boundary count, Euler characteristic and compression

**Competition locators:** Lemmas 4.4–4.5 and Corollary 4.6, pp. 9–10; Lemma 4.9, pp. 11–12; §5 T0 bookkeeping, pp. 17–18.

Linking gives $\pi_1(M)\to\mathbb Z$. Each oriented single-longitude Seifert surface is primitive dual to this map; it is nonseparating because a meridian has intersection number one. Cutting along it gives a connected manifold; stacking copies indexed by integers gives the cyclic cover. A lifted surface is the interface between two stacks and separates the cover into two connected half-spaces.

Cut along $S$. Distinguish the closed fundamental domain $\overline C$, whose two walls are identified by projection, from $C^\circ=\overline C\setminus(S_0\cup S_1)$. Only the latter projects injectively to $M\setminus S$, and it may still contain the relevant ambient-boundary annulus. Lift $A,B$ there. Label their upper half-spaces by containing $S_1$, and lower ones by containing $S_0$. Define $U_\uparrow=H_A\cap H_B$, $U_\downarrow=L_A\cap L_B$.

At a transverse point the two frontiers use the opposite $(+,+)$ and $(-,-)$ sectors. Each of four sheet rays and every cut-open input patch appears exactly once. Coorientation in the stacking direction agrees with input orientations; a region's inward push-off direction need not be that coorientation. Round with R03 and push with R04, keeping the safety tubes and flows in $C^\circ$. The projected frontiers are embedded, miss $S,A,B$, and miss each other.

The boundary cover is an open annulus. The two disjoint longitudinal core circles have a linear order there: the lower frontier takes the lower one, the upper frontier the upper one. There are no seam endpoints at the ambient boundary. Thus each frontier has **exactly one** longitudinal boundary circle and exactly one component $P_\uparrow,P_\downarrow$ with boundary. Algebraic intersection number alone would not establish this count.

Before discarding closed components, closed-circle cut-and-reglue has zero Euler correction:

$$
\chi(T_\uparrow)+\chi(T_\downarrow)=\chi(A)+\chi(B).
$$

Once no disc patches have been proved, no discarded closed component is a sphere. Without a seam, a sphere would be an entire closed input component; with seams, an innermost seam on the sphere bounds a seam-free patch disc, contradicting no disc patches. Write $c=\sum_j\chi(C_j)\le0$ for all discarded components. Then

$$
g(P_\uparrow)+g(P_\downarrow)=g(A)+g(B)+c/2\le g(A)+g(B).
\tag{R6.1}
$$

An essential nonseparating compression reduces genus by one. A separating compression caps a closed side of genus $k\ge1$; retaining the original boundary side reduces genus by $k$. The single longitude boundary remains, each genuine compression strictly lowers integer genus, and a maximal finite sequence ends at an incompressible surface. Choose the actual sequences and their final classes before any later neighbour.

For total compression decrease $d\ge0$,

$$
g(w_\uparrow)+g(w_\downarrow)=g(u)+g(w)+c/2-d.
\tag{R6.2}
$$

If equality with the input sum holds, $c=d=0$. Every genuine compression has positive decrease, so both sequences have no steps and the coarse surfaces are already incompressible. Discarded tori may remain since their Euler characteristic is zero. No claim that compression is area-nonincreasing is used.

<a id="r07"></a>
## R07 — Two scales and transport of specified descendants

**Competition locators:** Lemma 4.9(2), pp. 11–12; Lemma 4.5 / Corollary 4.6, p. 10; T0 common-neighbour step p. 17; T2 common-neighbour step p. 36.

Fix smooth coarse classes using positive admissible rounding/push-off scales, and then fix their terminating compression sequences and final vertices. For a later compact $Z$ disjoint from the transverse input union, put $d_Z=\operatorname{dist}(Z,A\cup B)>0$. Keeping width fixed while $\sigma\to0$ only approaches the rounded surface: a small disc crossing its rounded core but separated from the input disproves that inference. It is an auxiliary local countermodel, not a realized common-neighbour counterexample.

Instead take $\eta_\lambda=\lambda\eta_0$, $\lambda>0$. All caps remain valid, support $16Q\lambda\eta_0$ tends uniformly to zero, and all positive-width endpoints have the same smooth class by R03. Choose $\lambda$ so the rounded surface lies within $d_Z/4$ of the input, **then** choose a positive push-off displacement below $d_Z/4$. Positive widths and push-off scales can be compared on compact interpolation tracks with a common small flow time and smoothly selected inward fields. The coarse class is unchanged; zero width is not a smooth endpoint.

For an incompressible $Q$ disjoint from the current connected boundary surface $P$, clean an **already specified** compressing disc $D$. Its transverse intersections with $Q$ are finite interior circles. Choose an innermost disc $E\subset Q$ with interior disjoint from $D$, and let $F\subset D$ have the same boundary. The interior corner sphere $E\cup F$ bounds a ball. Connected $P$, disjoint from its sphere and joined to the ambient boundary, lies outside. The often omitted second check is that $D\setminus\operatorname{Int}F$ is a connected annulus containing $\partial D$; its interior does not meet the sphere, and its boundary is attached to the outside $P$. It too lies outside the ball.

A ball slide replacing $F$ by a small parallel copy of $E$, smoothed in their shared collar, consequently hits neither $P$ nor the remainder of $D$. Use R05's slightly larger smooth ball and two smooth disc endpoints to realize the slide relative to $P$. A sufficiently small one-sided collar of $Q$ removes the selected circle and all circles inside $F$, without adding new ones. Finitely many slides clean $D$. They preserve the specified compression's output class. At each subsequent step first transport the next **originally specified** disc along the current ambient isotopy, then clean it. Induction preserves every intermediate and final class.

By $(E^*)$, choose a minimum $Z\in z$. By $(U^*)$, the same $Z$ misses $A$ and $B$; distinct classes exclude coincidence. For distance-2 inputs $z=u,w$ cannot meet both common-neighbour premises; the paper's separate handling by (a) is harmless. Apply the two-scale construction and clean the transported sequences against $Z$. For T1/T2 first choose a small $t_z>0$ making $A_{t_z}$ miss $Z$, then use the two scales; R11 keeps the classes fixed.

Thus the order is

$$
\forall(x,u,w)\ \exists(w_\uparrow,w_\downarrow)\ \forall z
\ \exists(t_z,\eta_z,\sigma_z,\text{same-class representatives and cleaned discs}).
$$

For (a), do the cleaning separately against $S,B,A_t$ (or $A$ in T0). Only pairwise adjacency is asserted: no single representative or disc system need avoid every neighbour at once, and later $Z$ need not miss $S$. The fine representatives for (b) need not retain the quantitative area gain used for (d); a previously obtained class-area competitor remains valid.

<a id="r08"></a>
## R08 — Complete graph-difference, reflection and tangency argument

**Competition locators:** Proposition 5.7, pp. 18–19, equations (21)–(24); analytic proof in Appendix B, pp. 31–33, including (36). **Sources:** GT standard statements (book unverified); Hildebrandt–von der Mosel author version Theorem 4.1, pp. 18/22; Vekua standard similarity principle (book unverified).

### Full height-and-gradient linearization

In an interior double graph write $B=\{y=\beta_0(x)\}$, $A=\{y=\widehat u(x)\}$, $f=\widehat u-\beta_0$. At a common boundary leaf, neatness gives a graph direction transverse to both tangent planes and a shared half-cylinder. Flatten $B$ by $y'=y-\beta_0(x)$ when perturbing the difference as a height; at the boundary $\beta_0=0$, preserving the leaf coordinate.

For the ambient graph-area integrand $\mathcal F(x,u,p)$, the equation is $\partial_i\mathcal F_{p_i}-\mathcal F_u=0$. Interpolate **both** $u_\tau=\beta_0+\tau f$ and $p_\tau=D\beta_0+\tau Df$. Subtracting yields

$$
0=\partial_i(a^{ij}f_j+d^if)-e^jf_j-k_0f,
$$

where $a^{ij}=\int_0^1\mathcal F_{p_ip_j}\,d\tau$, $d^i=\int\mathcal F_{p_iu}$, $e^j=\int\mathcal F_{up_j}$, $k_0=\int\mathcal F_{uu}$, all evaluated along that interpolation. Hence

$$
Lf=\operatorname{div}(a\nabla f)+b\cdot\nabla f+cf=0,
\quad b^j=d^j-e^j,\quad c=\partial_i d^i-k_0.
$$

The principal matrix is symmetric uniformly positive on the fixed compact graph range, and coefficients smooth on a smaller closed disc/half-disc. Different equivalent arrangements can give different lower-order coefficients; no height independence of the ambient metric is assumed. Interpolating only gradients is insufficient.

### Positive auxiliary solution and its separate derivative bound

On $D_R$ or $D_R^+$, for $q\in W^{1,2}_0$, use

$$
\mathcal B[q,\varphi]=\int aDq\cdot D\varphi-\int(b\cdot Dq)\varphi-\int cq\varphi.
$$

Poincaré gives $\|q\|_2\le C_PR\|Dq\|_2$, so

$$
\mathcal B[q,q]\ge(\lambda-C_PR\|b\|_\infty-C_P^2R^2\|c\|_\infty)\|Dq\|_2^2.
$$

Take $R$ small enough for coercivity at least $\lambda/2$. Lax–Milgram gives $Lq=-c$; $h=1+q$ solves $Lh=0$ with boundary trace one. After scaling $x=R\xi$, drift and zero-order terms become $Rb$ and $R^2c$. Energy gives $\|q_R\|_2+\|Dq_R\|_2\le CR^2$; the standard supremum estimate retaining its $L^2$ term gives $\|q_R\|_\infty\le CR^2$. Thus $h\ge1/2$. Do not substitute a maximum-principle estimate requiring a missing sign of $c$.

There is a standard barrier backup independent of the remembered exact GT 8.15 edition. Let $\psi=K(R^2-|x|^2)$. Then

$$
L\psi=-2K\operatorname{tr}a-2K(\partial_i a^{ij}+b^j)x_j+cK(R^2-|x|^2).
$$

First fix $K$ large, then shrink $R$ so $L\psi\le-\|c\|_\infty$. The functions $q-\psi,-q-\psi$ have nonpositive boundary traces, including the half-disc's flat edge, and nonnegative $L$-values. Positive-part tests with the same coercivity give $|q|\le\psi\le KR^2$.

**Bound $Dh$ separately.** Smooth coefficients and constant flat-edge data give local interior or flat-boundary regularity on a smaller neighbourhood away from artificial half-disc corners. Thus $h$ is smooth there and $Dh$ bounded. Positivity of a weak solution alone would not supply that bound.

### Remove the zero-order term before maximum principles or reflection

Set $v=f/h$, $A_0=ha$, $d_0=aDh+hb$. Expanding gives

$$
L(hv)=vLh+\operatorname{div}(ha\nabla v)+(aDh+hb)\cdot\nabla v.
$$

Normalize with $k=(\det A_0)^{-1/2}$:

$$
\operatorname{div}(kA_0\nabla v)+(kd_0-A_0\nabla k)\cdot\nabla v=0.
$$

The derivative $-A_0\nabla k$ belongs in the drift. The new symmetric principal matrix has determinant one and is elliptic; there is no new zero-order term. For the common-leaf case, $v$ has zero flat-edge trace.

Apply the checked boundary isothermal theorem on a smaller smooth Jordan domain with metric the inverse of the normalized matrix. A $C^{1,\alpha}$ closed-boundary conformal diffeomorphism is supplied. In the boundary case choose the Möbius pole away from the relevant boundary arc and restrict to a compact half-neighbourhood. Only there is the map $F$ and its inverse uniformly Lipschitz, with nonzero bounded Jacobian.

In the weak change of variables,

$$
\widehat a=DF\,a\,DF^T/|\det DF|,
\quad \widehat b=DF\,b/|\det DF|.
$$

This is a density law; no derivative of $DF$ is taken. Conformality makes $\widehat a$ scalar, and determinant one makes it $I$. The local drift is bounded. Thus $\Delta\widehat v+\widehat b\cdot D\widehat v=0$.

### Odd reflection, Sobolev entry and similarity factorization

In boundary coordinates $(x,r)$, reflect $V(x,-r)=-\widehat v(x,r)$; reflect the tangential drift evenly and the normal drift oddly. For a full-disc test function $\varphi$, combine the two half-disc integrals using $\varphi(x,r)-\varphi(x,-r)$, which has zero flat-edge trace. Density of zero-trace tests establishes the weak reflected equation without assuming a classical flux. The reflected drift is generally only $L^\infty$. First eliminating mixed principal terms was essential.

On the local closed half-patch $\widehat v$ is $C^1$; the odd reflection has bounded gradient, with tangential derivative zero at the edge. Hence $\Delta V=-\widetilde b\cdot DV\in L^p$ for every finite $p$. Local Laplace regularity gives $V\in W^{2,p}$, $w=2\partial_zV\in W^{1,p}$, $p>2$. Starting from $W^{1,2}$, one can instead bootstrap through $W^{2,2}$ and the two-dimensional embedding. This entry is required before invoking similarity.

For real $V$, $w=V_x-iV_r$ satisfies

$$
\partial_{\bar z}w=-\tfrac14(\widetilde b_1+i\widetilde b_2)w
-\tfrac14(\widetilde b_1-i\widetilde b_2)\overline w=Aw+B\overline w.
$$

The target PDF includes the complex conjugate; a missing OCR/text overline is not an error in this formula. A standard local proof of similarity is as follows: let $Q=A+B\overline w/w$ where $w\ne0$, and zero where $w=0$. It is bounded and $\partial_{\bar z}w=Qw$. A cutoff Cauchy transform on a larger disc gives $\partial_{\bar z}\omega=Q$ locally, $\omega\in W^{1,p}\subset C^{0,\alpha}$. Then $\Phi=e^{-\omega}w$ is weakly holomorphic and hence holomorphic. Thus $w=e^\omega\Phi$; the exponential has positive upper and lower modulus bounds on compact subdiscs. A nonzero factor has finite-order isolated zeros. This does not claim an original-page Vekua check.

### Recover the difference gradient, propagate coincidence, obtain finite tangencies

At a tangency, $f=df=0$, so $v=dv=0$. A nonzero factor of order $m\ge1$ gives $|dv|\asymp\rho^m$, $|v|\le C\rho^{m+1}$. With $h\ge1/2$, bounded $Dh$, and local bi-Lipschitz coordinates,

$$
|df|=|h,dv+v,dh|\ge c_1\rho^m-c_2\rho^{m+1}>0
$$

on a sufficiently small punctured disc/half-disc. This is isolation **among critical/tangency points**, not isolation as a point of the intersection set. A Scherk graph difference $\log(\cos y/\cos x)$ has a unique critical point at zero but two zero arcs $y=\pm x$ through it, illustrating the wording correction without providing a global Seifert counterexample.

If $w\equiv0$, $v$ is constant and its tangency value or zero boundary trace forces local coincidence. Coincidence germs are open in $\operatorname{Int}A$. At an interior limit point, closedness of $B$ and tangent-plane continuity give common graphs; the holomorphic factor vanishes on an open subset, so its uniqueness propagates coincidence across the graph. The germ set is also closed. Connectedness and proper closures give $A=B$, contradicting distinct vertices. Local coincidence is not propagated merely by continuity.

If an interior tangency did not change sign, $v$ would attain a zero extremum; the strong maximum principle for the **zero-order-free** equation makes it identically zero, again impossible. Thus interior differences change sign arbitrarily near every tangency.

At the boundary, critical points are closed and locally isolated and hence finite. Noncritical boundary points have noncritical neighbourhoods. A finite boundary cover therefore contains an entire open collar in which $df\ne0$, although $|df|$ need not have a positive minimum right up to the boundary. Interior tangencies are confined to a compact region away from that collar; their set is closed and discrete, hence finite. T1's intersection already has positive boundary distance.

<a id="r09"></a>
## R09 — Actual perturbations, noncollapsing circles and good-region length

**Competition locators:** Lemmas B.1–B.3, pp. 33–35; Corollary B.4(1), pp. 34–35; T1 perturbation and Lemma B.5, pp. 37–38.

For T2 first shrink the no-critical collar so all interior tangency discs are outside its closure. On the common boundary let $a(s)=\partial_r f(s,0)$. Its zeros are finite, so choose a fixed sign $\varsigma$, positive-length closed arc $I$, and $a_0>0$ with $\varsigma a\ge a_0$. Put $\Lambda=\sup|\partial_r^2f|$, and choose

$$
r_1\le\min\{r_0/4,\ a_0/(2\max\{1,\Lambda\})\}.
$$

Then $\varsigma f\ge a_0r/2$ on $I\times(0,r_1]$. The maximum corrects the original undefined denominator when $\Lambda=0$; all these choices precede $t$.

Fix smooth $0\le\chi\le1$, one on $r\le r_0/2$, supported in $r<r_0$; its derivative is supported on a compact transition band. In separate interior tangency charts flatten $B$, and fix disjoint cutoffs $\psi_p$, one on smaller cores. Define $A_t$ by the differences $F_t=f+\varsigma t\chi$ in the collar, and $f_p-\varsigma t\psi_p$ in each interior chart; keep the other parts unchanged. These are local graph definitions, not one global graph function.

On the transition band $c_\chi=\min|df|>0$; choose $t\|d\chi\|_\infty<c_\chi/2$. Where $d\chi=0$, $dF_t=df\ne0$ throughout the open collar. On the interior cores the unique critical value moves off zero; on their fixed transition annuli the gradient lower bound dominates the cutoff error. Every sufficiently small positive $t$ is transverse to $B$, neat, in the class $w$, disjoint from $S$, and has a new boundary leaf. The graph track from zero is neat and extends ambiently. It converges smoothly to $A$, so $e(t)\ge0$ by class minimality and $e(t)\to0$. $A_t$ is not assumed minimal.

If circles $\gamma_n\subset A_{t_n}\cap B$ collapsed in diameter as $t_n\to0$, their limit lies in $A\cap B$. There are three cases:

1. At an interior transverse point, quantitative graph convergence gives a unique through-arc in a fixed smaller double-graph ball, which cannot contain a whole circle.
2. At an interior tangency, the circle eventually lies in a convex constant-cutoff core. Its projected Jordan disc lies in that core. A constant level on its boundary forces an interior extremum or constancy. The sole critical point of the original difference changes sign, and subtracting a constant does not make it an extremum; constancy would produce a whole disc of critical points. Both are impossible.
3. At a boundary/collar point, its projected Jordan disc stays in $r>0$: the linear coordinate $r$ cannot have a smaller interior minimum than on its boundary. The actual $F_t$ has no critical point anywhere on that disc, contradicting constant zero boundary values. No uniform positive gradient bound as $r\downarrow0$ is needed.

This gives $\rho_0>0$ and a small-parameter threshold with every circle's diameter at least $\rho_0$. The transverse intersection is finite, nonempty (distance 2 excludes disjoint representatives), and consists of interior circles.

Let the $N$ interior tangency balls of radius $2\rho_2$ be disjoint, with $4N\rho_2<\rho_0/8$ and the additional collar safety bounds. Put $P=\bigcup B_{2\rho_2}(p)$, $G=M\setminus P$, $G'=M\setminus\bigcup B_{\rho_2}(p)$. Collapse each ball to a point. A near-shortest quotient path may delete repeated visits to a collapsed point; lifting it adds at most $4\rho_2$ per ball. Hence $d(a,b)\le d'(a,b)+4N\rho_2$, while a circle's projected length is at most $\operatorname{length}(\gamma\cap G)$. Points with distance at least $\rho_0/2$ give

$$
\operatorname{length}(\gamma\cap G)>3\rho_0/8.
$$

The original circle may enter a ball many times; no uniform visit count is assumed. When $N=0$, omit that restriction and choose a positive scale under the remaining safety bounds. This is only Corollary B.4(1), independent of angle or tube estimates.

For T2, $\varsigma F_t=\varsigma f+t\chi>0$ over $I\times(0,r_1]$, so this strip is swept free of intersections. A collar-contained circle is noncontractible in the annulus, since otherwise its Jordan disc contradicts the no-critical $F_t$. Put $H_{\rm gain}=G\cap\{r\ge r_1\}$, extending $r$ continuously as $r_0$ outside the collar. With $C'_{\rm met}\ge1$ bounding collar coordinate Lipschitz constants:

- If $\min_\gamma r\ge r_1$, use the quotient length bound.
- If $\min r<r_1$ and $\max r>r_0/2$, two distinct arcs cross the band $[r_1,r_0/2]$, giving total length at least $r_0/(2C'_{\rm met})$ there.
- Otherwise the circle is essential in the collar annulus and its projection covers the boundary circle. Points projecting into $I$ lie above $r_1$; the Lipschitz image-length bound gives length at least $\ell(I)/C'_{\rm met}$ in the gain set.

Thus every circle has gain-set length at least

$$
c_*=\min\{3\rho_0/8,r_0/2,\ell(I)\}/C'_{\rm met}>0.
$$

Take the intersection of all parameter thresholds, including that of B.4(1). The length proof does not call B.4(2)/(3), so there is no length/angle/width cycle. In particular the whole collar is not a constant level $f=-\varsigma t$; the cutoff must remain in $F_t$.

For T1, $d_0=\operatorname{dist}(A\cap B,\partial M)>0$. Use only interior flattened charts, heights $f_p-t\psi_p$, with neighbourhoods at boundary distance greater than $d_0/2$. Boundary remains fixed; the same class/transversality/convergence conclusions hold. The first two collapse cases give $\rho_0$; the quotient gives length $>3\rho_0/8$ outside tangency balls. No boundary sign arc or collar projection argument is needed.

<a id="r10"></a>
## R10 — Buffered full tubes, exact smooth platform and unified gain

**Competition locators:** Corollary B.4(2)/(3), pp. 35–36; T2 gain and equation (44), pp. 36–37; Lemma B.5 / T1 gain, pp. 38–39.

### Uniformity only on a thick good region

In T2 let $V_t=\Gamma_t\cap G'\cap\{r\ge r_1/2\}$ and

$$
K=A\cap B\cap\left(M\setminus\bigcup B_{\rho_2/2}(p)\right)\cap\{r\ge r_1/4\}.
$$

It is compact, away from boundary and tangencies, and everywhere transverse. A fixed buffered neighbourhood contains all $V_t$ for sufficiently small $t$, by convergence and compactness. An angle lower bound $2\theta_1$ there transfers to $\theta\ge\theta_1$.

Cover $K$ by finitely many doubled single-sheet graph balls, explicitly excluding all remote sheet parts by compact embeddedness. The fixed smooth scheme converges in sufficiently high $C^k$ norms (for instance $C^4$); uniform inverse bounds on the normal Jacobian give a unique graph arc for the **entire** intersection in each protected ball. Use a slightly larger protected set $V_t^+$ with the same buffer. Its graph and angle bounds control intersection curvature, $m$, $1/m$, $m'$, straightening charts and metric derivatives. Curvature alone would not give global reach.

In a single graph the chord controls arc separation and its normal-coordinate map is injective on a uniform small scale. A finite-cover Lebesgue radius and the doubled-ball margins ensure every protected basepoint and all sufficiently close possible colliding basepoints lie in one such ball. This checks other branches, not only pairs already in the good set.

For each fixed $t$, compact embedded $\Gamma_t$ has a possibly small whole-curve safe normal radius $r_t>0$, also excluding other input sheets. Take $r_t<R/2$, with $R$ a uniform protected radius. A smooth cutoff $\xi_t$, one near $V_t$, supported in $V_t^+$, defines radius $r_t+(R-r_t)\xi_t$. Two unexpanded fibres are safe by $r_t$. If one is expanded, every potential colliding basepoint is within $2R$, in the same protected doubled ball whose **whole intersection** is one arc; local injectivity excludes collision, even from a branch outside the target good set. That graph also excludes foreign sheets.

Shrink the straightening image by a fixed ratio to fit inside this normal tube. Include chart-distance comparisons, separation from $S$/the two walls, true ambient-boundary distance and every sector's sheet safety in R03's $R,d,K$. On the protected region there are common $R_g>0$, $K_g<\infty$, $d_g>0$, independent of $t,z$. Outside it the tube radius and data may degenerate.

A concrete warning against the original full-circle supremum inference comes from the Scherk graph $y=f(u,v)=\log(\cos v/\cos u)$, $B=\{y=0\}$, $A_t=\{y=f-t\}$. Along $v=a\sqrt t$, near $a=1$,

$$
m=\frac{\sqrt2}{\sqrt{a^2+1}\sqrt t}+O(\sqrt t),
\quad \frac{dm}{ds}=-\frac{a\sqrt{a^2+2}}{t(a^2+1)^2}+O(1).
$$

At $a=1$ this is $-\sqrt3/(4t)+O(1)$, although the surfaces converge smoothly and their curvatures stay bounded. This local model does not assert a global Seifert counterexample. It shows why a bad-region full-circle $\sup|m'|$ cannot supply uniform good-region width.

### Unified caps and exact platform

Use **R03's** coefficient and density constants throughout; do not retain a larger old $g_0$ after substituting its more conservative rounding interface. Let $\beta_1=\beta(\theta_1)$, $Q_1=\csc(\theta_1/2)$, $M_1=\cot(\theta_1/2)$, and fix

$$
E_g=\min\left\{\frac{R_g}{32Q_1},\frac{d_g}{64Q_1},\frac1{32K_gQ_1},
\sqrt{\frac{\beta_1}{8K_g^2}},\frac{\beta_1}{48K_gQ_1^2},1\right\}>0,
\quad H_g=\frac{\sqrt{\beta_1}}{8M_1}>0.
$$

Monotonicity of $\beta$ and the decreasing $Q,M_\theta$ show $E\ge E_g$, $H\ge H_g$ on the protected set. These are coordinate-width caps after straightening, not unconverted geometric tube radii.

Fix $q\in C^\infty(M,[0,1])$, one on $H_{\rm gain}$, supported in $G'\cap\{r>r_1/2\}$. Multiply smooth tangency-ball cutoffs (zero on radius $5\rho_2/4$, one outside $2\rho_2$) by a collar cutoff (zero below $5r_1/8$, one above $r_1$). They have fixed buffer; the collar cutoff is already constant near its outer edge. Put $L_q=\|dq\|_\infty$, and **before selecting $t$** set

$$
\eta_1=\min\{E_g/2, H_g/(2\max\{1,L_q\})\}>0.
$$

After any sufficiently small fixed $t$, take its full-curve positive caps $E_t,H_t$, choose

$$
0<\eta_2(t)\le\tfrac12\min\{\eta_1,\min_{\Gamma_t}E_t\},
\quad \eta_t=\eta_2(t)+(\eta_1-\eta_2(t))q|_{\Gamma_t}.
\tag{R10.1}
$$

At $q=0$, nonnegative smooth $q$ has $dq=0$, so width is a small positive constant and derivative zero, satisfying even tiny bad-region caps. At $q>0$, the protected bounds give $\eta_t\le E_g/2\le E_t$ and $|\eta_t'|\le\eta_1L_q\le H_g/2\le H_t$. At $q=1$ it is **exactly** $\eta_1$. Thus the width is positive smooth on the whole curve, with no convolution loss or undocumented smoothing of pointwise constraints.

The slice gains are nonnegative everywhere. Restricting their integral to the good length gives the common fixed lower bound

$$
G_t(\gamma)\ge\varepsilon_*:=\beta_1\eta_1c_*>0
\quad\text{for every circle and every sufficiently small }t.
$$

A disc patch would imply $2\varepsilon_*\le G_t(a)+G_t(b)\le e(t)$ by R05, using the **same** widths and gain coefficient. Only after fixing $\varepsilon_*$ reduce the threshold so $e(t)<\varepsilon_*$; all small parameters have no disc patches. Reduce it further to $e(t)<\varepsilon_*/2$ for the final area budget. Changing the gain coefficient requires recomputing $E_g,H_g,\eta_1,\varepsilon_*$, not simply renaming the old constant.

For T1 omit collar restrictions in $K,V_t,H_{\rm gain}$ and use boundary safety at least a conservative $d_0/4$. Use only ball cutoffs, $q=1$ on $G$, supported in $G'$. The same caps and checks give $\varepsilon_*=\beta_1\eta_1(3\rho_0/8)$.

### All quantitative dependencies in one order

$$
\begin{aligned}
(S,A,B)&\to\text{fixed scheme, including }r_1,\chi,\psi_p
\to\rho_0\to\rho_2\to c_*\\
&\to\text{buffered local geometry }(\theta_1,R_g,K_g,d_g)
\to q,E_g,H_g\to\eta_1\to\varepsilon_*\\
&\to\delta\to t\to\eta_2(t)\to\text{rounded surfaces}\to C(t)\to\sigma.
\end{aligned}
$$

All uniform constants may depend on the fixed representatives, metric, foliation and scheme, but not the later $z$ or selected $t$. Bad-region floors and post-rounding costs may depend on $t$. The diameter is derived from the scheme containing $r_1$, irrespective of the original displayed order. Widths and disc-swap gains are constructed before invoking no disc patches. $\eta_2(t)$ need not be differentiable in $t$; R11 uses another track for smooth class comparison.

<a id="r11"></a>
## R11 — Positive-parameter smooth coarse classes before the later neighbour

**Competition locators:** T2 positive-parameter comparison and common-neighbour step, p. 36; T1 reuse, p. 39.

Take any positive compact parameter interval $J=[t_a,t_b]\subset(0,\delta]$. Transversality, boundary separation and distance from $S$ have positive minima. For the embedding velocity $V_t$, let $n_B$ be the unit normal of $B$ and $p_t=\operatorname{proj}_{TA_t}n_B$. Correct it along the intersection by the tangential velocity

$$
\tau_t=-\frac{\langle V_t,n_B\rangle}{|p_t|^2}p_t.
$$

Then $V_t+\tau_t$ is tangent to $B$ but has the original normal velocity of $A_t$. In transverse coordinates $A_t=\{a=0\}$, $B=\{b=0\}$, its $b$-component on $A_t$ vanishes along $b=0$; factor out $b$ and extend that factor so the ambient component vanishes on all of $B$. Partition of unity preserves this linear tangency condition. At the separated boundaries use neat charts to keep the field tangent to $\partial M$; keep support away from $S$. The flow moves $A_{t_a}$ to $A_t$, preserves $B$ setwise and $S$ pointwise, and preserves $\partial M$ setwise.

Lift from the identity to the cyclic cover. The flow fixes both $S$ walls and commutes with deck translation. The upper side is continuously labelled by $S_1$, so the two labelled corner frontiers are transported separately. This alone does not say the flow sends one independently optimized smooth rounding to another.

To compare the **smooth** classes, use coherent positive-parameter normal frames and straightening charts on the intersection track. Signed sums/differences of the oriented sheet normals give nonvanishing labelled bisectors and a periodic frame. Compactness of $J$ gives a common positive tube radius and common positive admissibility bounds. Choose one small constant width $\bar\eta>0$; its arclength derivative is zero. The fixed profile in these coherent charts produces a compact smooth surface track agreeing with the old sheets near strip edges. Projection of the track to $J$, including its boundary track, is a submersion. Integrate a horizontal field with time component one and tangent to the boundary track to obtain a smooth neat embedding family; extend ambiently.

At each endpoint interpolate its quantitative width with $\bar\eta$ **in that endpoint's same charts**. Convex caps and strictly positive width make these smooth endpoint comparisons valid. Choose a common small push-off time and smooth inward fields along the compact track, then compare each endpoint's original push-off by a positive-time flow. All endpoints are smooth. Neither $t=0$ nor zero width is inserted, and no smooth dependence of the optimized $\eta_2(t)$ is assumed.

Consequently $[P_\uparrow(t)]$, $[P_\downarrow(t)]$ are separately constant on $(0,\delta]$. Choose one $t_*$, fix these coarse classes and both terminating compression sequences, hence the final vertices. Only afterwards choose $z,Z$, then $t_z$, widths and push-off scales as in R07. This closes the output-before-neighbour interface.

<a id="r12"></a>
## R12 — Assemble T0, T2 and T1, with area only in the genus-equality branch

**Competition locators:** T0 proof pp. 17–18; configuration split p. 18; T2 completion pp. 36–37; T1 completion pp. 38–39; Theorem 5.1 p. 13.

### T0: disjoint boundary leaves and transverse interiors

The nonempty compact intersection has positive angle lower bound $\theta_0$ and total length $\ell_0>0$. R03 permits a common constant width $\eta_0>0$. Each circle has positive $G$. Here $e=0$; R05 would force the sum of two positive gains to be zero if any disc patch existed. Hence no disc patches, before applying frontiers or discarding spheres.

Construct the coarse surfaces by R06, fix compressions and final vertices. Equation R6.2 gives (c). R07's separate specified-descendant cleaning against $S,A,B$ gives (a); its two-scale construction for later $Z$ gives (b).

For (d), enter **only if final genus equality holds**. R6.2 forces both compression sequences empty; the coarse classes are the output classes. Before discarding any closed component, the two corner frontiers partition $A\cup B$ off measure-zero seams, so their total area is $A(w)+A(u)$. Set $\varepsilon_0=\beta(\theta_0)\eta_0\ell_0>0$. Both frontiers use all seams, giving total rounding saving at least $2\varepsilon_0$. After rounding obtain the finite total push-off constant $C$, then choose a positive safe $\sigma$ with $C\sigma<\varepsilon_0$. Discarding closed components only reduces area. Thus

$$
\operatorname{Area}(P_\uparrow)+\operatorname{Area}(P_\downarrow)
<A(w)+A(u)-\varepsilon_0.
$$

These smooth neat leaf-boundary surfaces represent the output classes. Taking their class infima gives (d), without an area claim for compression.

### T2: a common boundary leaf, possibly with interior tangencies

R08–R10 give a fixed smooth perturbation scheme, uniform good-region gain $\varepsilon_*>0$ and no disc patches for all sufficiently small positive $t$. R11 fixes labelled coarse classes and specified descendants before $z$. R06 gives (c); R07 applied separately to $S,B,A_t$ gives (a). The same fixed descendants with later $t_z$, two scales and disc transport give (b).

If final genus equality holds, again no genuine compression occurred. The whole unrounded frontiers partition $A_t\cup B$, and rounding saves at least the conservative common amount $\varepsilon_*$ in total. Take $t$ with $e(t)<\varepsilon_*/2$; choose its floor width, round, obtain finite $C(t)$, then choose $C(t)\sigma<\varepsilon_*/4$. After discarding closed components,

$$
\begin{aligned}
\operatorname{Area}(P_\uparrow)+\operatorname{Area}(P_\downarrow)
&\le\operatorname{Area}(A_t)+\operatorname{Area}(B)-\varepsilon_*+C(t)\sigma\\
&<A(w)+A(u)-\varepsilon_*/4.
\end{aligned}
$$

R11 identifies these with the already fixed output classes. Taking infima proves (d). Fine representatives for (b) need not retain this saving, because the class-area bound already has its competitor.

### T1: disjoint boundary leaves with interior tangencies

Each reused interface is checked separately. Properness and compactness give $d_0>0$ from the intersection to $\partial M$. Flattened interior constant-core perturbations keep the boundary fixed and preserve the vertex class, neatness and disjointness from $S$; $e(t)\ge0$ tends to zero. The two interior noncollapse cases and quotient argument give length $3\rho_0/8$ outside tangency balls. The protected compact set omits collar restrictions; its angle/tube bounds include boundary safety $d_0/4$. Ball-only cutoff platforms give a newly computed $\varepsilon_*$ using the same R03 caps. Disc swaps with $e(t)\to0$ exclude patches before the frontier construction.

R06 and separate cleaning yield (c),(a). Positive compact-parameter tracks, with separated fixed boundaries, satisfy all R11 conditions; fixed descendants and later two-scale representatives give (b). In the genus-equality/no-compression branch, precisely the T2 budget $e(t)<\varepsilon_*/2$, then $C(t)\sigma<\varepsilon_*/4$, gives (d). No boundary sign arc is used in T1, and no assertion of uniform bad-region slope derivative is carried over.

### Exhaustion and conclusion

Boundary leaves are either equal or disjoint. For disjoint leaves, the interiors are transverse (T0) or have tangencies (T1); equal leaves give T2. T2 need not mean tangency along the whole boundary. These three cases exhaust the situation. Each case fixes both outputs before any later common neighbour and proves all four clauses. Thus the repaired body yields Theorem 5.1(a)–(d) under the declared complete external statements and standard analytic inputs. It does not close the independent proof-source or Appendix A existence debts.

<a id="r13"></a>
## R13 — Correction index and reference precision

This table identifies the original text to change. Page numbers are competition printed pages. Mathematical replacements are in R01–R12; original failures/unresolved verdicts remain in the step table.

| Original location / nodes | Correction |
|---|---|
| §5 opening p. 13; Proposition 5.7 input pp. 18–19; D22–D24 | Replace A.6/A.7 supply by complete E(ii) + independent Hopf (R01). Do not say Appendix A was never called. |
| Definition A.1 p. 23; Lemma 5.4(3)/(5) pp. 14–15, proof p. 29; D29 | State tame corner-region transport separately from positive-width smooth isotopy (R03). Negative verdict applies only to smooth corner endpoints. |
| Lemma 5.4 pp. 14–15, proof pp. 29–31; D25–D28 | Use positive smooth width, true $16Q\eta$ safety support and common four-sector caps; keep changed part in the closed wedge; include both area-density integrals. |
| Lemma 5.4 inputs p. 14; D28 | Require the corner object already smooth proper neat away from the interior crease; preserve its existing boundary collar. |
| Lemma 5.5 pp. 15/31; D30–D31 | Zero time in the closed region; positive time in the open region; leaf-projectable boundary field with a positive normal bound; finite cost only after rounding. |
| Lemma 5.6 pp. 16–17; D34–D36 | Exact corner patch for area bookkeeping; direct original-sheet rounding; slightly larger smooth ball for class certification. Reverse comparison pays $e$, not false minimality of $A_t$. |
| Lemma 4.9 proof p. 12; D37–D40 | Use the wall-deleted strip for injective projection; count boundary core circles by annular order. “Lemma 5.5(3)” refers to its unnumbered isotopy property, not an existing numbered third clause. |
| Lemma 4.9(2) pp. 11–12; T0 p. 17; T2 p. 36; D43/D51/D81 | Shrink rounding before push-off; in T1/T2 allow later $t_z$; transport specified descendants and preserve the original $\exists$ outputs before $\forall z$. |
| Lemma 4.5 p. 10; D45 | Add the remaining disc annulus outside the ball; clean the preselected sequence, not a newly chosen descendant. |
| Lemma A.3 p. 24; Proposition A.5 p. 26; D14/D15/D20 | Supply gradient regularity, including height/spatial/lower-order terms; use the boundary Dirichlet inverse/comparison route. Ordinary solution Hölder continuity is insufficient. |
| Lemma A.4 pp. 24–25; Proposition A.5 p. 26; Lemma A.7 pp. 27–28 | Use the minimal immersion equation for bounded drift and an interior ball in the actual curved domain; total boundary angle is concluded after Hopf. |
| Proposition A.5 pp. 25–26; D18 | Establish proper connected punctured projection truncation before height-order covering degree. |
| Proposition 5.7 pp. 18–19; D56 | Linearize height and gradient together, flatten $B$ before altering the graph difference as a height. |
| Analytic proof pp. 31–32; D59/D60 | Separate positivity from $Dh$; avoid artificial half-disc corners; include determinant-normalization drift derivative. |
| Analytic proof pp. 32–33; D61–D65 | Restrict conformal bi-Lipschitz claims to local compact patches; weak zero-trace reflection; prove Sobolev entry before similarity. The conjugate already exists in the PDF. |
| Proposition 5.7 p. 19 / proof p. 32; D66 | Replace “isolated in the intersection” by “isolated among tangency points” or “no other critical point in a punctured neighbourhood.” |
| Lemma B.1 p. 33; D71 | Replace the zero-denominator expression by $a_0/(2\max\{1,\Lambda\})$. |
| Lemmas B.2/B.3 pp. 34–35; D72/D73/D75 | Keep actual $F_t=f+\varsigma t\chi$; no positive gradient lower bound is claimed all the way to the boundary. |
| Corollary B.4(3) pp. 35–36; D77 | Use buffered whole-intersection tubes, excluding foreign branches and sheets, and only local good-region data; no uniform full-circle $m'$. |
| Equation (44) p. 37; D78 | Replace unspecified smoothing by fixed $q$ and exact affine width platform; recompute common caps and $\varepsilon_*$. |
| Positive-parameter comparison p. 36; D80 | Add coherent charts and common positive constant-width smooth tracks before comparing endpoint optimized roundings. |
| T2 conclusion p. 37 / T1 conclusion p. 39; D82/D86 | Make genus equality and empty compression sequences explicit before the class-area comparison. |
| Configuration split p. 18; parameter display p. 37; D55 | State three exhaustive configurations, including already-treated T0; put $r_1$ inside the scheme before deriving $\rho_0$. |
| §3 p. 7 / §4 p. 8, target [10]; D02/D03 | Add Kakimizu **p. 228** for irreducibility and **p. 225** for surface/vertex conventions; both targeted checks are complete. |

For other reference precision, use Hass–Scott Theorem 6.12 pp. 112–113, sufficiently-convex definition p. 110 and homogeneous regularity p. 109; Schultens **preprint** Theorems 2/4 p. 4, Proposition 9 / Corollary 10 p. 19, Corollary 11 / Theorem 12 p. 20; Hildebrandt–von der Mosel **author version** Theorem 4.1 p. 18 and boundary proof p. 22; FHS Theorem 6.2 p. 630 and §7 pp. 634–637; Anderson Theorem 3.1 pp. 101–102 **with its truncated objects retained**. None of these page additions closes D09/D10/D12/D22. Textbook candidate pages remain unverified as specified in the [bibliography](../sources/bibliography.md).
