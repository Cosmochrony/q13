# Q13 -- Gauge--Gravity Spectral Synthesis

**Gauge--Gravity Spectral Synthesis: A Conditional Einstein--Yang--Mills System
from Projective Spectral Entropy**

J. Beau, Independent Researcher, France

## Abstract

The companion papers (Gravity, Q12) established that the projective spectral entropy
functional $S_\Pi[g, \mathcal{A}] = \tfrac{1}{2}\log\det' A_{g,\mathcal{A}}$ produces the
Einstein tensor as the horizontal $a_2$ response and the local Yang--Mills equations as the
vertical $a_4$ response of the same functional.

The present paper joins the two variations within a single renormalized local action. Its
robust content is a **conditional** Einstein--Yang--Mills system: varying the matched action
with respect to the connection at fixed metric gives $D_\mu F^{a\mu\nu} = 0$, while varying
the same $\mathrm{tr}_\rho(F^2)$ term with respect to the metric gives exactly the Yang--Mills
stress tensor, through

$$\frac{1}{\sqrt{g}}\frac{\delta}{\delta g^{\mu\nu}}\int \sqrt{g}\,\mathrm{tr}_\rho(F^2)\,d^4x = 2\tau_{\mu\nu},
\qquad
\tau_{\mu\nu} = \mathrm{tr}_\rho\!\left(F_{\mu\rho}F_\nu{}^\rho - \tfrac14 g_{\mu\nu}F^2\right).$$

Once the Wilson coefficients are matched canonically, $c_{\mathrm{EH}} = 1/(16\pi G_N)$ and
$c_F = 1/(4g_{\mathrm{YM}}^2)$, the standard equation
$G_{\mu\nu} + \Lambda_{\mathrm{eff}} g_{\mu\nu} = 8\pi G_N T^{\mathrm{YM}}_{\mu\nu}$ is recovered
**by definition** of $T^{\mathrm{YM}}$.

**Central message**: one matched local action supplies both field equations; the spectral
expansion fixes the *degree of ultraviolet divergence* of each sector, not the finite couplings.

## Key Results

**Theorem (Conditional Einstein--Yang--Mills system)**: joint stationarity of the matched local
action yields

1. $G_{\mu\nu} + \Lambda_{\mathrm{eff}} g_{\mu\nu} = 8\pi G_N T^{\mathrm{YM}}_{\mu\nu}$,
2. $D_\mu F^{a\mu\nu} = 0$ (fixed-metric connection variation),

with $8\pi G_N = 1/(2c_{\mathrm{EH}})$ — **not** $c_{\mathrm{YM}}/c_{\mathrm{EH}}$.

**Structural (qualitative only)**: the two sectors carry different ultraviolet divergence
degrees, quadratic at $a_2$ and logarithmic at $a_4$.

**Matching data, not predictions**: $G_N$, $g_{\mathrm{YM}}$ and $\Lambda_{\mathrm{ren}}$ are
independent renormalized inputs. The cosmological $a_0$ term does contribute to the metric
equation and is retained.

## Changes in this version (1.3)

Major corrective revision. Withdrawn or corrected:

- **Metric variation** was wrong by a factor $-2$: the correct result is $2\tau_{\mu\nu}$, not
  $-4\,\mathrm{Tr}(F_{\mu\rho}F_\nu{}^\rho) + g_{\mu\nu}\mathrm{Tr}(F^2)$.
- **$8\pi G_N = c_{\mathrm{YM}}/c_{\mathrm{EH}}$ withdrawn**: the physical $T^{\mathrm{YM}}$
  already contains $g_{\mathrm{YM}}^{-2}$; $G_N$ and $g_{\mathrm{YM}}$ are independent matching data.
- **$a_0$**: the claim that it does not vary was false; it is retained as $\Lambda_{\mathrm{ren}}$.
- **$a_6$ section replaced by a cautious inventory**: in four dimensions $a_6$ is *not*
  logarithmically divergent; the pure-gauge invariant is $\mathrm{tr}_\rho(F^3)$, not $\Omega^4$
  (which belongs to $a_8$); several independent $RF^2$-type and derivative invariants occur, so no
  unique cross-term is claimed; the previously displayed $[R^{\mu\nu\rho\sigma},F_{\rho\sigma}]$
  is identically zero, the Riemann tensor being a gauge scalar.
- **Eddington--Born--Infeld theorem withdrawn**: the determinant construction was dimensionally
  and algebraically invalid (false Pfaffian identification, wrong semidefinite sign of $F_{\mu\rho}F^\rho{}_\nu$,
  $\ell^2 M$ where dimensions require $\ell^4 M$, inhomogeneous $R + \kappa F^2$, unproven upper bound).
- **Quantitative hierarchy withdrawn**: contradicted Gravity 3.3.1 and Q12 1.3.
- **Obsolete full horizontal--vertical operator split removed**, aligning with Q12 1.3.
- Production: fixed the table overflow and the empty PDF metadata; removed the stale
  `version` field from `zenodo.json`.

## Status

Preprint. DOI: [10.5281/zenodo.20209859](https://doi.org/10.5281/zenodo.20209859)

## Position in the Programme

- **Depends on**: Gravity paper ($S_\Pi[g]$ functional, $a_2$ Einstein sector),
  Q12 (Yang--Mills from $a_4$, admissible principal bundle),
  Q6a (gauge group $G_\Pi$), Q11 (effective Lorentzian metric)
- **SU(3) status**: $[H\text{-color}]_{\mathrm{pointwise}}$ established in O31/O32; it enters here
  only through the representation $\rho$ in which $\mathrm{tr}_\rho$ and $I_\rho$ are taken
- **Open**: non-linear completion (to be rebuilt from scratch, if at all), quantitative $a_6$
  coefficients, whether admissibility constrains any combination of the matching data,
  Lorentzian continuation of the gauge sector

## Compilation

```bash
cd q13
bash compile.sh
# or manually:
pdflatex -output-directory=out tex/q13.tex
```
