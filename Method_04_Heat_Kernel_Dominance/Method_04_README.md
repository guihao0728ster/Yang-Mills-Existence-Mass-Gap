# Method IV: Heat Kernel Spin-Field Dominance

# 方法四：热核旋–场主导性

---

## Independent Research Path / 独立研究路径

This proof derives asymptotic freedom from **Riemannian geometry**: the sign of $\beta$ is determined by the **Seeley–DeWitt coefficient** $h_2$, which encodes the curvature of the gauge bundle through the index-theoretic structure of the heat kernel.

The starting point is the **Lichnerowicz–Weitzenböck formula**:

$$\slashed{D}^2 = D^2 + \sigma \cdot F$$

which decomposes the squared Dirac-type operator into an orbital part ($D^2$) and a spin-field part ($\sigma \cdot F$). The heat trace $K(t) = \operatorname{Tr}[e^{-t\slashed{D}^2}]$ has the short-time asymptotic expansion (Seeley–DeWitt):

$$K(t) \sim (4\pi t)^{-2} \sum_{n=0}^{\infty} h_n \, t^n$$

The second coefficient on flat space:

$$h_2 = \int d^4x \, \operatorname{Tr}[(\sigma \cdot F)^2] > 0$$

is **positive** because $(\sigma \cdot F)^2$ is the square of a Hermitian operator. This positivity directly yields paramagnetic dominance and $\beta_0 = (11/3)C_A > 0$.

## Unique Contribution / 独特贡献

- **Geometric derivation** of asymptotic freedom: $\beta$ is determined by bundle curvature.
- **Covariance inequality**: $\operatorname{Cov}(F^2, G_{\mathrm{Dirac}}) > 0$, connecting the gluon condensate to the Dirac spectral density—a new falsifiable prediction.
- **Spin-field unification**: $\sigma \cdot F$ is the single primitive from which all of asymptotic freedom derives.

## Files / 文件

| File | Description |
|------|-------------|
| `YM_Proof_4_HeatKernel_English.pdf` | English manuscript (20 pages, 52 equations) |
| `YM_Proof_4_HeatKernel_English.tex` | LaTeX source |
| `YM_Proof_4_HeatKernel_Chinese.pdf` | 中文版（18页，52个公式） |
| `YM_Proof_4_HeatKernel_Chinese.tex` | LaTeX 源文件 |
| `references_YM_Proof_4_HeatKernel.bib` | Bibliography (14 entries, all with DOI/URL) |
