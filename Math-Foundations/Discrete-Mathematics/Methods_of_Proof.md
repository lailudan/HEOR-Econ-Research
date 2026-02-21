
### 🗓 1/25 Mathematics for Computer Science & Linear Algebra （正序笔记）
> **Progress**: Started MIT 6.042J (Lec 1) and mastered the visual derivation of Linear Transformations.


#### 1. Logic & Proofs (MIT 6.042J Lec 1)
* **What is a Proof?**: A verification of a **Proposition** through a sequence of logical deductions starting from **Axioms**.
* **The "Induction" Trap**: Proving a case for $n=1, 2, ... 40$ does not constitute a proof for all $n$. Mathematics requires absolute logical necessity, not just patterns.
* **Gödel’s Incompleteness**: No set of axioms is both **Consistent** (no contradictions) and **Complete** (can prove everything). There will always be true statements that are unprovable.


### Lec 1: 证明、猜想与逻辑的边界

**1. 数学真理的绝对性**
- 法律真理靠辩论，科学真理靠实验，数学真理靠逻辑。
- 在逻辑面前，没有等级之分，只有证明的严密性。

**2. 著名的逻辑挑战**
- **四色定理 (Four Color Theorem)：** 第一个由计算机辅助证明的定理。它告诉我们，复杂系统的冲突（着色）存在理论上限，同时也引发了关于“人脑无法验证的证明是否可靠”的信任博弈。
- **哥德巴赫猜想 (Goldbach's Conjecture)：** “任一大于2的偶数都可写成两个质数之和”。极其简单的表述，却拥有极其复杂的底层逻辑。它展示了数学中“显而易见”与“难以证明”之间的鸿沟。
- **黎曼假设 (Riemann Hypothesis)：** 关乎素数分布的终极奥秘。莱顿教授用它说明，有些命题即使我们直觉上认为它是真的，但在没有逻辑闭环（证明）之前，它永远只能是猜想。

**3. 个人思考 (Personal Insight)**
- **识别恶意与反例：** 就像数学家寻找黎曼假设的反例一样，我的“直接反击”和“深度追问”是在寻找社会博弈中的“逻辑断裂点”。
- **Hidden Agenda：** 哥德巴赫猜想提醒我，表面简单的现象背后可能隐藏着极深层的机制。作为研究者，我不能满足于“看起来是真的”，必须追求“证明它是真的”。
- **决策止损：** 面对像黎曼假设这样耗费无数天才精力的难题，我也学到了在博弈中何时应用“秘书理论”进行止损——在不确定性中寻找那个最稳健的满意解。

**4. 真值表 (Truth Table) —— 逻辑的现形镜**
- **定义：** 穷举所有命题组合的真假情况，验证复杂逻辑项的最终值。
- **实战应用：** - 拆解“如果...那么...”的诱导性承诺。
    - 识别逻辑断裂点：如果前提为真但结论为假，则该逻辑路径必为伪。
    - 离散数学里的核心：与 (AND)、或 (OR)、非 (NOT)
      与(AND)： 必须两个都是真的，结果才是真。（就像婚姻，必须两个人都忠诚才叫忠诚）。
      或 (OR)： 只要有一个是真的，结果就是真。（就像逃生出口，左边或右边开了都能活）。
      非 (NOT)： 把真相倒过来。（骗子最擅长的，指鹿为马）。
- **感悟：** 真值表让我明白，反诈不需要读心术，只需要把对方的陈述代入真值表进行“一致性检测”。

**5. 逻辑陷阱：空虚真理 (Vacuously True)**
- **骗子诡计：** 利用 $P \to Q$ 在前提为假时恒为真的特性，诱导受害者。
- **深刻领悟：** “只有投了才证明是假的”是骗子设下的成本陷阱。
- **应对策略：** - 利用**逆否命题 ($\neg Q \to \neg P$)**：观察负面结果来反推前提的虚假，实现零成本证伪。
    - **逻辑高压：** 通过追问“解释解释”，在不支付成本的前提下，强行检测对方逻辑链的连通性。

**6. 逻辑三部曲：从诱饵到神话**
- **$p \Rightarrow q$ (蕴含)：** 骗子的诱饵。利用“未证实即为真”的灰色地带。
- **$q \Rightarrow p$ (逆命题)：** 幸存者偏差。看到别人赚钱 ($q$) 就以为前提 ($p$) 正确，这是严重的逻辑误判。
- **$p \iff q$ (充要条件)：** 封闭的神话系统。要求 $p$ 和 $q$ 步调绝对一致。
- **感悟：** 当我问“你再给我解释解释”时，我是在强行把对方从模糊的 $p \Rightarrow q$ 拉入严苛的 $p \iff q$ 检验中。只要发现一步对不上，他的逻辑矩阵就全线飘红 (F)。

**7. 逻辑系统的终极博弈：一致性 vs 完备性**
- **一致性 (Consistency)：** 系统内部不矛盾。这是我识破谎言的基石——只要对方“打脸”，逻辑即刻失效。
- **完备性 (Completeness)：** 能够解释所有问题。
- **感悟：** 哥德尔告诉我们，一个绝对自洽的系统必然有其解释不了的盲区。这意味着我不需要成为“全知全能”的专家，但我必须做一个“逻辑一致”的智者。
- **实战：** 面对那些号称能解释一切（完备）的理财大师，我要警惕其内部可能隐藏的巨大不一致性。

**8. 逆命题的陷阱：严防“倒果为因”**
- **核心禁忌：** $p \Rightarrow q$ 成立，不代表 $q \Rightarrow p$ 成立。
- **生活实例：** - “顶级大帅哥有人追” 是真命题。
    - “有人追就是顶级大帅哥” 是伪命题（可能是因为他有钱或有手段）。
- **反诈警示：** 看到“结果 ($q$)”是真的，不代表“原因 ($p$)”就是真的。骗子常展示虚假结果来伪造不存在的原因。

**9. 逻辑术语对齐：充分 vs 必要**
- **充分条件 ($p \Rightarrow q$)：** “有之必然”。
  - 例子：考上博导是拿到学位的充分条件。
- **必要条件 ($q \Rightarrow p$)：** “无之必不然”。
  - 例子：呼吸是活着的必要条件。
- **充要条件 ($p \iff q$)：** “有之必然，无之必不然”。
  - 例子：在逻辑上，真正的诚实是言行的一致性。

**10. 深度理解：为什么 (F, F) 结果为 T？**
- **核心逻辑：** 真值表测量的不是 $p$ 或 $q$ 的好坏，而是整个“逻辑规则”是否被破坏。
- **例子：** “考上大学 ($q$) 必须先参加高考 ($p$)”。
  - 如果你没参加高考 ($p$ 为 F)，也没考上大学 ($q$ 为 F)，这完全符合规则。
  - 因为规则没被破坏，所以这个逻辑命题本身是 **真 (T)**。
- **感悟：** 骗子经常利用这种“规则没被破坏”的灰色地带（空虚真理）来维持其话术的表面自洽。

**11. 实战分析：人格独立的逻辑公式**
- **素材：** “只要希望被理解，人格就不独立。”
- **逻辑模型：** 充要条件 ($p \iff q$)。
  - $p$: 渴望理解
  - $q$: 人格不独立
- **核心感悟：** 这是一种“逻辑洁癖”。它认为“独立”与“渴望”是互斥的。如果你想在系统里保留“独立”这个属性，你必须在真值表里把所有 $p$ 为真的路径全部切断 (Cut)。
- **连接点：** 这和我“直接反击”陌生人的本能一致——我不求你理解我的反击，我只负责维护我逻辑的一致性。

**12. 警惕“互斥陷阱”：独立 vs. 渴望**
- **逻辑误区：** 将“人格独立”与“情感需求”设为互斥事件 ($A \cap B = \emptyset$)。
- **恶毒之处：** 这种逻辑抹杀了人的生物性，通过极端的定义来剥夺个体的自我认同。
- **正确建模：** 独立是一种**决策权**。我可以有渴望，但在真值表最终输出决策时，我的渴望不占据主导地位。
- **反思：** 别让别人用“你不够独立”这种逻辑废话来拿捏你。

**13. 认知日志：拥抱“似懂非懂”**
- **状态：** 逻辑术语尚未完全内化，处于“模糊匹配”阶段。
- **哲学对齐：** 哥德尔告诉我们系统是不完备的，认知亦然。
- **策略：** 不死磕每一个公式，重点抓取“逻辑防御”的直觉。
- **待办：** 在实际观察社会骗局时，反复调用“必要条件”和“充分条件”的模板进行比对。



### 🗓 1/28 Discrete Math: The "Fake Statue" Breakthrough
> **Logic**: Mathematical Induction & Recursion.

#### 1. The "Pseudo-Statue" Strategy (Ludan's Insight)
* **Problem**: A $4 \times 4$ grid has only one real statue, but we need every $2 \times 2$ quadrant to have a "hole" to be solvable.
* **Solution**: Place one L-shaped tile at the very center.
* **The Magic**: The three corners of this center tile act as **"Artificial Statues"** for the other three quadrants.
* **Result**: Now every quadrant has exactly one hole (either real or artificial). We can now tile the rest perfectly.

* **Cognitive Milestone**: Spent 45 mins in "Productive Struggle." Independently derived the concept of "Artificial Statues" for recursive tiling. Realized that understanding the structural logic is 10x more valuable than merely following the video timeline.

#### 2. Mathematical takeaway
* **Induction isn't magic**: It's about finding a way to make the "next step" ($N+1$) look exactly like the "previous step" ($N$) by clever structuring.


### 🗓 1/27 Discrete Math: The Art of Contradiction
> **Source**: MIT 6.042J Lec 2 by Tom Leighton.

#### 1. Logic Strategy: Proof by Contradiction
* **Method**: To prove $P$, assume $\neg P$ (Not $P$) and show it leads to a logical disaster.
* **Famous Proof**: $\sqrt{2}$ is irrational. 
    * If $\sqrt{2} = a/b$ (in lowest terms), then both $a$ and $b$ must be even.
    * But if both are even, the fraction wasn't in lowest terms $\rightarrow$ **CONTRADICTION**.

#### 2. Why it matters for HEOR/Economics
* **Model Validation**: If assuming a policy has "zero effect" leads to predictions that contradict observed market reality, the policy MUST have an effect.


#### 3. 归纳法 (Induction) - 22min **
- **概念：** 建立一种“传递性”的真理。

**归纳法的本质 (Mathematical Induction)**
- **$P(0)$ 为真** + **$P(n) \Rightarrow P(n+1)$ 为真** = **所有 $P(n)$ 均为真**。
- 逻辑锚点：归纳法不需要穷举无限，它只需要证明“传递性”。

**逻辑漏洞识别：伪归纳与循环论证**
- **伪归纳 (False Induction)：** 警惕“传递性”失效。
  - 案例：马的颜色证明。
  - 核心：必须检查从 $n$ 到 $n+1$ 的每一个微观步骤，尤其是起步阶段。
- **循环论证 (Circular Reasoning)：** 逻辑的“原地踏步”。
  - 特征：结论本身被藏在了前提里。
  - 识别：如果对方解释了半天，只是在不断重复同一个意思，说明逻辑链条没有向外延伸，是无效证明。
- **感悟：** 真正的逻辑必须是“向外生长”的，必须从一个坚实的、独立的**前置条件**推导出来。

- **逻辑断裂：消失的交集 (Empty Intersection)**
- **马的教训：** 归纳法的传递性依赖于“重叠”。
- **失效点：** 当规模缩小到 $n=2$ 时，前一组 $\{1\}$ 和后一组 $\{2\}$ 的交集为空。
- **反诈应用：** 警惕那些“看起来可以无限复制”的模式。
  - 问：从 $n=1$ 到 $n=2$ 的时候，支撑它们连通的“交集”是什么？
  - 如果交集为空，那它就不是归纳，而是纯粹的臆想。

**解决难题的逆向思维 (Stronger Induction)**
- 当目标 $P$ 难以达成时，尝试证明一个包含 $P$ 的更广义命题 $P'$。
- **博弈应用：** 在研究“失踪人口”或“经济模型”时，如果针对个案无法闭环，就去寻找整个系统（任意位置）的通解。

**4. 教授的“地砖哲学”**
- 建筑师（Frank Gehry）制造麻烦，数学家（Leighton）通过归纳法在混乱中寻找秩序。
- **感悟：** 逻辑不仅是防御，更是解决复杂工程问题的“构造蓝图”。


















### 🗓 1/31 Discrete Math: 不变量原理 (Invariant) 与 强归纳法 (Strong Induction)

**课程状态：** 已完成 Lec 3 核心逻辑梳理  
**核心关键词：** 状态机 (State Machines)、不变量 (Invariants)、强归纳 (Strong Induction)

---

## 1. 逻辑质量：为什么“看起来对”的证明是危险的？
在进入复杂推导前，Leighton 教授强调了证明的**鲁棒性 (Robustness)**。

* **Airbus A300 坠机案例：** 逻辑系统中的一个微小 Gap（间隙），在特定输入下会导致整个物理系统崩溃。
* **倒置逻辑陷阱 (Backward Reasoning)：** * **错误示例：** 假设 $1 = -1$ $\implies$ $1^2 = (-1)^2$ $\implies$ $1 = 1$ (True)。
    * **本质谬误：** 从命题 $P$ 推出一个真命题，并不代表 $P$ 本身是真的。
    * **博弈启示：** 骗子最喜欢从“结果（发财了）”反推“前提（项目是真的）”。

---

## 2. 核心武器：不变量原理 (The Invariant Principle)
这是处理**状态机 (State Machine)** 问题的终极武器。它用来解决：**“一个目标状态是否可达？”**

### A. 数学定义
对于一个系统：
1.  **起始状态：** $S_0$。
2.  **不变量 (Invariant)：** 一个性质 $P$。
3.  **判定规则：** 如果 $P(S_0)$ 为真，且对于任何一次合法操作（从状态 $S$ 转移到 $S'$），都有 $P(S) \implies P(S')$，那么 $P$ 对所有从初始状态出发的可达状态都为真。

