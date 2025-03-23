# §4. Stiefel-Whitney Classes 



### 1. DEFINITION 

- **AXIOM 1.** 
  $$
  w_i(\xi)\in H^i(B(\xi);\mathbb{Z}_2),\quad i=0,1,2,\dots,
  $$
  We stipulate 
  $$
  w_0(\xi)=1\in H^0(B(\xi);\mathbb{Z}_2),
  $$
  and 
  $$
  w_i(\xi) = 0,\quad\text{for}\;i>\text{rank}\,\xi.
  $$

- **AXIOM 2.** **NATURALITY.** 
  $$
  w_i(f^*\eta)=f^*w_i(\eta).
  $$
  
- **AXIOM 3.** **THE WHITNEY PRODUCT THEOREM.** 
  $$
  w_k(\xi\oplus\eta)=\sum_{i=0}^{k}w_i(\xi)\cup w_{k-i}(\eta). 
  $$
  For example 
  $$
  \left\{
  \begin{gathered}
  w_1(\xi\oplus\eta)=w_1(\xi)+w_1(\eta),\\
  w_2(\xi\oplus\eta)=w_2(\xi)+w_1(\xi)w_1(\eta)+w_2(\eta), \\
  \cdots\cdots
  \end{gathered}
  \right.
  $$

- **AXIOM 4.** **NORMALIZATION.** 
  $$
  w_1(\gamma^1_1)\neq0
  $$
  where $\gamma^1_1$ is the canonical (tautological) line bundle over.



**REMARK.** It is not at all obvious that classes $w_1(\xi)$ satisfying the four axioms can be defined. In this section we assume they do exist, and we give some applications. 



### 2. Consequence of the Four Axioms 

- **Proposition 1**: 
  $$
  \xi\cong\eta\Rightarrow w_{i}(\xi)=w_{i}(\eta).
  $$
  **proof.** Let $f:E(\xi)\rightarrow E(\eta)$ be the isomorphic map, $f\big|_{B(\xi)}:B(\xi)\rightarrow B(\eta)$ is identity. Then 
  $$
  w_i(\xi) = w_i(f^*\eta)=f^*w_i(\eta)=w_i(\eta),\quad i=0,1,2,\dots
  $$

- **Proposition 2**: 
  $$
  \xi\text{ trivial v.b.}\Rightarrow w(\xi)=1.
  $$
  **proof.** Let $\text{pt}\times\mathbb{R}^n$ be a v.b. over a point. $\varepsilon$ can be viewed as the pull-back bundle induced by the constant map $c:B(\varepsilon)\rightarrow\text{pt}$. Since $H^i(\text{pt})=0$ for $i>0$. So 
  $$
  w_i(\varepsilon) = c^*w_i(\text{pt}\times\mathbb{R}^n) = 0,\quad i>0.
  $$

- **Proposition 3**: 
  $$
  w_{i}(\varepsilon\oplus\eta)=w_{i}(\eta), \text{ for }\varepsilon \text{ trivial v.b.}
  $$

- **Proposition 4**: If $\xi$ is an $\mathbb{R}^{n}$-bundle with a Euclidean metric which possesses a nowhere zero cross-section, then $w_{n}(\xi)=0$. If $\xi$ possesses $k$ cross-sections which are nowhere linearly dependent, then 
  $$
  w_{n - k + 1}(\xi)=w_{n - k + 2}(\xi)=\cdots=w_{n}(\xi)=0
  $$



An interesting case is that $\xi\oplus\eta$ is trivial. The Whitney product theorem provides that one can compute all the $w_i(\eta)$ from $w_i(\xi)$, and vice versa. 



- **DEFINITION (the ring consisting of all formal infinite series).** 
  $$
  \mathrm{H}^{\mathrm{II}}(\mathrm{B};\mathbb{Z}_2):=\Big\{\mathrm{a}=\mathrm{a}_{0}+\mathrm{a}_{1}+\mathrm{a}_{2}+\cdots\,\Big|\,\mathrm{a}_{\mathrm{i}}\in\mathrm{H}^{\mathrm{i}}(\mathrm{B};\mathbb{Z}_2)\Big\}
  $$
  with product 
  $$
  (\mathrm{a}_{0}+\mathrm{a}_{1}+\mathrm{a}_{2}+\cdots)(\mathrm{b}_{0}+\mathrm{b}_{1}+\mathrm{b}_{2}+\cdots)=(\mathrm{a}_{0}\mathrm{b}_{0})+(\mathrm{a}_{1}\mathrm{b}_{0}+\mathrm{a}_{0}\mathrm{b}_{1})+(\mathrm{a}_{2}\mathrm{b}_{0}+\mathrm{a}_{1}\mathrm{b}_{1}+\mathrm{a}_{0}\mathrm{b}_{2})+\cdots.
  $$
  This product is commutative (since we are working modulo $2$) and associative. 


- **DEFINITION (The total Stiefel-Whitney class).** 
  $$
  \mathrm{w}(\xi)=1 + \mathrm{w}_{1}(\xi)+\mathrm{w}_{2}(\xi)+\cdots+\mathrm{w}_{n}(\xi)+0+\cdots
  $$
  Note that the Whitney product theorem can now be expressed by the simple formula 

	$$
	\mathrm{w}(\xi\oplus\eta)=\mathrm{w}(\xi)\mathrm{w}(\eta).
	$$

- **Lemma.** The collection of all infinite series 
	$$
	\mathrm{w}=1 + \mathrm{w}_{1}+\mathrm{w}_{2}+\cdots \in \mathrm{H}^{\mathrm{II}}(\mathrm{B};\mathbb{Z}_2)
	$$
	forms a commutative group under multiplication. (This is precisely the group of units of the ring $\mathrm{H}^{\mathrm{II}}(\mathrm{B};\mathbb{Z}_2)$.) 
	
	**proof.** We can proof it by induction. 
	
	Alternatively $\overline{\mathrm{w}}$ can be computed by the power series expansion: 
	$$
	\begin{align*}
	\overline{\mathrm{w}}&=[1 +	(\mathrm{w}_{1}+\mathrm{w}_{2}+\mathrm{w}_{3}+\cdots)]^{-1}\\
	&=1-(\mathrm{w}_{1}+\mathrm{w}_{2}+\mathrm{w}_{3}+\cdots)+(\mathrm{w}_{1}+\mathrm{w}_{2}+\cdots)^{2}-(\mathrm{w}_{1}+\mathrm{w}_{2}+\cdots)^{3}+\cdots\\
	&=1-\mathrm{w}_{1}+(\mathrm{w}_{1}^{2}-\mathrm{w}_{2})+(-\mathrm{w}_{1}^{3}+2\mathrm{w}_{1}\mathrm{w}_{2}-	\mathrm{w}_{3})+\cdots
	\end{align*}
	$$
	This leads to the precise expression $\frac{(i_{1}+\cdots + i_{k})!}{i_{1}!\cdots i_{k}!}$ for the coefficient of $\mathrm{w}_{1}^{i_{1}}\mathrm{w}_{2}^{i_{2}}\cdots\mathrm{w}_{k}^{i_{k}}$ in $\overline{\mathrm{w}}$. 



- **Lemma (Whitney duality theorem).** If $M$ is embedded in Euclidean space, $\nu$ is the normal bundle then 
  $$
  \mathrm{w}_{i}(\nu)=\overline{\mathrm{w}}_{i}(\tau_{\mathrm{M}}).
  $$

- **Example ($w(S^n)$).** For the standard embedding $S^{n}\subset\mathbb{R}^{n+1}$, the normal bundle is trivial. 
  $$
  w(\tau)w(\nu)=1,\;w(\nu)=1\Rightarrow w(\tau)=1.
  $$
  

### 3. Bundles over $\mathbb{R}P^n$. 

To compute the Stiefel-Whitney classes of bundles over $\mathbb{R}P^n$, it is forst necessary to describe the $\mod 2$ cohomology of $\mathbb{R}P^n$. 

- **Lemma.** 
  $$
  H^i(\mathbb{R}P^n,\mathbb{Z}_2)=
  \begin{cases}
  \mathbb{Z}_2, & 0\leq i\leq n; \\
  0, & i>n.
  \end{cases}
  $$
  Furthermore, 
  $$
  H^*(\mathbb{R}P^n,\mathbb{Z}_2) = \mathbb{Z}_2[a]/(a^{n+1})
  $$
  where $a$ denote the non-zero element (hence a generator) of $H^1(\mathbb{R}P^n,\mathbb{Z}_2)$. 
  
  

1. **Canonical line bundle $\gamma^1_n$.** 
   $$
   w(\gamma^1_n)=1+a.
   $$

2. **$\gamma^{\perp}$ (the orthognoal complement of $\gamma^1_n$ in $\varepsilon^{n+1}$).** 
   $$
   w(\gamma^{\perp})=1+a+a^2+\cdots+a^n.
   $$

3. **The tangent bundle $\tau(\mathbb{R}P^n)$.** 

   1. $$
      \tau(\mathbb{R}P^n)\cong\mathrm{Hom}(\gamma^1_n,\gamma^{\perp}).
      $$

   2. $$
      \begin{align}
      \tau\oplus\varepsilon^1 & \cong\mathrm{Hom}(\gamma^1_n,\gamma^{\perp})\oplus\mathrm{Hom}(\gamma^1_1,\gamma^1_1)=\mathrm{Hom}(\gamma^1_1,\gamma^{\perp}\oplus\gamma^1_1)=\mathrm{Hom}(\gamma^1_1,\varepsilon^{n+1}) \\
      & \cong\mathrm{Hom}(\gamma^1_1,\varepsilon^{1})\oplus\cdots\oplus\mathrm{Hom}(\gamma^1_1,\varepsilon^{1})\cong\gamma^1_1\oplus\cdots\gamma^1_1
      \end{align}
      $$

   3. $$
      w(\mathbb{R}P^n)=(1+a)^{n+1}=1+\binom{n+1}{1}a+\binom{n+1}{2}a^2+\cdots+\binom{n+1}{n}a^n.
      $$

   4. Here is a table of the binomial coefficient $\binom{n+1}{i}\mod 2$, for $n\leq14$. 


<style>
    table th, table td {
        text-align: center;
    }
</style>
<table>
  <col> <!-- 第一列宽度自适应 -->
  <col style="width: 800px"> <!-- 第二列设置固定宽度 -->
  <tr>
    <th></th>
    <td>1</td>
  </tr>
  <tr>
    <th></th>
    <td>1&nbsp 1</td>
  </tr>  
  <tr>
    <th>P^1</th>
    <td>1&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^2</th>
    <td>1&nbsp 1&nbsp 1&nbsp 1</td>
  </tr>
  <tr>
    <th>P^3</th>
    <td>1&nbsp 0&nbsp 0&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^4</th>
    <td>1&nbsp 1&nbsp 0&nbsp 0&nbsp 1&nbsp 1</td>
  </tr>
  <tr>
    <th>P^5</th>
    <td>1&nbsp 0&nbsp 1&nbsp 0&nbsp 1&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^6</th>
    <td>1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1</td>
  </tr>
  <tr>
    <th>P^7</th>
    <td>1&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^8</th>
    <td>1&nbsp 1&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 1&nbsp 1</td>
  </tr>
  <tr>
    <th>P^9</th>
    <td>1&nbsp 0&nbsp 1&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 1&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^10</th>
    <td>1&nbsp 1&nbsp 1&nbsp 1&nbsp 0&nbsp 0&nbsp 0&nbsp 0&nbsp 1&nbsp 1&nbsp 1&nbsp 1</td>
  </tr>
  <tr>
    <th>P^11</th>
    <td>1&nbsp 0&nbsp 0&nbsp 0&nbsp 1&nbsp 0&nbsp 0&nbsp 0&nbsp 1&nbsp 0&nbsp 0&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^12</th>
    <td>1&nbsp 1&nbsp 0&nbsp 0&nbsp 1&nbsp 1&nbsp 0&nbsp 0&nbsp 1&nbsp 1&nbsp 0&nbsp 0&nbsp 1&nbsp 1</td>
  </tr>
  <tr>
    <th>P^13</th>
    <td>1&nbsp 0&nbsp 1&nbsp 0&nbsp 1&nbsp 0&nbsp 1&nbsp 0&nbsp 1&nbsp 0&nbsp 1&nbsp 0&nbsp 1&nbsp 0&nbsp 1</td>
  </tr>
  <tr>
    <th>P^14</th>
    <td>1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1&nbsp 1</td>
  </tr>
</table>

- **COROLLARY 4.6 (Stiefel).** The class $w(P^n)$ is equal to 1 if and only if $n + 1$ is a power of 2. Thus the only projective spaces which can be parallelizable are $P^1,P^3,P^7,P^{15},\dots\ $. 

  (We will see in a moment that $P^1$, $P^3$, and $P^7$ actually are parallelizable. On the other hand it is known that the higher projective spaces $P^{15}$, $P^{31},\ldots$ are not parallelizable. See [Bott-Milnor], [Kervaire, 1958], [Adams, 1960].) 



#### Division algebra

- **THEOREM 4.7 (Stiefel).** Suppose that there exists a bilinear product operation 

  [^This product operation is not required to be assosiative, or to have an identity element.]: 

  $$
  p:\mathbb{R}^n \times \mathbb{R}^n \to \mathbb{R}^n
  $$


  without zero divisors. Then the projective space $P^{n - 1}$ is parallelizable, hence $n$ must be a power of $2$. 

  In fact such division algebras are known to exist for $n = 1,2,4,8$: namely **the real numbers**, **the complex numbers**, **the quaternions**, and **the Cayley numbers**. It follows that the projective spaces $P^1$, $P^3$ and $P^7$ are parallelizable. That no such division algebra exists for $n > 8$ follows from the references cited above on parallelizability. 

  **proof.** Let $b_1,\dots,b_n$ be the standard basis for $\mathbb{R}^n$. We define 
  $$
  \begin{align}
  R_{b_i}:\mathbb{R}^n&\rightarrow\mathbb{R}^n \\
  y&\mapsto p(y,b_i)
  \end{align}
  $$
  It is clearly an isomorphism of $\mathbb{R}^n$ to itself. Hence 
  $$
  v_i:=R_{b_i}\circ(R_{b_1})^{-1}
  $$
  is also an automorphism of $\mathbb{R}^n$. Note that $v_1(x),\dots,v_n(x)$ are linearly independent for $x\neq0$ and that $v_1(x)=x$. Since if 
  $$
  k_1v_1(x)+\cdots+k_nv_n(x)=0
  $$
  Let $y=(R_{b_1})^{-1}(x)\neq0$,  then 
  $$
  \begin{align}
  &\; k_1p(y,b_1)+\cdots+k_np(y,b_n)=0 \\
  \Rightarrow &\; p(y,k_1b_1+\cdots+k_nb_n)=0 \\
  \Rightarrow &\; k_1b_1+\cdots+k_nb_n=0 \\
  \Rightarrow &\; k_1=\cdots=k_n=0.
  \end{align}
  $$
  For each line $L$ through the origin, we can define 
  $$
  \bar{v_i}=\mathrm{p}_{L^{\perp}}\circ v_i|_{L}:L\rightarrow L^{\perp}
  $$
  where $\mathrm{p}_{L^{\perp}}$ denote the orthogonal projection from $\mathbb{R}^n$ to $L^{\perp}$. Clearly $\bar{v}_1=0$, and $\bar{v}_2,\dots,\bar{v}_n$ are everywhere linearly independent. Thus they are $n-1$ linearly independent cross-sections of the v.b. 
  $$
  \tau_{\mathbb{R}P^{n-1}}\cong\mathrm{Hom}(\gamma^1_{n-1},\gamma^{\perp}).
  $$
  So the tangent bundle $\tau_{\mathbb{R}P^{n-1}}$ is a trivial bundle. 



#### Immersions

Now we investigate how large $k$ must be for $\mathbb{R}P^n$ being immersed in $\mathbb{R}^{n+k}$. From the Whitney duailty theorem we know that if $M^n$ can be immersed in $\mathbb{R}^{n+k}$, then
$$
w_i(\nu)=\bar{w}_i(M).
$$
Since $w_i(\nu)=0$ for $i>k$, we can get a lower bound of $k$ by viewing the non-zero term of $\bar{w}_i(M)$. i.e. 
$$
\text{If }\bar{w}_l(M)\neq0, \text{ then }k\geq l.
$$
