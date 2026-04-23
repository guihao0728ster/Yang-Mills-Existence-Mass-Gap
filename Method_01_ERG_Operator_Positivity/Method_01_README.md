# Method I: Exact Renormalization Group Operator Positivity

# 方法一：精确重整化群算子正定性

---

## Independent Research Path / 独立研究路径

This proof derives the mass gap through the **Wetterich exact renormalization group (ERG) equation**, leveraging the fact that on a finite lattice, the ERG equation is an *exact mathematical identity*—not a truncation or approximation—involving finite matrices and finite traces.

The core argument rests on three lemmas from finite-dimensional linear algebra and Lorentz representation theory:

1. **Operator Positivity** (L1): For Hermitian $S = A^{-1/2} B A^{-1/2}$, the even power $S^{2n} \geq 0$, guaranteeing non-negative paramagnetic contributions at every energy scale.
2. **Classical Structure Locking** (L2): Gauge invariance forces $\Gamma_k^{(2)}|_{\bar{F}=0}$ to retain its classical Lorentz form, regardless of quantum corrections.
3. **Lorentz Algebraic Protection** (L3): The paramagnetic-to-orbital ratio $10{:}1$ is uniquely fixed by the $\mathfrak{so}(4)$ algebra and is immune to dynamical corrections.

These three lemmas combine to yield $\beta(g) < 0$ for all $g > 0$—converting the perturbative *calculation* $\beta_0 > 0$ into a non-perturbative *structural theorem*.

## Key Equations

- ERG: $\partial_t \Gamma_k = \frac{1}{2} \operatorname{STr}[(\Gamma_k^{(2)} + R_k)^{-1} \partial_t R_k]$
- Result: $\partial_t(1/g_{\mathrm{phys}}^2) = -\frac{11}{6} C_A Z_k^2 I(k) < 0$

## Files / 文件

| File | Description |
|------|-------------|
| `YM_Proof_1_ERG_English.pdf` | English manuscript (22 pages, 45 equations) |
| `YM_Proof_1_ERG_English.tex` | LaTeX source |
| `YM_Proof_1_ERG_Chinese.pdf` | 中文版（20页，45个公式） |
| `YM_Proof_1_ERG_Chinese.tex` | LaTeX 源文件 |
| `references_YM_Proof_1_ERG.bib` | Bibliography (18 entries, all with DOI/URL) |
