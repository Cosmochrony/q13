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

Since $\mathrm{tr}_\rho(F^2) = I_\rho F^a_{\mu\nu}F^{a\,\mu\nu}$, canonical matching fixes the
products $c_{\mathrm{EH}} = 1/(16\pi G_N)$ and $c_F I_\rho = 1/(4g_{\mathrm{YM}}^2)$, where
$I_\rho$ is the Dynkin index of the fibre representation. The equation
$G_{\mu\nu} + \Lambda_{\mathrm{eff}} g_{\mu\nu} = 8\pi G_N T^{\mathrm{YM}}_{\mu\nu}$ then holds
**by definition** of $T^{\mathrm{YM}}$, with $8\pi G_N = 1/(2c_{\mathrm{EH}})$ depending on the
Einstein coefficient alone. The derivation is Euclidean; identification with the Lorentzian
Einstein--Yang--Mills equations requires a continuation not performed here.

**Central message**: one matched local action supplies both field equations; within a proper-time
cutoff the spectral expansion fixes the *degree of ultraviolet divergence* of each sector, not the
finite couplings.

## Key Results

**Theorem (Conditional Einstein--Yang--Mills system)**: joint stationarity of the matched local
action yields

1. $G_{\mu\nu} + \Lambda_{\mathrm{eff}} g_{\mu\nu} = 8\pi G_N T^{\mathrm{YM}}_{\mu\nu}$,
2. $D_\mu F^{a\mu\nu} = 0$ (fixed-metric connection variation),

with $8\pi G_N = 1/(2c_{\mathrm{EH}})$, depending on the Einstein coefficient alone.

**Structural (qualitative only, within a proper-time cutoff)**: the two sectors carry different
ultraviolet divergence degrees, quadratic at $a_2$ and logarithmic at $a_4$. This is a
scheme-dependent statement: the zeta-regularized determinant carries no power divergences.

**Matching data, not predictions**: $G_N$, $g_{\mathrm{YM}}$, $\Lambda_{\mathrm{ren}}$ (the $a_0$
term does contribute to the metric equation) and the dimension-six coefficients are independent
renormalized inputs.

**$a_6$**: inventory only — a representative spanning list, modulo integrations by parts and
Bianchi identities, not a basis. In four dimensions $a_6$ produces no ultraviolet divergence; the
pure-gauge invariant at this order is $\mathrm{tr}_\rho(F^3)$; several $RF^2$-type and derivative
structures occur and are interrelated by those identities, so no unique cross-term is singled out.

## Status

Preprint. DOI: [10.5281/zenodo.20209859](https://doi.org/10.5281/zenodo.20209859)

## Position in the Programme

- **Depends on**: Gravity paper ($S_\Pi[g]$ functional, $a_2$ Einstein sector),
  Q12 (Yang--Mills from $a_4$, admissible principal bundle),
  Q6a (gauge-structure sub-programme), Q11 (effective Lorentzian metric)
- **Gauge group**: $G_\Pi$ is a supplied compact group, not identified by the gauge-structure
  sub-programme. O31 is a withdrawal notice: it withdraws the co-admissibility of the individual
  capacity profiles — the content of $[H\text{-color}]_{\mathrm{pointwise}}$ — and every derivation
  of a gauge factor, the composite $\mathrm{SU}(3)\times\mathrm{SU}(2)\times\mathrm{U}(1)$
  included. No result here depends on which group is supplied: $G_\Pi$ enters only through the
  representation $\rho$ in which $\mathrm{tr}_\rho$ and the Dynkin index $I_\rho$ are taken
- **Open**: non-linear completion (to be rebuilt from scratch, if at all), quantitative $a_6$
  coefficients, whether admissibility constrains any combination of the matching data,
  Lorentzian continuation, in the geometric sector (not established by Q5b or Q6b) and in the gauge sector

## Compilation

```bash
cd q13
bash compile.sh
# or manually:
pdflatex -output-directory=out tex/q13.tex
```
