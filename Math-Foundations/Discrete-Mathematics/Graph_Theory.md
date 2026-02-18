f# MIT 6.042J 离散数学：从逻辑符号到图论结构 2026-02-18

  
**当前进度：** MIT Lec 6 (Graph Theory)  
**研究方向：** 逻辑建模 / 卫生经济学 (HEOR) / 系统博弈分析

---

## 🛠️ 第一部分：逻辑符号工具箱 (The Symbol Toolkit)

在进入复杂证明前，必须明确“逻辑坐标系”的边界。

| 符号 | 名称 | 逻辑定义 | 典型场景 |
| :--- | :--- | :--- | :--- |
| **$p \vee q$** | **Inclusive OR** | $p, q$ 至少一个为真即可。 | 基础准入条件。 |
| **$p \oplus q$** | **Exclusive OR** | 有且仅有一个为真。**不同时发生**。 | 开关状态、加密密钥。 |
| **$\forall$** | **Universal** | 对集合中**每一个**元素都成立。 | 全局定理。 |
| **$\exists$** | **Existential** | 集合中**至少存在一个**元素成立。 | 寻找反例或特例。 |
| **$d \mid n$** | **Divides** | $d$ 能整除 $n$（余数为 0）。 | 数论/水桶问题。 |
| **$\lfloor x \rfloor$** | **Floor** | 小于等于 $x$ 的最大整数。 | 离散化处理。 |


> **图的正式定义：从构件到系统 
> **在建筑学中，我们看重梁与柱的节点；在图论中，我们将其抽象为 $G = (V, E)$。
> **Vertices (V): 顶点或节点。它是系统的基本单元。
> **Edges (E): 边。它是节点间的二元关系集合。
> **Simple Graph (简单图): 不允许出现自环 (Loops) 或 多重边 (Multiple Edges)。这是我们目前研究的基准坐标系。
> **Adjacency (相邻): 如果两个节点被一条边连接，称其为相邻。


---

## 🕸️ 第二部分：图论核心 (Lec 6: Graph Theory Basics)

### 1. 握手定理 (Handshake Lemma)
**定理内容：** 在任何无向图中，所有顶点的度数（Degree）之和等于边数（Edges）的两倍。
$$\sum_{v \in V} \text{deg}(v) = 2|E|$$

> **社会学应用：性伴侣平均数悖论** > 建立一个**二分图 (Bipartite Graph)**。由于每一条边都连接一个男性和一个女性，两性的总度数必然相等。  
> $\text{Avg}_m \times |V_m| = \text{Avg}_w \times |V_w|$。  
> **结论：** 除非人口比例失调，否则平均数的差异在数学上是不可能的。



### 2. 图着色与冲突解决 (Graph Coloring)
**核心指标：** 色数 $\chi(G)$ —— 合法着色所需的最小颜色数。

* **$d+1$ 定理：** 如果图的最大度数为 $d$，则该图一定可以用 $d+1$ 种颜色着色。
* **贪心算法：** 按照特定顺序着色，虽不一定得到 $\chi(G)$，但能保证上界。

### ⚠️ 易混淆点：General Coloring vs. Four Color Theorem

- **General Graph (Lec 6):** - 关注 $d+1$。只要你的度数足够高，颜色可以无限增加。
  - 例子：一个 5 个点且两两相连的图,（$K_5$）,最大度数 $d=4$，需要 5 种颜色。
  
- **Planar Graph (Four Color Theorem):**
  - 关注“平面性”。上述的 $K_5$ 在平面上是画不出来的（边一定会交叉）。
  - 只要边不交叉，数学家证明了你永远只需要 4 种颜色。

### 💡 深度思考：上限 (Upper Bound) 的意义

在 Lec 6 中，教授给出的 $d+1$ 是一个 **Upper Bound**。
- **定理含义**：$\chi(G) \le \Delta(G) + 1$。
- **直观理解**：这就像是你去装修，预算员告诉你“最多花 4 万”。最后你通过精打细算只花了 3 万（即 $\chi(G)=3$），这并不代表预算员算错了，而是说明你的方案优于最差情况。

**为什么研究上限？**
因为求 **$\chi(G)$ (精确最小值)** 在计算机科学里是 **NP-Hard** 问题（极难算）；而求 **$d+1$ (保底上限)** 只需要看一眼度数就能算出来。在快速决策（比如 HEOR 里的紧急资源调度）中，上限比最优解更有用。  
**HEOR 联想：**
在医院资源建模中，如果任务冲突是“线性的”（时间轴），它往往接近平面图逻辑；但如果涉及到复杂的“多重交叉感染路径”，它就变成了“一般图”，此时必须用 $d+1$ 的策略来准备资源。

## 🏛️ 第三部分：形式化证明 (Formal Proofs)

### Prove: $d+1$ , 着色定理的归纳法推导
**Proof by Induction on $n$:**
1.  **Base Case ($n=1$):** 只有一个点，<!-- TODO: 公式渲染异常，疑似 $\text{deg}(v)=0$ 不支持 --> <img width="192" height="68" alt="25ed2a20-807e-4bcd-aa2b-3a77692411cd" src="https://github.com/user-attachments/assets/fc57f1ae-9a2a-4773-a310-28258188ce78" />
，可以用 $0+1=1$ 种颜色，成立。
2.  **Inductive Step:**
    - 假设结论对 $n$ 个节点的图成立。
    - 考虑 $n+1$ 个节点的图，移除一个点 $v$。
    - 剩余子图已按假设完成着色。
    - 将 $v$ 放回 $v$ 最多有 $d$ 个邻居，在 $d+1$ 种可选颜色中，**至少存在一种颜色**未被邻居占用。
    - $\therefore$ 结论对 $n+1$ 成立。
<img width="1432" height="906" alt="681127f7-641f-4253-afa2-a78f55965e24" src="https://github.com/user-attachments/assets/f48b14bd-87d7-4bb0-bf4e-48952fdb6882" />


## 🧬 第四部分：跨学科建模思维 (Case Studies)

### 1. 《亚人》中的节点聚类 (Sato's Connectivity)
佐藤（Sato）的天才之处在于将 **Disconnected Graph** 转化为 **Connected Components**。
* **原子化防御：** 初始状态下 $E = \emptyset$，政府无法通过 BFS（广度优先搜索）进行追踪。
* **信号诱导：** 佐藤通过广播建立 **Hub Node**，诱导隐藏节点主动请求建立边 (Request an Edge)。
* **风险点：** 连通性虽然赋予了群体武力，但也让系统产生了“中心节点脆弱性”。

### 2. HEOR 罕见病建模 (Rare Disease Iceberg)
为什么罕见病患者难以寻找？
* **标签错误：** 节点属性被误诊（Misclassification），导致在图数据库中被过滤。
* **激励不兼容：** 当 $\text{Benefit} < \text{Cost}_{\text{stigma}}$ 时，节点倾向于断开所有外部连线（保持原子化）。
* **解决方案：** 建立中心化的 **Registry Hub**（类似于佐藤的信号塔），但通过健康激励（新药/医保覆盖）来降低连接成本。



---

## 📝 待办与思考 (To-Do)
- [ ] 深入理解 **The Pulverizer**（欧几里得算法）在计算乘法逆元中的应用。
- [ ] 思考：在神户大学的研究中，如何利用“图的直径”来衡量医疗信息传递的延迟？
- [ ] 复习：强归纳法与普通归纳法在处理“拆积木游戏”时的逻辑差异。

---
> **"Mathematics is the logic of certainty; Graph theory is the architecture of relationships."**
