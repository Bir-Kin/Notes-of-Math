# GTM82讲稿

- 奇异链复形的Mayer-Vietoris序列 
  $$
  0\leftarrow S^{\mathfrak{U}}_{q}(X)\xleftarrow{\varepsilon}\bigoplus\limits_{\alpha_0}S_q(U_{\alpha_0})\xleftarrow{\delta}\bigoplus\limits_{\alpha_0<\alpha_1}S_q(U_{\alpha_0\alpha_1})\xleftarrow{\delta}\cdots,\quad\forall q.
  $$
  where the $\text{\v{C}ech boundary operator}$ 
  $$
  \begin{align}
  \delta:\bigoplus_{\alpha_0<\cdots<\alpha_p}S(U_{\alpha_0\cdots\alpha_p})&\rightarrow\bigoplus_{\alpha_0<\cdots<\alpha_{p-1}}S(U_{\alpha_0\cdots\alpha_{p-1}}) \\
  (\delta c)_{\alpha_0\cdots\alpha_{p-1}}&:=\sum_{\alpha}c_{\alpha\alpha_0\cdots\alpha_{p-1}}
  \end{align}
  $$

- 奇异上链复形的Mayer-Vietoris序列 

  （由前者可以直接推出，因为 $\mathrm{Hom}(\cdot,\mathbb{Z})$ 保持自由 $\mathbb{Z}$-模正合列的正合性）
  $$
  0\rightarrow S_{\mathfrak{U}}^{q}(X)\xrightarrow{\varepsilon^*}\prod\limits_{\alpha_0}S^q(U_{\alpha_0})\xrightarrow{\delta^*}\prod\limits_{\alpha_0<\alpha_1}S^q(U_{\alpha_0\alpha_1})\xrightarrow{\delta^*}\cdots,\quad\forall q.
  $$
  where $\varepsilon^*$ is the restriction map and $\delta^*$ is the alternating difference
  $$
  (\delta^*\omega)_{\alpha_0\cdots\alpha_{p+1}}:=\sum_{i=0}^{p+1}(-1)^i\omega_{\alpha_0\cdots\hat{\alpha_i}\cdots\alpha_{p+1}}
  $$

- 奇异上同调的双复形，谱序列 

  - 一般拓扑空间的 $\text{good cover}$.  可三角剖分空间 ($\text{triangularizable}$). 
  - 纤维丛的奇异上同调的谱序列，$\text{Leray' s theorem}$，$\text{K\"unneth formula}$, 乘法结构. 
  - 一些例子 ($S(T_{S^k}),\,\mathrm{SO}(3),\,\mathrm{SO(4)},\,U(n)$ 的上同调群). 

- ❓一点同调代数知识 (感觉用不上，不想讲) 

- 奇异同调的双复形对应的谱序列 



- **Motivation:** 想将纤维丛谱序列的计算过程推广至一般的 $\pi:E\rightarrow X$, 有一个技术要求是 
  $$
  H^q(\pi^{-1}U)\simeq H^q(F), \text{ for some fixed space } F \text{ and for any contractible open set } U.
  $$

- Serre 纤维化 / Hurewicz 纤维化 ($\text{Fibration}$) 

  - 定义: 满足同伦提升性 
  - :star2:性质: 1)... 2)... 

- 道路纤维化 ($\text{The Path Fibration}$) 

  - 道路空间 $P(X)$, 回路空间 $\Omega(X)$ 的定义. 
  - 为什么 $\pi:P(X)\rightarrow X$ 是纤维化. 
  - $H^*(\Omega(S^n))$ 的计算. 