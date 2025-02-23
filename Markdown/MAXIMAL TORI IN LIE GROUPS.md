# MAXIMAL TORI IN LIE GROUPS

**Notice.** From now on $G$ is a compact connected $\mathrm{Lie}$ group. 

### 1. Definition of Maximal tori and its basic properties

- **4.6 Definition.** A $\underline{\rm maximal\;torus}$ $T\subset G$ is : 

  1. a subgroup which is a torus, such that
  2. if $T\subset U\subset G$ and $U$ is a torus then $T=U$. 

  -  **4.7 Remark.** If $G$ is not compact, it need not have any non-trivial tori. For example $\mathbb{R}^n$. I guess ${\rm Heisenberg\; group}$ may also be an example. 
  - **4.8 Proposition.** Any subtorus of $G$ is contained in a maximal torus. 
  - **4.9 Proposition.** Let $T$ be a maximal torus of $G$, and $A$ a connected Abelian subgroup of $G$ with $T\subset A$. Then $T=A$. 

------



 ### 2. Roots of compact connected $\rm{Lie}$ groups 

- **4.10 CONSTRUCTIONS.** If $T$ is a torus of $G$, it operates on $G_e$ by $T\subset G\overset{{\rm Ad}}{\rightarrow}{\rm Aut}\, G_e$. Choose a positive definite symmetric form on $G_e$ invariant under $G$, and so under $T$. Then (3.78) splits into orthogonal irreducible $T$-spaces of dimensions $1$ and $2$.Those of dimension $1$ are trivial. We can choose anorthonormal base in those of dimension $2$, and represent T by $T→{\rm SO}(2)$. 

- **4.11 DEFINITION.** The $\underline{\rm integer\;lattice}$ of $L(T)$ is $\mathrm{exp}^{-1}(e)$ where $\mathrm{exp} : L(T)\rightarrow T$. 

- **4.12 PROPOSITION.** $L(G)=G$ splits as a $T$-space in the form $V_0\oplus\sum_i^mV_i$, where $T$ acts on $V_0$, trivially, ${\rm dim} V_i = 2$ for $i >0$ and $T$ acts on $V_i$ as 
  $$
  \begin{bmatrix}
  {\rm cos}2\pi\theta_i(t) & -{\rm sin}2\pi\theta_i(t) \\ 
  {\rm sin}2\pi\theta_i(t) & {\rm cos}2\pi\theta_i(t)
  \end{bmatrix}.
  $$
  ​	Here $θ_i:T\rightarrow \mathbb{R}/\mathbb{Z}$ is given by a linear form $θ_i:L(T)\rightarrow\mathbb{R}$ taking integer values on the integer lattice, and no $\theta_i$ is zero. 

- **4.13 DEFINITION.** If $T$ is a maximal torus, the functions $\pm\theta_i$ are called the $\underline{\rm roots}$ of $G$, By 3.24 they are well definedin terms of $T$, We will see that they are independent of $T$. 
  
  - **4.14 PROPOSITION (极大环面子群的刻画).** $T$ is maximal if and only if $V_0=L(T)$. 
    - **4.15 COROLLARY.** $\mathrm{dim} G-\mathrm{dim} T$ is even.

-----



### 3. Conjugation theorem

- **🌟4.21 THEOREM (共轭定理).** Let $T\subset G$ be a maximal torus. Then any $g\in G$ is contained in a conjugate of $T$. 

  - **4.22 COROLLARY.** Every element of $G$ lies in a maximal torus, since the conjugate of a maximal torus is a maximal torus. 

  - **4.23 COROLLARY.** Any two maximal tori, $T$, $U$ are conjugate. 

    *Hence any construction apparently dependent on a choice of $T$ is independent of the choice up to an inner automorphis m of $G$.* 

- **4.24 DEFINITION.** It follows that any two maximal tori have the same dimension. This is called the $\underline{\rm rank}$ of $G$, and written $k$ or $l$. 
- **4.25 PROPOSITION (工具型引理).** Let $S$ be a connected Abelian subgroupof $G$, and let $g\in G$ commute with all elements of $S$. Then there is a torus $T$ containing $g$ and $S$. 
- **4.26 PROPOSITION (工具型引理).** Let $T$ be a maximal torus of $G$. If $T\subset A\subset G$ where $A$ is Abelian, then $T=A$. That is, a maximal torus is a maximal Abelian subgroup.

-----



### 4. Wely group $W$ 