### B. 实战：8-Puzzle (数字华容道) 的逻辑死锁
教授展示了一个挑战：将 $\{G, H\}$ 两个字母互换位置。



* **逻辑工具：逆序对 (Inversions)**
    * 如果字典序大的字母排在小的字母前面，计为 1 个逆序对。
* **操作对逻辑的影响：**
    * **左右滑动：** 字母的相对顺序完全没变，逆序对数量变化为 $0$。
    * **上下滑动：** 一个字母会跳过它前面或后面的 $2$ 个字母。这会导致逆序对的数量改变 $+2, -2$ 或 $0$。
* **核心不变量：奇偶性 (Parity)**
    * 逆序对总数的**奇偶性**在每次移动后保持不变。
* **结论：** 目标状态（$\{G, H\}$ 互换）会导致逆序对总数从奇数变偶数（或反之）。由于奇偶性是锁死的不变量，因此**该目标在逻辑上永远不可达**。

---

## 3. 武器升级：强归纳法 (Strong Induction)
当 $P(n+1)$ 的证明不仅依赖前一步 $P(n)$，而是需要依赖前面**所有**步骤 $\{P(0), P(1), \dots, P(n)\}$ 时使用。

### A. 模板对比
* **普通归纳：** $P(n) \implies P(n+1)$。
* **强归纳：** $\forall k \in [0, n], P(k) \implies P(n+1)$。
* **直觉理解：** 普通归纳是推骨牌；强归纳是爬楼梯，你可以踩着下面所有的横木。

