**You:**

How does Bott periodicity determine the cohomology groups of compact classical Lie groups?

* * *

**ChatGPT:**

以下从 Bott 周期性定理的基本思路出发，说明它如何帮助我们确定紧致经典李群（主要指 $U(n)$、$SU(n)$、$SO(n)$、$Sp(n)$ 等）的同调（或上同调）群的结构。为了清晰起见，先回顾 Bott 周期性的声明，然后说明如何借助它得到这些李群的同调代数结构。

* * *

## 一、Bott 周期性定理的要点

1. **酉群的 Bott 周期性** 
    Bott 周期性告诉我们，对无限维酉群 $U$ 而言，其循环空间（loop space）存在 2 周期性：
    $$
    \Omega^2 U \;\simeq\; U \times \mathbb{Z},
    $$
    
    或者更常见的同伦等价写法为
    
    $$
    \Omega U \;\simeq\; \mathbb{Z}\times BU,\quad  
    \Omega^2 U \;\simeq\; U,\quad  
    \Omega^3 U \;\simeq\; \mathbb{Z}\times BU,\;\dots
    $$
    
    这里 $\Omega$ 表示“基于某个特定基点的循环空间（基环空间）”，$BU$ 则是“无限维酉群的类空间（classifying space）”。上述等价蕴含：
    
    * 对于所有 $k\ge1$，都有
      
        $$
        \pi_{k}(U)\;\cong\;\pi_{k+2}(U),
        $$
        
        即单位ary 群的同伦群具有周期 $2$。
    
2. **正交群／辛群的 Bott 周期性** 
    类似地，对正交群和辛群，也存在各自的周期性：
    
    * **正交群** $O$（或连通分支 $SO$）的循环空间满足
      
        $$
        \Omega^8 SO \;\simeq\; SO,
        $$
        
        因此 $\pi_k(SO)\cong\pi_{k+8}(SO)$，具有周期 8。
        
    * **辛群** $Sp$（注意 $Sp(n)$ 含为紧致矩阵群的连通盖）同样满足 8 周期：
      
        $$
        \Omega^8 Sp \;\simeq\; Sp.
        $$

这些“循环空间同伦等价”为我们分析同伦群、同调群提供了极其有力的工具。下一步，将这些同伦信息如何传递到同调信息，并最终确定李群的同调代数结构。

* * *

## 二、从同伦到同调：利用 Hurewicz 与 Hopf 代数结构

1. **李群的 Hurewicz 同构** 
    对于每个紧致单连通李群 $G$（例如 $SU(n)$、$Sp(n)$ 等），它是一个有限维的 CW 复形，且作为连通的 Lie 群，其 $\pi_1$ 是有限的（或者对于 $SU(n)$、$Sp(n)$，$\pi_1=0$）。利用 Bott 周期性可以知道这些群的低阶同伦群在奇数维度“滞后”为 $\mathbb{Z}$，偶数维度为 $0$。具体地，以 $U(n)$ 为例（所谓“稳定”后取 $n\to\infty$ 的情况记作 $U$）：
    $$
    \pi_{2m}(U)\;=\;0,\quad  
    \pi_{2m-1}(U)\;\cong\;\mathbb{Z},\qquad m\ge1.
    $$
    
    对于有限维的 $U(n)$，当阶数小于 $2n$ 时，也有相同的规律。类似地，$SU(n)$、$Sp(n)$、$SO(n)$ 这些群在“低阶”同伦群也都能通过 Bott 周期性和有限维截断（stable range）得出 $\mathbb{Z}$ 或 $0$ 的分布。
    
    然后，由于 $G$（连通且 $\pi_1$ 或有限，且 $\pi_i(G)$ 在 $i<\dim G$ 时能用 Bott 调控）的 Hurewicz 同构定理可知：
    
    * 第 $k$ 阶同伦群 $\pi_k(G)$（当 $k$ 足够小，以至于 $\pi_1,\dots,\pi_{k-1}$ 没有贡献的时候）会映射到第 $k$ 阶同调群 $H_k(G;\mathbb{Z})$，并且在那些奇数维度上给出 $\mathbb{Z}$ 的生成元。
      
    * 换言之，奇数维度的 $\pi_{2m-1}(G)\cong \mathbb{Z}$ “对应” 到 $H_{2m-1}(G;\mathbb{Z})\cong\mathbb{Z}$。
    
