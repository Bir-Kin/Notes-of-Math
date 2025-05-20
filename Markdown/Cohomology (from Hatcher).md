# Cohomology

### $\S$ Cup Product

**Def:** For cochains $\varphi\in C^k(X;R)$ and $\psi\in C^l(X;R)$, the **cup product** $\varphi\smile\psi\in C^{k+l}(X;R)$ is
$$
(\varphi\smile\psi)(\sigma):=\varphi(\sigma|_{[v_0,\cdots,v_k]})\psi(\sigma|_{[v_k,\cdots,v_n]}).
$$
**Prop:** For $\varphi\in C^k(X;R)$ and $\psi\in C^l(X;R)$, 
$$
\delta(\varphi\smile\psi)=(\delta\varphi)\smile\psi+(-1)^k\varphi\smile\delta\psi.
$$
Thus it induces a cup prduct of cohomology groups
$$
H^k(X;R)\times H^l(X;R)\xrightarrow{\smile} H^{k+l}(X;R).
$$
It also gives relative cup products 
$$
H^k(X;R)\times H^l(X,A;R)\xrightarrow{\smile} H^{k+l}(X,A;R), \\
H^k(X,A;R)\times H^l(X;R)\xrightarrow{\smile} H^{k+l}(X,A;R), \\
H^k(X,A;R)\times H^l(X,A;R)\xrightarrow{\smile} H^{k+l}(X,A;R).
$$
More generally, 
$$
H^k(X,A;R)\times H^l(X,B;R)\xrightarrow{\smile} H^{k+l}(X,A\cup B;R)
$$
<span style="color:gray">
To get this, we first have</span> 
$$
\color{gray}C^k(X,A;R)\times C^l(X,B;R)\xrightarrow{\smile} C^{k+l}(X,A+B;R)
$$
<span style="color:gray">then we use the fact that inclusion</span> 
$$
\color{gray}C^n(X,A\cup B;R)\rightarrow C^n(X,A+B;R)
$$
<span style="color:gray">induces isomorphism on cohomology.</span> 

**Prop:** For a map $f:X\rightarrow Y$, the induced maps $f^*:H^n(Y;R)\rightarrow H^n(X;R)$ satisfy 
$$
f^*(\alpha\smile\beta)=(f^*\alpha)\smile(f^*\beta).
$$
**Thm:** When $R$ is commutative, for $\alpha\in H^k(X,A;R)$ and $\beta\in H^l(X,A;R)$, we have 
$$
\alpha\smile\beta=(-1)^{kl}\beta\smile\alpha
$$
 proof: The key is to define a **reversing map** 
$$
\begin{align}
\rho:C_n(X)&\rightarrow C_n(X) \\
\sigma&\mapsto(-1)^{\frac{n(n+1)}{2}}\bar{\sigma}
\end{align}
$$
It can be shown that $\rho$ is a chain map and is homotopic to the identity, so it induces the identity on cohomology. 