### B. 案例：拆积木游戏 (Unstacking Game)
* **规则：** $n$ 块积木，每次拆成两堆 $a$ 和 $b$，得分 $a \times b$。
* **目标：** 证明无论怎么拆，最后总分都是 $\frac{n(n-1)}{2}$。
* **强归纳证明要点：**
    * 假设对于所有规模小于 $k$ 的堆，公式都成立。
    * 将 $k+1$ 拆成 $a$ 和 $b$。
    * 总分 = $ab + \text{Score}(a) + \text{Score}(b)$。
    * 代入强归纳假设：$ab + \frac{a(a-1)}{2} + \frac{b(b-1)}{2}$。
    * 化简后完美符合 $\frac{(k+1)k}{2}$。
### 🧱 Formal Proof: The Unstacking Game Invariant

**Theorem:** For $n$ blocks, regardless of the splitting strategy, the total score is always $S_n = \frac{n(n-1)}{2}$.

**Proof by Strong Induction:**

1. **Base Case ($n=1$):**
   A single block cannot be split. Total score is $0$.
   Formula: $\frac{1(1-1)}{2} = 0$. (True)

2. **Inductive Hypothesis:**
   Assume that for all $1 \le k \le n$, the total score for unstacking $k$ blocks is $P(k) = \frac{k(k-1)}{2}$.