2. **Hopf 代数结构与上同调环** 
    紧致李群 $G$ 是一个 $H$-空间（在光滑意义下，它同时具有可微结构与群结构），其上同调 $H^*(G;\mathbb{Z})$ 是一个 Hopf 代数。在连通且同调为无扭的情况下（对 $U(n)$、$SU(n)$、$Sp(n)$、$SO(n)$ 这些群，系数用 $\mathbb{Z}$ 时上同调是没有扭的），根据 Hopf 代数的结构定理，可以断言：
    
    * 如果 $H_*(G;\mathbb{Z})$（当用奇数维度的同调生成时，只在若干奇数维度有生成元）形成一个外部乘积（Exterior algebra）的代数，那么 $H^*(G;\mathbb{Z})$ 就也是一个外部代数（Exterior algebra）。
      
    * 具体而言，当 $G$ 连通且奇数维度有 $r$ 个自由生成元时，作为上同调环，$H^*(G;\mathbb{Z})$ 必定同构于
      
        $$
        \Lambda_{\mathbb{Z}}(\;x_{d_1},\,x_{d_2},\,\dots,\,x_{d_r}\;),
        $$
        
        其中每个 $x_{d_i}$ 都是奇数维度 $d_i$ 上的一个生成元。
    
3. **由 Bott 周期性给出具体的奇数维生成元位置**
   
    * **对于 $U(n)$**：通过 Bott 周期性可知，在“稳定区间”内（即 $k<2n$ 时），
      
        $$
        \pi_{2m-1}(U(n))\;\cong\;\mathbb{Z},\quad 1\le m\le n.
        $$
        
        而在偶数维度则 $\pi_{2m}(U(n))=0$。因此，Hurewicz 同构给出
        
        $$
        H_{2m-1}(U(n);\mathbb{Z})\;\cong\;\mathbb{Z},  
        \quad  
        m=1,2,\dots,n,
        $$
        
        对应到上同调后，$H^*(U(n);\mathbb{Z})$ 就是由 $n$ 个奇数维生成元构成的外部代数：
        
        $$
        H^*(U(n);\mathbb{Z})  
        \;\cong\;  
        \Lambda_{\mathbb{Z}}\bigl(e_{1}, e_{3}, e_{5},\dots, e_{2n-1}\bigr),
        $$
        
        其中 $\deg(e_{2m-1})=2m-1,(,;m=1,\dots,n)$。这正是经典结果：
        
        $$
        H^k(U(n);\mathbb{Z})\;=\;  
        \begin{cases}  
        \text{自由阿贝尔群，生成元来自奇数维度上的外部形式} & \text{若 }k\in\{1,3,5,\dots,2n-1\}\text{ 的若干子和},\\  
        0 & \text{其他维度}.  
        \end{cases}
        $$
    * **对于 $SU(n)$**：因为 $SU(n)$ 是 $U(n)$ 上的 $;S^1$ 中心子群（对应行列式为 1），有正合列
      $$
        1 \;\longrightarrow\; S^1 \;\longrightarrow\; U(n) \;\longrightarrow\; SU(n)\;\longrightarrow\; 1.
      $$
      
        对应同调测序可推出 $H^*(SU(n);\mathbb{Z})$ 同构于
      
      $$
      \Lambda_{\mathbb{Z}}(e_{3},\,e_{5},\,e_{7},\,\dots,\,e_{2n-1}),
      $$
      
        也就是说，省去了 $e_1$ （即 $U(n)$ 中的那一维）后，余下的奇数维生成元依旧保持外部代数结构。这里的第一生成元是度数 3，即去掉了 $U(n)$ 中 $\deg=1$ 的那个因素。
      
    * **对于 $Sp(n)$**（紧致辛群）也是同理。由于 Bott 周期性告诉我们 $\pi_{2m-1}(Sp(n))=\mathbb{Z}$ 当且仅当 $m=1,2,\dots,n$（且维度对应要比单位群“延后”一些，具体生成度是 $\deg = 4i-1$），但更常见的结论是：
      
        $$
        H^*(Sp(n);\mathbb{Z})  
        \;\cong\;  
        \Lambda_{\mathbb{Z}}\bigl(y_{3},\,y_{7},\,y_{11},\,\dots,\,y_{4n-1}\bigr),
        $$
        
        其中 $\deg(y_{4i-1})=4i-1,;i=1,\dots,n$。这也可由 Bott 周期性结合 Hurewicz 得到。
        
    * **对于 $SO(n)$**（或其连通分支 $Spin(n)$）：由于 Bott 周期性是 8 周期，且同伦群在奇数维或某些特定维度上是 $\mathbb{Z}$，通过 Hurewicz 可以得到 $H_{k}(SO(n);\mathbb{Z})$ 在某些奇数维度为 $\mathbb{Z}$。具体地，常见经典结果表明（假设 $n$ 足够大，使得稳定区间生效）：
      $$
        H^*(SO(2m+1);\mathbb{Z})\;\cong\;  
        \Lambda_{\mathbb{Z}}\bigl(z_{3},\,z_{7},\,z_{11},\,\dots,\,z_{4m-1}\bigr),
        $$
        $$
        H^*(SO(2m);\mathbb{Z})\;\cong\;  
        \Lambda_{\mathbb{Z}}\bigl(z_{3},\,z_{7},\,z_{11},\,\dots,\,z_{4m-5},\,z_{2m-1}\bigr),
        $$
        
        各生成元的度数 (3, 7, 11, …) 与 Bott 周期性预测的同伦群 $\pi_{2k-1}(SO)$ 对应，且可以通过逐步分析纤维丛
        
        $$
        SO(n-1)\longrightarrow SO(n)\longrightarrow S^{n-1}
        $$
        
        以及 Bott 周期性叠加来归纳得到这些生成元所在的维度。
        
    
    总之，利用 Bott 周期性得知 $\pi_{2m-1}(G)\cong\mathbb{Z}$，而偶数维度同伦群为 $0$，通过 Hurewicz 同构可见 $H_{2m-1}(G;\mathbb{Z})\cong \mathbb{Z}$。结合 Hopf 代数的“奇数维生成元必然生成一个外部代数”的事实，就能推导出 $H^*(G;\mathbb{Z})$ 是外部代数，且生成元恰好位于 Bott 周期性所给出的那些奇数维度上。
    

