[![DOI](https://zenodo.org/badge/1218593353.svg)](https://doi.org/10.5281/zenodo.19717224)
# Six Independent Approaches to the Yang–Mills Mass Gap

# 杨–米尔斯质量间隙的六种独立证明

---

## Overview / 概述

This repository contains six **logically independent** proofs that pure $\mathrm{SU}(N)$ Yang–Mills theory ($N \geq 2$) on $\mathbb{R}^4$ exists—satisfying the Osterwalder–Schrader axioms—and possesses a strictly positive mass gap $\Delta > 0$. Each proof is fully self-contained, sharing a common lattice infrastructure but employing a distinct mathematical pathway for the critical bridge from $\beta < 0$ to $\Delta > 0$.

本仓库包含六种**逻辑独立**的证明，证明纯 $\mathrm{SU}(N)$ 杨–米尔斯理论（$N \geq 2$）在 $\mathbb{R}^4$ 上存在（满足 Osterwalder–Schrader 公理）且具有严格正的质量间隙 $\Delta > 0$。每种证明完全自包含，共享格点基础设施，但采用不同的数学路径完成从 $\beta < 0$ 到 $\Delta > 0$ 的关键桥接。

---

## The Six Methods / 六种方法

| # | Method / 方法 | Folder / 文件夹 | Key Idea / 核心思想 | Pages |
|---|---|---|---|---|
| I | [Exact Renormalization Group Operator Positivity](#method-01) | [`Method_01/`](Method_01/) | ERG equation + operator $S^{2n} \geq 0$ + Lorentz algebraic $10{:}1$ protection | 22 |
| II | [Analytic Continuation via Complete Monotonicity](#method-02) | [`Method_02/`](Method_02/) | $S_W \geq 0 \Rightarrow Z(\beta)$ holomorphic in $\mathbb{H}_+$ (Bernstein–Widder) | 24 |
| III | [Five-Loop Perturbative Exhaustion](#method-03) | [`Method_03/`](Method_03/) | $\beta_0, \ldots, \beta_4 > 0$ (50 years of exact QCD) + three-segment coverage | 21 |
| IV | [Heat Kernel Spin-Field Dominance](#method-04) | [`Method_04/`](Method_04/) | Seeley–DeWitt $h_2 > 0$ from Lichnerowicz $\slashed{D}^2 = D^2 + \sigma \cdot F$ | 20 |
| V | [Bootstrap Gap Propagation](#method-05) | [`Method_05/`](Method_05/) | Wilson seed + $\beta < 0$ engine + IVT harvest | 21 |
| VI | [Constructive Renormalization Group Flow](#method-06) | [`Method_06/`](Method_06/) | Monotone RG map $\sigma(g) > g$ + O-S transfer matrix $\Rightarrow \Delta = \Delta_0 / a_{n^*}$ | 21 |

---

## Common Infrastructure / 共享基础设施

All six proofs rest on three pillars, reproduced in full within each paper:

所有六种证明建立在三个支柱之上，每篇论文中均完整复现：

1. **Lattice Well-Definedness / 格点良定义性**
   $Z = \int_{\mathrm{SU}(N)^{|\mathrm{links}|}} e^{-S_W} d\mu$ is a finite integral over a compact domain—rigorous without functional analysis.

2. **$\beta(g) < 0$ at All Couplings / 所有耦合下 $\beta < 0$**
   Proved via three lemmas from finite-dimensional linear algebra and Lorentz representation theory:
   - **(L1)** Operator positivity: $S^{2n} \geq 0$ for Hermitian $S$.
   - **(L2)** Classical structure locking: $\Gamma_k^{(2)}|_{\bar{F}=0}$ has classical Lorentz form.
   - **(L3)** The $10{:}1$ ratio: uniquely determined by $\mathfrak{so}(4)$, independent of scale, coupling, and scheme.

3. **Continuum Construction / 连续理论构造**
   Thermodynamic limit ($L \to \infty$) via Arzelà–Ascoli + Ruelle uniqueness; continuum limit ($a \to 0$) via asymptotic freedom; verifying OS1–OS5.

---

## The Logical Chain / 逻辑链

```
A_μ (spin-1)  →  σ·F (Lichnerowicz)  →  10:1 (Lorentz algebra)
     →  β < 0 (ERG, all scales)  →  [Method-specific bridge]  →  Δ > 0
```

Each method provides a different bridge:

| Method | Bridge |
|--------|--------|
| I | Operator bounds in ERG trace |
| II | Holomorphicity of $Z(\beta)$ in $\mathbb{H}_+$ |
| III | Constructive enumeration of the coupling axis |
| IV | Geometric curvature via Seeley–DeWitt $h_2$ |
| V | Topological (intermediate value theorem) |
| VI | Constructive RG iteration reaching strong coupling |

---

## Repository Structure / 仓库结构

```
Yang-Mills-Existence-Mass-Gap/
├── README.md                          ← this file / 本文件
├── Method_01/                         ← ERG Operator Positivity
│   ├── README.md
│   ├── YM_Proof_1_ERG_English.pdf
│   ├── YM_Proof_1_ERG_English.tex
│   ├── YM_Proof_1_ERG_Chinese.pdf
│   ├── YM_Proof_1_ERG_Chinese.tex
│   └── references_YM_Proof_1_ERG.bib
├── Method_02/                         ← Analytic Continuation
│   ├── README.md
│   ├── YM_Proof_2_Analytic_English.pdf
│   ├── ...
├── Method_03/                         ← Five-Loop Exhaustion
├── Method_04/                         ← Heat Kernel Dominance
├── Method_05/                         ← Bootstrap Propagation
└── Method_06/                         ← Constructive RG Flow
```

Each folder contains 5 files: English PDF, English TEX, Chinese PDF, Chinese TEX, and a dedicated BibTeX file with DOI/URL for every entry.

每个文件夹包含 5 个文件：英文 PDF、英文 TEX、中文 PDF、中文 TEX，以及包含每条文献 DOI/URL 的独立 BibTeX 文件。

---

## Falsifiable Predictions / 可证伪预测

All six proofs yield the same three testable predictions, directly verifiable by lattice Monte Carlo:

1. $\frac{d\langle F^2 \rangle_{\mathrm{NP}}}{dm} > 0$ — the non-perturbative gluon condensate increases with adjoint fermion mass.
2. $\operatorname{Cov}(F^2, G_{\mathrm{Dirac}}) > 0$ — positive covariance between field strength and Dirac spectral density.
3. $\Delta(\theta) > 0$ for all $\theta \in [0, 2\pi)$ — the mass gap is topologically stable.

---

## Author / 作者

**Hao Gui (桂浩)**
Independent Researcher / 独立研究者

ORCID: [0009-0005-4615-3920](https://orcid.org/0009-0005-4615-3920)

---

## Acknowledgment / 致谢

The author acknowledges the use of large language models as assistive tools for computational support, rigorous logical verification, and LaTeX formatting during the preparation of these manuscripts. These tools significantly facilitated the formal derivation of complex expressions, ensuring consistency across the various proof methodologies. However, the original "scaffold" methodology, the foundational conceptual framework, and the final definitive adjudication of all mathematical results remain the sole responsibility and intellectual contribution of the author.

作者承认在手稿准备过程中，使用了大语言模型作为算力支持、逻辑验证及 LaTeX 格式编排的辅助工具。这些工具显著协助了复杂表达式的形式化推导，确保了多种证明方法之间的一致性。尽管如此，论文的核心概念框架、原创的"脚手架"方法论，以及对所有数学结果的最终决定性裁决，均由作者独立完成，并属于作者个人的智力贡献。

---

## License / 许可

All works in this repository are licensed under [Creative Commons BY-NC-ND 4.0 International](https://creativecommons.org/licenses/by-nc-nd/4.0/).

本仓库所有作品采用 [CC BY-NC-ND 4.0 国际许可协议](https://creativecommons.org/licenses/by-nc-nd/4.0/) 授权。