3. **Inductive Step:**
   Consider $n+1$ blocks. Suppose the first split divides the stack into two piles of size $a$ and $b$, where $a + b = n + 1$ and $a, b \ge 1$.
   The total score $S_{n+1}$ is the sum of the current split score plus the scores of unstacking the two resulting piles:
   $$S_{n+1} = (a \cdot b) + P(a) + P(b)$$
   
   Substituting the inductive hypothesis:
   $$S_{n+1} = ab + \frac{a(a-1)}{2} + \frac{b(b-1)}{2}$$
   $$S_{n+1} = \frac{2ab + a^2 - a + b^2 - b}{2}$$
   $$S_{n+1} = \frac{(a+b)^2 - (a+b)}{2}$$
   
   Since $a+b = n+1$:
   $$S_{n+1} = \frac{(n+1)^2 - (n+1)}{2} = \frac{(n+1)n}{2}$$

**Conclusion:**
The formula holds for $n+1$. By the principle of Strong Induction, the total score is an **invariant** based solely on the number of blocks. $\square$


---

## 4. 跨学科思考 (Architecture & Economics)
* **结构性限制：** 建筑师可以设计歪斜的楼，但数学家通过“不变量”在混乱中寻找秩序。
* **教材坐标系：** 高斯 (Gauss) 的漏洞告诉我们，不要迷信“显而易见”。如果一个向量空间看上去是线性无关的，必须通过严谨的判定基准（如不变量）来验证。
* **经济学博弈：** 在分析金融数据时，寻找那个“不变量”（如：零和博弈中的总额）。如果一个模型承诺的结果打破了不变量，则该模型必然存在欺骗。


