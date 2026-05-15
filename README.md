# Q13 -- Gauge--Gravity Spectral Synthesis

**Gauge--Gravity Spectral Synthesis: Joint Equations of Motion and Hierarchy
from Projective Spectral Entropy**

J. Beau, Independent Researcher, France

## Abstract

The companion papers (Gravity, Q12) established that the projective spectral entropy
functional $S_\Pi[g, \mathcal{A}] = \tfrac{1}{2}\log\det' A_{g,\mathcal{A}}$ produces the
Einstein equations as the horizontal $a_2$ response and the Yang--Mills equations as the
vertical $a_4$ response of the same functional.

The present paper carries out the gauge--gravity synthesis: we solve the joint variational
problem $\delta_{g,\mathcal{A}} S_\Pi = 0$, derive the coupled Einstein--Yang--Mills
equations of motion, compute the gauge--gravity coupling term at order $a_6$, and obtain
the hierarchy ratio
\[
  G_N g_{\mathrm{YM}}^2 \sim \frac{\ell_{\mathrm{sp}}^2}{12\,\dim V}
  \log(\Lambda/\mu)
\]
as a quantitative structural prediction. We then complete the gauge sector with the
admissible Born--Infeld extension, which bounds gauge field strengths by the structural
constant $c_\chi$ in direct analogy with the Born--Infeld completion of the gravitational
sector.

**Central message**: $S_\Pi[g,\mathcal{A}]$ unifies gravity and gauge dynamics in a single
spectral functional whose Seeley--DeWitt expansion determines both the equations of motion
and the gauge--gravity hierarchy from the geometry of the admissible projection alone.

## Key Results

**Theorem (Joint Einstein--Yang--Mills equations)**: The joint variational principle
$\delta_{g,\mathcal{A}} S_\Pi = 0$ yields:

1. Einstein equations with gauge source: $G_{\mu\nu} = 8\pi G_N T^{\mathrm{YM}}_{\mu\nu} + \mathcal{O}(a_6)$
2. Yang--Mills equations on the curved base: $D_\mu F^{a\mu\nu} = \mathcal{O}(a_6)$
3. Gauge--gravity mixing at order $a_6$ is suppressed by $R\ell_{\mathrm{sp}}^2 \ll 1$

**Theorem (Gauge--gravity hierarchy)**:
\[
  G_N g_{\mathrm{YM}}^2
  \sim \frac{\ell_{\mathrm{sp}}^2}{12\,\dim V} \cdot \log\!\left(\frac{\Lambda}{\mu}\right) \ll 1
\]
as a structural consequence of the Seeley--DeWitt expansion.

## Status

Preprint. DOI: [10.5281/zenodo.20209859](https://doi.org/10.5281/zenodo.20209859)

## Position in the Programme

- **Depends on**: Gravity paper ($S_\Pi[g]$ functional, $a_2$ Einstein result),
  Q12 (Yang--Mills from $a_4$, admissible principal bundle),
  Q6a (gauge group $G_\Pi$), Q11 (effective Lorentzian metric),
  born-infeld-paper ($c_\chi$ structural bound)
- **Inherited conditionality**: SU(3) sector conditional on [H-color]
  (confirmed numerically in O32 for $q \in \{61, 151, 211\}$; analytical proof open)

## Compilation

```bash
cd q13
bash compile.sh
# or manually:
pdflatex -output-directory=out tex/q13.tex
```
