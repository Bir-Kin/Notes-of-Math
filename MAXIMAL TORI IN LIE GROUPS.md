# MAXIMAL TORI IN LIE GROUPS

**Notice.** From now on $G$ is a compact connected $\mathrm{Lie}$ group. 

### 1. Definition of Maximal tori and its basic properties

- **Definition.** A Maximal torus $T\subset G$ is : 

  1. a subgroup which is a torus, such that
  2. if $T\subset U\subset G$ and $U$ is a torus then $T=U$. 

  

  -  **Remark. ** If $G$ is not compact, it need not have any non-trivial tori. For example $\mathbb{R}^n$. I guess ${\rm Heisenberg\; group}$ may also be an example. 
  - **Proposition.** Any subtorus of $G$ is contained in a maximal torus. 
  - **Proposition.** Let $T$ be a maximal torus of $G$, and $A$ a connected Abelian subgroup of $G$ with $T\subset A$. Then $T=A$. 



 ### 2. Roots of compact connected $\rm{Lie}$ groups 

- **CONSTRUCTIONS.** If $T$ is a torus of $G$, it operates on $G_e$ by $T\subset G\overset{{\rm Ad}}{\rightarrow}{\rm Aut}\, G_e$. Choose a positive definite symmetric form on $G_e$ invariant under $G$, and so under $T$. Then (3.78) splits into orthogonal irreducible $T$-spaces of dimensions $1$ and $2$.Those of dimension $1$ are trivial. We can choose anorthonormal base in those of dimension $2$, and represent T by $T→{\rm SO}(2)$. 

- **DEFINITION.** The integer lattice of $L(T)$ is $\mathrm{exp}^{-1}(e)$ where $\mathrm{exp} : L(T)\rightarrow T$. 

- **PROPOSITION.** $L(G)=G$ splits as a $T$-space in the form $V_0\oplus\sum_i^mV_i$, where $T$ acts on $V_0$, trivially, ${\rm dim} V_i = 2$ for $i >0$ and $T$ acts on $V_i$ as 
  $$
  \begin{bmatrix}
  {\rm cos}2\pi\theta_i(t) & -{\rm sin}2\pi\theta_i(t) \\ 
  {\rm sin}2\pi\theta_i(t) & {\rm cos}2\pi\theta_i(t)
  \end{bmatrix}.
  $$
  Here $θ_i:T\rightarrow \mathbb{R}/\mathbb{Z}$ is given by a linear form $θ_i:L(T)\rightarrow\mathbb{R}$ taking integer values on the integer lattice, and no $\theta_i$ is zero. 

- **DEFINITION.** If $T$ is a maximal torus, the functions $\pm\theta_i$ are called the roots of $G$, By 3.24 they are well definedin terms of $T$, We will see that they are independent of $T$. 
  - **PROPOSITION (极大环面子群的刻画).** $T$ is maximal if and only if $V_0=L(T)$. 
    - **COROLLARY.** $\mathrm{dim} G-\mathrm{dim} T$ is even.



### 3. Conjugation theorem

- **THEOREM (共轭定理🌟).** Let $T\subset G$ be a maximal torus. Then any $g\in G$ is contained in a conjugate of $T$. 

  - **COROLLARY.** Every element of $G$ lies in a maximal torus, since the conjugate of a maximal torus is a maximal torus. 

  - **COROLLARY.** Any two maximal tori, $T$, $U$ are conjugate. 

    Hence any construction apparently dependent on a choice of $T$ is independent of the choice up to an inner automorphis m of $G$. 

- **DEFINITION.** It follows that any two maximal tori have the same dimension. This is called the rank of $G$, and written $k$ or $l$. 
- **PROPOSITION (工具型引理).** Let $S$ be a connected Abelian subgroupof $G$, and let $g\in G$ commute with all elements of $S$. Then there is a torus $T$ containing $g$ and $S$. 
- **PROPOSITION (工具型引理).** Let $T$ be a maximal torus of $G$. If $T\subset A\subset G$ where $A$ is Abelian, then $T=A$. That is, a maximal torus is a maximal Abelian subgroup.



### 4. Wely group $W$ 

#### Wely 群的定义

- **DEFINITION.** Let $T$ be a maximal torus of $G$. Then the \underline{Weyl group} $W$ (or $\varPhi$) of $G$ is the group of automorphisms of $T$ which are the restrictions of inner automorphisms of $G$. This is independent of the choice of $T$.

  Any such automorphism has the form $t\to ntn^{-1}, n\in N(T)$​. Let 

  $$
  \begin{align}
  c:G&\rightarrow\mathrm{Inn}\,G \\
  g&\mapsto(x\mapsto gxg^{-1})
  \end{align}
  $$
  
  
  $N(T)$ is a closed subgroup of $G$, and so compact. Let $Z(T)$ be the centraliser of $T$, that is, the set of $z\in G$ such that $ztz^{-1}=t$ all $t\in T$. $Z(T)$ is also closed, and $T\subset Z(T)\subset N(T)$. Thus $N(T)$ maps onto $N(T)/Z(T)\cong W$. $N(T)/T$ is finite (see the proof of 4.21), so $W$ is finite. 
  
  Since we are considering $G$ connected, $Z(T)=T$ (4.25), and $W = N(T)/T$. 

#### Wely 群与 Lie 群的表示、根系



### 5. Regularity and Singularity of an element