> **"If you can't prove $P$, try to prove something stronger."** > —— Tom Leighton, MIT 6.042J

# 🧩 Formal Proof: Infeasibility of the 8-Puzzle State Transition

## 1. Mathematical Definitions

* **State ($S$):** A specific configuration of the tiles $\{A, B, \dots, H\}$ and the empty square in the $3 \times 3$ grid.
* **Inversion:** A pair of tiles $(L_i, L_j)$ is called an **inversion** if $L_i$ precedes $L_j$ in the alphabetical order, but $L_j$ appears before $L_i$ in the grid (when scanning row-by-row, left-to-right).
* **Inversion Number ($N$):** The total count of inversions in a given state (the empty square is ignored in this count).
* **Parity:** The property of an integer being even or odd ($N \pmod 2$).

---

## 2. The Invariant Principle

**Claim:** The **parity** of the inversion number $N$ is an **invariant** under any legal move in the 8-puzzle.

### 2.1 Case Analysis of Moves
A legal move consists of sliding a tile into the empty square. This is equivalent to moving the empty square **Left, Right, Up, or Down**.

#### **Case 1: Horizontal Moves (Left/Right)**
When the empty square moves left or right, the relative order of the tiles in a row-major scan remains identical.
$$\Delta N = 0$$
The parity is unchanged.

#### **Case 2: Vertical Moves (Up/Down)**
When the empty square moves up or down, a tile (let's call it $T$) "jumps" over exactly two other tiles ($L_1$ and $L_2$).
* If $T$ was in an inversion with both $L_1$ and $L_2$, $N$ decreases by 2.
* If $T$ was in an inversion with neither, $N$ increases by 2.
* If $T$ was in an inversion with only one of them, $N$ stays the same ($+1 -1 = 0$).

In all sub-cases, the change in the inversion number is:
$$\Delta N \in \{+2, -2, 0\}$$

Since $\Delta N$ is always an **even number**, the parity of $N$ remains constant:
$$N_{new} \equiv N_{old} \pmod 2$$



---

## 3. Proof by Contradiction

To prove that a target state (e.g., swapping tiles G and H) is unreachable from the start state:

1.  **Initial Parity:** Calculate $N_{start}$. Suppose $N_{start} \equiv 1 \pmod 2$ (Odd).
2.  **Target Parity:** Calculate $M_{target}$ for the desired state. For a single swap of adjacent tiles like G and H, the parity will change, so $M_{target} \equiv 0 \pmod 2$ (Even).
3.  **Contradiction:** Because the parity of the inversion number is an invariant, any state reachable from $S_{start}$ must have an **odd** inversion number. 
4.  **Conclusion:** Since the target state has an **even** inversion number, it exists outside the reachable state space of the system.

$$\therefore S_{target} \text{ is unreachable from } S_{start}. \quad \square$$

---

## 4. Key Takeaway for System Analysis
In any state-machine system, identifying an **Invariant** allows one to define the boundaries of what is possible. If the "Genetic Code" (Parity) of your current state does not match the "Genetic Code" of your goal, no amount of computation or effort will bridge the gap.

### 🧠 Case Study: Breaking the Invariant
**Question:** Does adding an extra external slot make the 8-puzzle solvable?
**Answer:** Yes.
**Logic:**
1. The standard $3 \times 3$ grid is a **Closed System** with a fixed parity invariant.
2. An external slot transforms the system into an **Open System**.
3. It allows for a **single swap (transposition)**, which changes the parity of the inversion number from $n$ to $n \pm 1$.
4. **Key Takeaway:** If a logical problem is "unsolvable," look for a way to change the **Domain (Definition)** of the problem.