- **4.29 DEFINITION (Wely 群的定义).** Let $T$ be a maximal torus of $G$. Then the $\underline{\rm Weyl\; group}$ $W$ (or $\varPhi$) of $G$ is the group of automorphisms of $T$ which are the restrictions of inner automorphisms of $G$. This is independent of the choice of $T$.

  ​	Any such automorphism has the form $t\to ntn^{-1}, n\in N(T)$. *Let* 

  $$
  \begin{align}
  A:G&\rightarrow\mathrm{Inn}\,G \\
  g&\mapsto(x\mapsto gxg^{-1})
  \end{align}
  $$
  
  *be the map that send an element of $G$ to an inner automorphism. Wely group contains elements of which $T$ is invariant. That inner automorphism is conjugating the element in the normalization of $T$, i.e. $N(T)$​. So* 
  $$
  W = A(N(T))\;?
  $$
  ​	$N(T)$ is a closed subgroup of $G$, and so compact. Let $Z(T)$ be the centraliser of $T$, that is, the set of $z\in G$ such that $ztz^{-1}=t$ all $t\in T$. $Z(T)$ is also closed, and $T\subset Z(T)\subset N(T)$. Thus $N(T)$ maps onto $N(T)/Z(T)\cong W$. $N(T)/T$ is finite (see the proof of 4.21), so $W$ is finite. 
  
  ​	Since we are considering $G$ connected, $Z(T)=T$ (4.25), and $W = N(T)/T$. 

#### Wely 群与 Lie 群的表示、根系

- **4.30 COROLLARY** of 4.21. Let $V$ be a $G$-space. Then $\chi_V$ is determined by its restriction to $T$ and is invariant under $W$. 

- **4.31 COROLLARY.** The homomorphism $i^*: K(G)\to K(T)$ of (complex) representation rings is mono, and its image is contained in the subring of elements invariant under $W$. 

- **4.32 PROPOSITION.** Restriction gives a one-one correspondence between class functions on $G$ and continuous functions on $T$ invariant under $W$. 

  - **4.33 LEMMA (工具引理).** If $t_1,t_2\in T$ are conjugate in $G$, then there is $w\in W$ with $t_2 = wt_1$. 

- **4.37 PROPOSITION.** $W$ permutes the roots of $G$. 

  $\underline{\rm Proof.}$ For each $w\in W$, $w=\left.A_x\right|_T$ for some $x\in G$, and then $G_e\overset{{A}_x'}{\longrightarrow} G_e$ is the required equivalence, i.e. we have a commutative diagram: 
  
  <img src="C:\Users\bobo\Desktop\数学笔记\Figures\wely群置换根系.png" style="zoom: 40%;" />
  
  This shows that $T\xrightarrow{\mathrm{Ad}}\mathrm{GL}(G_e)$ and $T\xrightarrow{w}T\xrightarrow{\mathrm{Ad}}\mathrm{GL}(G_e)$ are equivalent representation. So they have the same representation decomposition but with a permutation. 

-----



### 5. Regularity and Singularity of an element

- **4.34 LEMMA.** Let $N(g)_1$ be the identity component of the normaliser of some $g\in G$. Then $N(g)_1$ is the union of the maximal tori of $G$ containing $g$. 

  *This lemma describe the centerizer of a fix element $g$. It quantifies the commutativity of $g$.*

- **4.35 COROLLARY.** The following two definitions are equivalent: 

  1. $g\in G$ is $\underline{\rm regular}$ if it is contained in just one maximal torus, $\underline{\rm singular}$ if it is contained in more than one maximal torus. 
  2. $g\in G$ is $\underline{\rm regular}$ if $\dim N(g)=\text{rank }G$, $\underline{\rm singular}$ if $\dim N(g)>\text{rank }G$. 

  *The ${\rm regularity/singularity}$ distinguish the commutativity of different elements. Since every point is contained in some maximal torus, it has at least $\mathrm{rank}\:G$ commutativity. Those which have extra commutativity are said to be singular.* 

- **4.38 DEFINITION.** Let $U_r = \{t\in T ;\; \theta_r(t)\equiv 0 \pmod{1}\}$. $U_r$ is a closed subgroup of $T$ of dimension $k - 1$, where $k = \text{rank }G$. It is clearly monogenic. It need not be connected. 

- **4.40 LEMMA.** If $t$ lies in exactly $\nu$ of the $U_r$, then $\dim N(t)=k + 2\nu$. 

- **4.41 COROLLARY.** $t\in T$ is regular if it lies in no $U_r$, and singular if it lies in some $U_r$. 

  *This corollary gives another description of ${\rm regularity/singularity}$.* 

- **4.42 COROLLARY.** The singular elements of $G$ form a set of dimension $\leq n - 3$, where $n = \dim G$, in the sense that this set is the image of a compact manifold of dimension $n - 3$ under a smooth map. 

  *This corollary tells us the regular elements are 'alomst everywhere'.* 