* * *

## 三、总结各经典群的上同调结果

下面统一列出紧致经典李群在稳定范围内（即群维度足够大，以保证 Bott 周期性所控制的所有生成元都“出现”）的上同调代数结构。为了简洁，只写出环同构类型与各生成元所在的度数。

1. **单位群 $U(n)$**
   
    $$
    H^*(U(n);\mathbb{Z})  
    \;\cong\;  
    \Lambda_{\mathbb{Z}}\bigl(x_{1},\,x_{3},\,x_{5},\,\dots,\,x_{2n-1}\bigr),
    $$
    
    其中 $\deg(x_{2m-1}) = 2m-1,;m=1,2,\dots,n$。
    
2. **特殊单位群 $SU(n)$**
   
    $$
    H^*(SU(n);\mathbb{Z})  
    \;\cong\;  
    \Lambda_{\mathbb{Z}}\bigl(x_{3},\,x_{5},\,x_{7},\,\dots,\,x_{2n-1}\bigr),
    $$
    
    省去了度数 $1$ 的生成元。
    
3. **紧致辛群 $Sp(n)$**
   
    $$
    H^*(Sp(n);\mathbb{Z})  
    \;\cong\;  
    \Lambda_{\mathbb{Z}}\bigl(y_{3},\,y_{7},\,y_{11},\,\dots,\,y_{4n-1}\bigr),
    $$
    
    其中 $\deg(y_{4i-1}) = 4i-1,;i=1,2,\dots,n$。
    
