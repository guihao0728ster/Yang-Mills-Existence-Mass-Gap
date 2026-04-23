# Method II: Analytic Continuation via Complete Monotonicity

# 方法二：基于完全单调性的解析延拓

---

## Independent Research Path / 独立研究路径

This proof elevates the elementary inequality $s_P \geq 0$ (non-negativity of the Wilson plaquette action density) into a powerful complex-analytic tool via the **Bernstein–Widder theorem**.

The logical chain:

1. $s_P \geq 0$ implies $S_W = \beta \sum_P s_P \geq 0$.
2. Therefore $Z(\beta) = \int e^{-\beta S_0} d\mu$ is the **Laplace transform** of a positive measure.
3. By the Bernstein–Widder theorem, $Z$ is **completely monotone**: $(-1)^n Z^{(n)} \geq 0$.
4. As a Laplace transform, $Z(\beta)$ is **holomorphic** in the entire right half-plane $\mathbb{H}_+ = \{\operatorname{Re}\beta > 0\}$.
5. Holomorphicity implies **real analyticity** of the free energy $f(\beta) = -(1/V)\ln Z$, which is *strictly stronger* than concavity—it excludes all non-analytic behavior, not just first-order transitions.

Combined with $\beta < 0$ at all couplings, holomorphicity provides the strongest possible regularity for the coupling-constant dependence, making gap propagation a consequence of complex analysis (identity theorem, Morera's theorem) rather than operator theory.

## Unique Contribution / 独特贡献

- **No Lee–Yang zeros** on the positive real axis: $Z(\beta) > 0$ for all real $\beta > 0$.
- **Real analyticity** of $f(\beta)$: convergent Taylor series at every point.
- **Analytic bridge**: gap propagation via the identity theorem for holomorphic functions.

## Files / 文件

| File | Description |
|------|-------------|
| `YM_Proof_2_Analytic_English.pdf` | English manuscript (24 pages, 56 equations) |
| `YM_Proof_2_Analytic_English.tex` | LaTeX source |
| `YM_Proof_2_Analytic_Chinese.pdf` | 中文版（22页，56个公式） |
| `YM_Proof_2_Analytic_Chinese.tex` | LaTeX 源文件 |
| `references_YM_Proof_2_Analytic.bib` | Bibliography (16 entries, all with DOI/URL) |
