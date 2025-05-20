# Homology of Manifolds

**Definition**  Let $ M $ be a fixed $ n $-dimensional manifold, not necessarily compact. We will first study the groups $ H_i(M, M - K) $ where $ K $ denotes a compact subset of $ M $. If $ K \subset L \subset M $, then the natural homomorphism  
$$
\rho_K : H_i(M, M - L) \to H_i(M, M - K)
$$
maps elements via restriction. The image $ \rho_K(\alpha) $ represents the <span style="color:red">"restriction"</span> of $ \alpha $ to $ K $.

**LEMMA A.7** 
The groups $H_i(M, M-K)$ are zero for $i>n$. A homology class $\alpha \in H_n(M, M-K)$ is zero if and only if the restriction 
$$
\rho_x(\alpha) \in H_n(M, M-x)
$$
is zero for each $x \in K$.

<span style="color:red">**Remark:** The key is the reversal direction. Which means that if $\alpha$ restrict to every point $x\in K$ is zero, then $\alpha$ itself is zero.</span> 



### The Fundamental Homology Class of Manifold

**DEFINITION** 
A *local orientation* $\mu_x$ for $M$ at $x$ is a choice of one of the two possible generators for $H_n(M, M - x; \mathbb{Z})$. 

**DEFINITION** 
An *orientation for M* is a function which assigns to each point $ x \in M $ a local orientation $ \mu_x $, such that the $ \mu_x $ vary "continuously" with $ x $. More precisely, for each $ x $ there exists a compact neighborhood $ N $ and a class $ \mu_N \in H_n(M, M - N) $ satisfying $ \rho_y(\mu_N) = \mu_y $ for all $ y \in N $. 

**THEOREM A.8** 
For any oriented manifold $M$ and any compact $K \subset M$, there is one and only one class $\mu_K \in H_n(M, M - K)$ which satisfies $\rho_x(\mu_K) = \mu_x$ for each $x \in K$. 
In particular, if $M$ itself is compact, then there is one and only one $\mu_M \in H_n(M)$ with the required property. This class $\mu = \mu_M$ is called the *fundamental homology class* of $M$. 

**REMARK 2.** 
Similar considerations apply to an oriented manifold-with-boundary $M$. For each compact subset $K \subset M$, there exists a unique class $\mu_K \in H_n(M, (M - K) \cup \partial M)$ with the property that $\rho_x(\mu_K) = \mu_x$ for each $x \in K \cap (M - \partial M)$.  In particular, if $M$ is compact, then there is a unique fundamental homology class $\mu_M \in H_n(M, \partial M)$ with the required property. It can be shown that the natural homomorphism  
$$
\partial : H_n(M, \partial M) \to H_{n-1}(\partial M)
$$
maps $\mu_M$ to the fundamental homology class of $\partial M$. *(Compare [Spanier, p. 304].)*  