4. **奇数维正交群 $SO(2m+1)$**
   
    $$
    H^*(SO(2m+1);\mathbb{Z})  
    \;\cong\;  
    \Lambda_{\mathbb{Z}}\bigl(z_{3},\,z_{7},\,z_{11},\,\dots,\,z_{4m-1}\bigr).
    $$
5. **偶数维正交群 $SO(2m)$**
   
    $$
    H^*(SO(2m);\mathbb{Z})  
    \;\cong\;  
    \Lambda_{\mathbb{Z}}\bigl(z_{3},\,z_{7},\,z_{11},\,\dots,\,z_{4m-5},\,z_{2m-1}\bigr).
    $$
    
    注意最后一个生成元 $\deg(z_{2m-1})=2m-1$ 是因为尽管 Bott 周期性是 8，但在截断到有限维 $SO(2m)$ 时，最后会有一个跌落到 $2m-1$ 维的生成元。
    

* * *

## 四、具体机理小结

1. **Bott 周期性给出同伦群的周期性分布** 
    先通过 Bott 周期性定理了解在“无限维稳定情形”或“适当稳定区间”内，$\pi_k(G)$ 何时为 $\mathbb{Z}$、何时为 $0$。对 $U(n)$ 来说，$\pi_{2m-1}(U(n))=\mathbb{Z}$ 当 $m\le n$，$\pi_{2m}(U(n))=0$；对 $SU(n)$、$Sp(n)$、$SO(n)$ 等类似。
    
2. **Hurewicz 同构定理** 
    当 $k$ 低于某个“第一非平凡同伦群出现之前”的维度时（即 $\pi_1,\dots,\pi_{k-1}$ 都不会干扰第 $k$ 阶同调），有
    $$
    Hurewicz:\quad \pi_k(G)\;\xrightarrow{\cong}\;H_k(G;\mathbb{Z}).
    $$
    
    因此，奇数阶 $\pi_{2m-1}(G)\cong\mathbb{Z}$ 对应 $H_{2m-1}(G;\mathbb{Z})\cong\mathbb{Z}$；偶数阶同伦群为 $0$ 则同调也为 $0$。
    
3. **Hopf 代数结构** 
    紧致李群（连通、无扭）其同调环 $H^*(G;\mathbb{Z})$ 是一个 Hopf 代数。对连通、单连通（或仅仅 $\pi_1$ 为有限）的情形，若同调只在若干奇数维度出现单参数（$\mathbb{Z}$），则该 Hopf 代数只能是外部代数。生成元的位置（度数）就对应那些奇数阶同伦群所在的位置。
    
4. **由 Bott 周期性得出同调环** 
    最终把上述三步连起来，就得到了“在 Bott 周期性控制下，紧致经典李群的上同调是某个外部代数，且生成元度数即来自 Bott 周期性中同伦群非平凡的奇数维度”。

* * *

## 五、结语

综上所述，**Bott 周期性定理** 的核心作用在于：

1. 确定了紧致李群（尤其是经典系列：$U(n)$、$SU(n)$、$SO(n)$、$Sp(n)$）在“稳定区间”内的同伦群分布——所有偶数维度同伦群为 0，若干奇数维度同伦群为 $\mathbb{Z}$，并且呈现周期结构（$U$ 群是周期 2，正交／辛群是周期 8）。
   
2. 由此通过 **Hurewicz 同构** 得到相应维度的同调群，也仅在对应奇数维度生成 $\mathbb{Z}$。
   
3. 最终利用李群的 Hopf 代数结构定理，推出其上同调环必然是一个奇数维外部代数，生成元度数正是 Bott 周期性决定的那些奇数维度。
   

因此，Bott 周期性定理直接决定了紧致经典李群的同调（上同调）群“在奇数维度集中出现 $\mathbb{Z}$，且形成一个外部代数”，进而完全刻画了它们的同调环结构。