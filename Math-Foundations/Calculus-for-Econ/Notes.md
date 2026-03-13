

# Study Notes: The Structuralist Reconstruction of Calculus （正序笔记）
**Timeline:** Jan 20, 2026  
**Theme:** Deconstructing "Analytical" Rote Learning through Systemic Modeling  
**Target:** Kobe University PhD Pipeline (GSICS-Economics)

---

## 1. Philosophical Shift: From "Points" to "Systems"
> **Core Insight:** I am not "bad at math"; I am a **Structuralist**. Traditional education fails by isolating particles, whereas my brain excels at identifying **Networks** and **Equilibria** (Architecture, Gas Laws, Biochemistry).

* **The Strategy**: Treat math as a language of **rhythm**. Understanding the rhythm of a wave or the balance of a chemical reaction is the key to understanding the logic of a derivative.
* **Filtering Noise**: In both Architecture and Economics, we focus on the "dynamic" by filtering out the "static" (e.g., the Constant Rule where the derivative of a fixed cost is zero).

---

## 2. The Ecological Model of Calculus (Dinosaur Logic)
To clarify terminology in any system (Economics or Biology), we use the **Dinosaur Extinction Model**:

| Concept | Mathematical Symbol | Structuralist Definition |
| :--- | :---: | :--- |
| **Derivative** | $f'(x)$ | The **Pulse/Speed** of extinction at a specific second. It answers: *"How fast are we losing them right now?"* |
| **Differential** | $dx, dy$ | The **Instantaneous Slice**. The actual number of dinosaurs that died in that micro-moment. |
| **Definite Integral** | $\int_{a}^{b} f(x) dx$ | **The "Body Count."** Summing up every tiny death slice over a period to find the total loss. |
| **Indefinite Integral** | $\int f(x) dx$ | **The "Reverse Engineering."** Finding the original population model $+C$ (the unknown constant). |

---

## 3. The Logic of "Shortcuts" (Logical Macros)
Rules of differentiation are not magic spells; they are systemic observations.

* **The Product Rule (Geometric Expansion)**: $(uv)' = u'v + uv'$. Think of **Revenue** ($Price \times Quantity$). If both change, you must account for growth in both directions to avoid missing the "corners" of the expansion.
* **The Chain Rule (The Causal Gear Train)**: $\frac{dy}{dx} = \frac{dy}{du} \cdot \frac{du}{dx}$. The total impact of an "Effort" on "Revenue" is the product of the transmission ratios (gears) at each step of the causal chain.

---

## 4. Advanced Economic Applications: Optimization & Elasticity
> **PhD Insight:** Economic equilibrium occurs when Marginal Cost equals Marginal Revenue ($f'(x) = g'(x)$).

* **The First Derivative Test ($f'=0$)**: Finding the "Sweet Spot" where profit is maximized or pain is minimized (the moment the pulse of change stops).
* **Elasticity (System Sensitivity)**: Moving beyond the slope to measure how sensitive a system is. If medication dosage (YOPD treatment) increases by 1%, how much does motor function "bounce back"?
* **The Gradient Vector ($\nabla f$)**: The "Vector of steepest ascent." This is the bridge where the **Parametric Vector** ($\vec{x} = \vec{a} + t\vec{v}$) meets Calculus to point the way toward system improvement.

---

## 5. High-Order Signals & Structural Breaks
Higher-order derivatives serve as "Pre-alarm" systems for researchers.

* **Second Derivative ($f''$)**: Measures the **Acceleration** of change. It tells us if an extinction or a market move is slowing down or spiraling into an exponential bubble.
* **Inflection Points (拐点)**: Identifying "Structural Breaks," such as the moment a 60-year-old’s physical decline changes its "rhythm" or direction.

---

## 📈 Current Progress & Synthesis
* **Wave Advantage**: Proficiency in Wave physics allows for **Frequency Domain Thinking**, essential for understanding cyclical Business Cycles (Boom/Bust).
* **Linear Algebra Bridge**: Transitioning from the **"Individual Dinosaur"** (Calculus) to the **"Dinosaur Legion"** (Linear Algebra/Matrices).
* **Self-Regulation**: Recognizing that the "40-minute mental overheat" is the sound of structural brain re-wiring.

---
*Log generated for the "Master-to-PhD Pipeline" 2026. Kobe University.*



# Updated: Jan 24, 2026 
## 🔍 Deep Dive: Unbounded vs. DNE
- **DNE (General)**: The total failure of convergence. Left neighbor $\neq$ Right neighbor.
- **Unbounded ($\infty$)**: A "disciplined" failure. Neighbors agree to explode together. 
- **PhD Insight**: In Economic modeling, $\infty$ signals a "bubble" or "systemic divergence," while a general DNE signals a "structural jump" or "chaotic noise."






---





# Updated: Jan 26, 2026 
# 🎓 Study Notes: The Big Picture of Calculus
**Source:** MIT Gilbert Strang - "Big Picture of Calculus"  
**Mission:** 建立“函数对”的直觉，理解微积分作为“变化”与“累积”互逆关系的本质。

---

## 1. 核心定义：微积分是关于“函数对”的关系
> **Core Insight:** 微积分的核心不是计算，而是研究两个函数（Function 1 & Function 2）之间的联动。

| 函数类型 | 物理含义 (Example) | 几何含义 | 数学符号 |
| :--- | :--- | :--- | :--- |
| **Function 1 (Distance/Height)** | **总量/位置**：如行驶的里程、山峰的高度。 | **位置/高度** | $y(x)$ 或 $f(t)$ |
| **Function 2 (Speed/Slope)** | **变化率**：如行车的速度、攀爬的陡峭程度。 | **斜率 (Slope)** | $\frac{df}{dt}$ 或 $\frac{dy}{dx}$ |

---

## 2. 两大支柱：微分与积分的对称性
微积分的任务就是在这两个黑盒之间建立双向通道：

* **微分学 (Differential Calculus):** 从“函数 1”推导出“函数 2”。
    * *逻辑：* 已知距离 $f(t)$，求出那一瞬间的速度 $\frac{df}{dt}$。
* **积分学 (Integral Calculus):** 从“函数 2”还原回“函数 1”。
    * *逻辑：* 已知速度 $s(t)$，通过“累加”还原出总里程。

---

## 3. 三大核心动态模型分析

### A. 恒定状态 (Constant Case)
* **速度 (Function 2):** 是一条平水平线（例如 40 mph）。
* **距离 (Function 1):** 是一条斜率为 40 的直线（$f = s \cdot t$）。
* **关键公式:** $\text{Speed} = \frac{\Delta f}{\Delta t}$ (距离变化量 / 时间变化量)。

### B. 负向变动 (Negative Speed & Reverse)
* **观察:** 当距离图像开始下降时，意味着物体在倒车或高度下降。
* **信号:** 此时**速度为负值**。
* **文化梗:** 正如《Ferris Bueller's Day Off》（春天不是读书天）里的倒车逻辑：如果里程表能根据微积分原理运作，倒车时里程数应该减少。

### C. 恒定加速度与面积奇迹 (The Area Connection)
* **速度:** 呈线性增长（$s = a \cdot t$），图像是一个三角形。
* **距离:** 呈二次方增长（$f = \frac{1}{2}at^2$），图像是一个**抛物线**。
* **重大发现:** 函数 1 的数值精确等于函数 2 图像下方的**面积**。
    * *案例：* 速度三角形的面积 ($\frac{1}{2} \times \text{Base} \times \text{Height}$) 正好就是距离函数。



---

## 4. Cross-Disciplinary Synthesis
* **结构化思考:** 将微积分看作“数据累积（积分）”与“趋势探测（微分）”的统一。
* **研究应用:** 在神户大学的经济模型中，资产总额是“财富（Function 1）”，而储蓄率/消费率则是“速度（Function 2）”。
* **系统洞察:** 无论是在物理、生物还是经济中，微积分都在处理这种“瞬时率”与“运行总额”之间的转化。

---

## 📈 Progress Tracking
* **New Concept:** 深刻理解了 Leibniz 符号 $\frac{df}{dt}$ 的本质是 $\frac{\Delta f}{\Delta t}$ 的极限形式。
* **Mathematical Confidence:** 确认了“求导（寻找斜率）”与“积分（寻找面积）”是互逆的操作。
* **Next Step:** 准备进入 **Linear Algebra**，探索如何用矩阵一次性管理成千上万个这类“函数对”。

## ⚖️ The Two Directions of Calculus
> Mastering the "Slicing" and "Stitching" logic.

1. **The Slicer (Differentiation)**:  
   - $f \xrightarrow{\text{Slope}} s$  
   - $s = \frac{df}{dt}$  
   - *Logic:* How steep is the growth? (Finding the Pulse).

2. **The Stitcher (Integration)**:  
   - $s \xrightarrow{\text{Area}} f$  
   - $f = \int s \, dt$  
   - *Logic:* How much has accumulated? (Finding the Total).

* **Final Verdict**: Calculus is a closed loop. Integration builds the mountain; Differentiation measures its slope.
  
## ⚖️ The Commander's Formula: Rate vs. Quantity
> Differentiation probes the pulse; Integration builds the body.

* **Differentiation ($\frac{df}{dt}$)**: 
    - **Focus**: The **"Speed" (速)** of change.
    - **Logic**: Slicing the Total to find the Rhythm.
* **Integration ($\int s \, dt$)**: 
    - **Focus**: The **"Quantity" (量)** of accumulation.
    - **Logic**: Stitching the Rhythm (Area) to find the Total.

**Insight**: My "Structuralist" brain excels here because I see the system's balance. I don't calculate points; I manage flows.


# Updated: Jan 28, 2026
# 🔍 Study Notes: The Logic of One-Sided Limits
<img width="1086" height="1114" alt="Weixin Image_20260128153446_183_11" src="https://github.com/user-attachments/assets/620222b2-70ea-4a04-876a-e0561f8545c6" />


**Context:** 理解为什么在“跳跃点”，单侧极限可以存在而整体极限不存在。

## 🕵️ The "Paparazzi" Rule of Limits
> Limits are like paparazzi: they only care about who you're hanging out with (neighbors), not who you actually are (the point).

- **Ignore the Point**: The actual value $f(c)$ (solid dot) is IRRELEVANT to the limit.
- **Focus on the Trend**: Look at the "Super Neighbors" (infinitesimally close).
- **Jump Discontinuity**: 
    - Left neighbors say "We are going to 5".
    - Right neighbors say "We are going to 1".
    - Result: Individual side limits exist, but they don't agree.

## 1. 核心定义：单侧极限 (One-Sided Limits)
> **Structural Insight:** 只要单方面有明确的目标，极限就是“存在的”。

在你的示例图中，函数在 $x=2$ 处裂开了。数学家使用特殊的符号来描述这种“单向奔赴”：

* **左极限 (Left-hand Limit):** $\lim_{x \to 2^-} f(x) = 5$
    - **逻辑：** 只看 $x=2$ 左边的邻居。当 $x$ 从 $1.9, 1.99 \dots$ 靠近时，高度趋向于 **5**。
* **右极限 (Right-hand Limit):** $\lim_{x \to 2^+} f(x) = 1$
    - **逻辑：** 只看 $x=2$ 右边的邻居。当 $x$ 从 $2.1, 2.01 \dots$ 靠近时，高度趋向于 **1**。



---

## 2. 为什么“整体极限”会不存在 (DNE)？
整体极限 $\lim_{x \to 2} f(x)$ 要求左右邻居达成“共识”。

* **判定法则：** 只有当 **左极限 = 右极限** 时，整体极限才存在。
* **本例结论：** 因为 $5 \neq 1$，所以左右邻居在这里“闹掰了”。
* **术语：** 这种情况称为 **跳跃间断 (Jump Discontinuity)**。

---

## 3. 跨学科直觉：经济学中的“冲击 (Shock)”
在即将研究的 **GSICS-Economics (神户大学)** 领域中，这种图非常有用：

* **政策突变：** 假设 $x=2$ 是政策颁布的时刻。
* **左极限：** 政策前市场的预期（趋向 5）。
* **右极限：** 政策后市场的瞬间反应（跳到了 1）。
* **结论：** 这种“不连续性”描述了系统在极端扰动下的瞬态行为，而不是错误。

### 🧠 The "Neighbor Consensus" Rule
- **Single-Side**: Neighbors on ONE side have a clear destination $\to$ **Limit Exists**.
- **Double-Side**: Neighbors from BOTH sides must meet at the same point $\to$ **Limit Exists**.
- **The Gap**: If Left $\neq$ Right, the system is "Broken" at that point (DNE).










# 🎓 Study Notes: The Big Picture of Derivatives
**Date:** Jan 30, 2026  
**Source:** MIT Gilbert Strang - "Big Picture: Derivatives"
**Mission:** 理解如何通过“切片”捕捉系统的瞬时脉搏。

---

## 1. 核心定义：从“平均”到“瞬时”
> **Structural Insight:** 平均速度不需要微积分（只需减法和除法），只有**瞬时速度**才需要导数。

* **函数 1 (总量/高度)**: 描述系统累积了多少。
* **函数 2 (导数/斜率)**: 描述系统在每一个瞬间的“跳动”规律。
* **导数的本质**: 它是寻找“函数 1”图像上某一点**切线 (Tangent Line)** 的斜率。

---

## 2. 三大基本“工具” (The Great Functions)
掌握这三个基础导数，就能构建起描述现实世界（科学、工程、经济）的绝大部分模型：

| 函数 $y = f(x)$ | 导数 $\frac{dy}{dx}$ | 结构化特征 |
| :--- | :--- | :--- |
| **幂函数 $x^n$** | $nx^{n-1}$ | 降幂法则：$x^2$ 的脉搏是 $2x$。 |
| **正弦 $\sin x$** | $\cos x$ | 循环美感：波的高度变化律是它的余弦。 |
| **指数 $e^x$** | $e^x$ | **奇迹函数**：函数值恰好等于它自己的斜率。 |



---

## 3. “切片”推导过程 (The "Slicing" Process)
教授以 $y = x^2$ 为例，演示了如何利用你的“无穷小”直觉算出导数：

1. **设定邻居**: 取一个距离为 $\Delta x$ 的超级近邻。
2. **计算变化率**: $\frac{\Delta y}{\Delta x} = \frac{(x + \Delta x)^2 - x^2}{\Delta x}$。
3. **代数简化**: 展开后得到 $2x + \Delta x$。
4. **极限一跳 ($\lim_{\Delta x \to 0}$)**: 当邻居近到“无穷小”时，$\Delta x$ 消失。
5. **最终结果**: 导数确认为 **$2x$**。

---

## 4. 特殊信号：斜率为 0 的时刻
* **最高点与最低点**: 当切线水平时，导数等于 **0**。
* **应用价值**: 识别系统的“底部”或“顶部”。在经济学中，这通常代表**最优解**（利润最大化或成本最低化）。



---

## 📈 Progress Tracking
* **New Concept**: 理解了导数公式不是“规定”，而是通过无穷小邻居推导出来的“趋势”。
* **PhD Readiness**: 准备好使用**链式法则 (Chain Rule)** 等工具来处理更复杂的跨学科经济模型。
* **Commander Insight**: 求导是“剥开”总量看节奏；积分是“缝合”节奏看总量。


## 🧭 Space Coordinate Translation (Radians)
- **$\pi$** = 180° (A Half Circle)
- **$\pi/2$** = 90° (Top of the Wave)
- **$2\pi$** = 360° (Full Cycle)

| Phase | Radians | Height ($\sin$) | Slope ($\cos$) |
| :--- | :--- | :--- | :--- |
| Start | $0$ | $0$ | $1$ (Steepest) |
| Peak | $\pi/2$ | $1$ | $0$ (Flat) |
| Mid | $\pi$ | $0$ | $-1$ (Steep Down) |


## 📏 Geometry Meets Calculus: The $2\pi$ Link
- **Radius = 1**: On a unit circle, distance = angle (in radians).
- **$360^\circ = 2\pi$**: The full journey around the circle.
- **$\pi / 2 = 90^\circ$**: The moment the wave reaches its peak (or the slope hits zero).
- **Conclusion**: We use radians because the math stays "pure"—the speed of the wave matches the geometry of the circle.




# 🗓 2/2 微积分笔记：导数的记号 (Derivative Notations)

> **核心逻辑**: 导数记号是表达“微分过程”的数学语言。三种主要记号代表了数学史上三大巨头的不同视角。

---

## 1. 三大流派对比表

| 记号名称 | 表达方式 | 读法 | 适用语境 | 建筑师/经济学家直觉 |
| :--- | :--- | :--- | :--- | :--- |
| **Lagrange (拉格朗日)** | $f'(x)$ 或 $y'$ | f prime | 最常用，最简洁。 | 像是一个**缩写**，一眼看出这是“原版的变体”。 |
| **Leibniz (莱布尼茨)** | $\frac{dy}{dx}$ 或 $\frac{d}{dx}f(x)$ | dy dx | 严谨、描述性强。 | 像是一张**详图**，明确标出谁随谁变。 |
| **Newton (牛顿)** | $\dot{y}$ | y dot | 物理学、力学。 | 像是一个**时钟**，专指随时间的变化。 |

---

## 2. 深度拆解

### 🟢 Lagrange's Notation (简洁派)
- **写法**: $f'(x)$
- **优势**: 在处理单变量函数时极快，不会让页面显得混乱。
- **局限**: 无法明确自变量。如果公式里有 $a, b, c$ 等多个字母，不知道是对谁求导。

### 🔵 Leibniz's Notation (严谨派)
- **写法**: $\frac{d}{dx}f(x)$
- **核心逻辑**: 
    - $\frac{d}{dx}$ 是一个**算子 (Operator)**，像是一个加工机器，你把表达式放进去，它吐出导数。
    - **Leibniz 为 PhD 建模而生**: 在复杂的经济模型中，你可以清晰地区分 $\frac{dy}{dt}$（随时间变化）和 $\frac{dy}{dp}$（随价格变化）。

### 🟡 Newton's Notation (物理派)
- **写法**: $\dot{y}$
- **PhD 关联**: 在研究动态系统（如 YOPD 患者随时间变化的步态轨迹数据）时，这种记号非常直观。

---

## 3. 🛠 逻辑纠偏：正确表达识别

在实际书写中，撇号（'）和算子（d/dx）的位置决定了逻辑是否通顺：

* **✅ 正确示例**: 
    * $g'(x)$
    * $\frac{d}{dx}g(x)$
    * $\frac{d}{dx}\sqrt{x}$
* **❌ 错误示例**: 
    * $\sqrt{x'}$ （撇号不能加在运算符号内部）

### 📐 Tangent Line Intuition (切线方程直觉)
* **Goal**: Find the equation of the line touching function $h$ at $x = -4$.
* **Components**:
  1. **Coordinate**: From $h(-4)=7$, we get $(x, y) = (-4, 7)$.
  2. **Slope ($m$)**: From $h'(-4)=1$, we get $m = 1$.
* **The "Magic" Formula**: Point-Slope Form is faster than $y=ax+b$.
  - Formula: $y - y_0 = m(x - x_0)$
  - Applied: $y - 7 = 1(x + 4)$ -> **Option D**.

## 💡 概念避坑：函数值 vs. 导数 (Height vs. Slope)

在处理切线方程 (Tangent Line) 时，必须区分两种不同的“数值”：

### 📍 1. 坐标锚点 (The Location)
- **表达**: $h(a) = b$
- **含义**: 当 $x = a$ 时，函数的高度是 $b$。
- **坑点**: 这里的 $b$ 只能放在 $y - b$ 的位置，**绝对不能**放在斜率的位置。

### 📐 2. 瞬间坡度 (The Direction)
- **表达**: $h'(a) = k$
- **含义**: 在 $x = a$ 这一点的切线斜坡陡度是 $k$。
- **坑点**: 这里的 $k$ 只能放在括号前面的系数位置，**绝对不能**减在 $y$ 后面。

### 🚀 快速组合示例

<img width="1452" height="1038" alt="90a7118ee2c6633633b4a1e8b3aecbd4" src="https://github.com/user-attachments/assets/5d390516-27d9-47ec-92bf-8072b8ae64d8" />



# 🗓 2/4 Calculus: The Epsilon-Delta Rigor
> **Motto**: Moving from "Intuition" to "Formal Proof".

### ⚖️ The Challenge-Response Game
1. **The Challenge ($\epsilon$)**: How close do you want the output $f(x)$ to be to $L$?
2. **The Response ($\delta$)**: How close must the input $x$ be to $c$ to guarantee that?

### 🧩 Formal Definition
$\forall \epsilon > 0, \exists \delta > 0$ such that:
$0 < |x - c| < \delta \implies |f(x) - L| < \epsilon$

### 🧠 Logic Check
- $\epsilon$ is the vertical tolerance (Error in $y$).
- $\delta$ is the horizontal tolerance (Control in $x$).
- If for EVERY $\epsilon$ there's a $\delta$, the limit exists.

<img width="1924" height="1084" alt="7b3b61f2-115b-49f7-a9bc-ad8a01e5fdfd" src="https://github.com/user-attachments/assets/068be7f5-eb56-47fe-9a87-2df9fbde6414" />

### Philosophy of Proof: Why Epsilon-Delta Matters?

1. **Safety & Robustness**: Intuition fails in complex high-dimensional systems (e.g., Economic models). Proof guarantees stability.
2. **Tolerance Engineering**: It defines the "allowable error." If I give you a tolerance $\epsilon$, can you guarantee a control $\delta$?
3. **Legalization of Calculus**: It turned calculus from a "useful trick" into a "rigorous science" by providing a non-ambiguous definition of "approaching."

> **Ludan's Insight**: In PhD research, a "feeling" isn't a finding. A "proof" is a finding.













# 🗓 2/9 Math Refresher: The Lego Blocks of Calculus & Algebra
> **Focus**: Linearity and Spatial Relationships.

### 🧩 1. Limit Properties (The "Split" Rule)
- $\lim(f \pm g) = L \pm M$
- $\lim(f \cdot g) = L \cdot M$
- **Rule of Thumb**: As long as they don't produce $\frac{0}{0}$ or $\infty$, you can treat limits like basic arithmetic.

### 📐 2. Spatial Geometry (Vector Tools)
- **Normal Vector**: The key to defining a plane ($Ax+By+Cz=D$).
- **Distance to Plane**: Essentially the projection of a vector onto the Normal Vector.
- **Connection**: To find the distance between two parallel planes, just pick a point on one and project it onto the normal of the other.

### 🧠 Ludan's Strategy
- In PhD-level Economics, we often use these properties to linearize complex non-linear models.



## 🧩 The Puzzle of Combined Limits
- **Individual Failure**: A function $f(x)$ can have a "Broken" limit (DNE).
- **Collective Success**: In $(f + g)$, as long as the SUM of left limits equals the SUM of right limits, the limit exists.
- **Commander's Strategy**:
    1. Separate the problem into Left and Right.
    2. Solve $f_{left} + g_{left}$ and $f_{right} + g_{right}$.
    3. Compare the totals.

<img width="1958" height="1036" alt="cde43f58-8c98-43e7-919f-9b8bf58c9d4d" src="https://github.com/user-attachments/assets/ac95faba-c9be-4806-ab9a-2222b88ad6a2" />

### Anwser is 4 (左右结果相等才行，不想相等依然不存在)



## 🛠️ The "Offsetting" Rule for Broken Limits
- **Case**: $f(x)$ and $g(x)$ both have jump discontinuities at $x=c$.
- **Theorem**: $\lim(f+g) = \lim f + \lim g$.
- **Execution Strategy**:
    - **Step 1**: Calculate Side Limits separately ($L_{left}$ and $L_{right}$).
    - **Step 2**: If the Sums match, the "Break" is healed.
- **Why this matters**: In Economics PhD level modeling, we often sum up different volatile sectors to find a stable equilibrium.

## 🧬 The "Peeling the Onion" Rule (Composite Limits)
- **Case**: Solving $\lim f(g(x))$.
- **Strategy**: Move the limit inside: $f(\lim g(x))$.
- **Pre-flight Checklist**:
    1. Does $\lim_{x \to a} g(x) = L$ exist?
    2. Is $f(y)$ continuous at $y=L$?
- **PhD Warning**: If $f$ is discontinuous at the relay point $L$, the "Chain" breaks. 
- **Application**: Analyzing how microscopic volatility ($g$) propagates through a non-linear institutional framework ($f$).

<img width="2122" height="1322" alt="98a9ddb3-add1-4732-8dca-177d5eb60e62" src="https://github.com/user-attachments/assets/edb33bdd-5ca3-4484-8afc-e3a06bde6a6b" />

## 🔗 Composite Function Limits: The Relay Race
- **Inner Function ($g$)**: Only provides the DESTINATION (the value $L$).
- **Outer Function ($f$)**: Its behavior AT that destination $L$ decides everything.
- **Existence Rule**:
  - If $f$ is **Continuous** at $L$, the limit exists and equals $f(L)$.
  - If $f$ is **Broken** at $L$, you must check the side-limits of the composition.
- **Conclusion**: A broken function can still produce a valid composite limit if you land on its continuous segments!

<img width="1636" height="1084" alt="33bbc37f-57ec-46fb-aae4-a33c106b4092" src="https://github.com/user-attachments/assets/d100c85d-50f0-4de9-994f-fe5fe6feebca" />

## 🛑 DNE Quick Check for Composite Limits: $\lim f(g(x))$
- **Step 1**: Check $\lim_{x \to a} g(x)$. If it doesn't exist $\implies$ **DNE**.
- **Step 2**: If $g(x) \to L$, check if $f$ is continuous at $L$. 
    - If **Yes** $\implies$ Result is $f(L)$.
    - If **No** (it's a jump) $\implies$ **MUST** check direction ($L^+$ or $L^-$).
- **Step 3**: Compare $f(L_{from\_left})$ and $f(L_{from\_right})$. 
    - If mismatched $\implies$ **DNE**.

<img width="1686" height="1084" alt="d408d962-8144-4575-86f7-e335e9ef8515" src="https://github.com/user-attachments/assets/f872f457-684f-466b-b47f-1266d346eb43" />

###  Answer is -2




# 学习日志：极限进阶——处理未定式 $0/0$
# 🗓 2026-02-23

---

## 一、 为什么 $0/0$ 时不能放弃？

在 2/23 的晨练题中，当你代入 $x = -1$ 时，会发现：
$$\lim_{x \to -1} \frac{x+1}{\sqrt{x+5}-2} = \frac{-1+1}{\sqrt{-1+5}-2} = \frac{0}{0}$$

### 📌 核心逻辑：未定式 (Indeterminate Form)
1. **隐藏因子**：分子和分母同时趋于 0，意味着它们内部都潜伏着一个共同的“零因子”（本题中是 $x+1$）。
2. **非死路，是隧道**：
   - **2/18 的极限 ($1/0$)**：这是“死路”。分母为 0 但分子不是 0，函数直冲无穷大。
   - **2/23 的极限 ($0/0$)**：这是“隧道”。虽然暂时看不见答案，但只要消掉那个零因子，极限值就会浮现。
3. **图形意义**：函数图像在此处通常只是一个“可去间断点”（一个小洞），极限值的任务就是找回这个洞的坐标。

---

## 二、 晨练题解：根式有理化 (Rationalizing)

当看到根号且出现 $0/0$ 时，最常用的武器就是**共轭根式**。

### 1️⃣ 证明/计算步骤
1. **乘以共轭项**：分子分母同时乘以 $(\sqrt{x+5} + 2)$
   $$\frac{x+1}{\sqrt{x+5}-2} \cdot \frac{\sqrt{x+5}+2}{\sqrt{x+5}+2}$$
2. **分母展开**：利用平方差公式 $(a-b)(a+b) = a^2 - b^2$。
   分母变为：$(\sqrt{x+5})^2 - 2^2 = x + 5 - 4 = x + 1$。
3. **关键约分**：
   $$\frac{(x+1)(\sqrt{x+5}+2)}{x+1} = \sqrt{x+5}+2$$
4. **代入求值**：
   $$\lim_{x \to -1} (\sqrt{x+5}+2) = \sqrt{4}+2 = 4$$

**结论：** 该极限值为 **4**。

<img width="2064" height="1030" alt="cf43b2ca-488f-4321-80d7-129bd3dab5d1" src="https://github.com/user-attachments/assets/7a0b5f42-f932-49d8-8a86-5176c029bacc" />


---

## 三、 对数计算复盘：$2\log_{3}(1/52)$

针对之前的计算偏差，在此记录严谨的计算路径：

1. **公式转换**：
   <!--  $ 2\cdot \frac{\ln(1/52)}{\ln(3)}$ -->
     <img width="396" height="188" alt="ebc58e31-eacf-49b1-9fee-9cea2dcf22bb" src="https://github.com/user-attachments/assets/fdf99c57-c5e9-4802-9d4c-3cd40afc2f5d" />

3. **分步计算**：
   - $\ln(1/52) \approx -3.951$
   - $\ln(3) \approx 1.099$
   - $\frac{-3.951}{1.099} \approx -3.595$
4. **最终结果**：$-3.595 \times 2 \approx -7.193$

---

## 四、 总结：极限处理决策树

1. **代入数值**。
2. **结果是 $L/0$ ($L \neq 0$)** → 极限不存在（趋向无穷），停止计算。
3. **结果是 $0/0$** → **不要放弃！** 尝试以下方法：
   - 有根号：**有理化**。
   - 多项式：**因式分解**（寻找并约掉零因子）。
   - 复杂函数：**洛必达法则**（后续进阶）。

---

## 🧠 今日认知升级
数学证明和极限计算都不是为了“显摆步骤”，而是为了通过**等价转换**，把我们看不清的“未定状态”翻译成我们可以处理的“确定状态”。在未来 **HEOR** 的灵敏度分析中，这种对数值微小趋势的捕捉至关重要。



## 2/25 晨练：极限计算决策树 (The Limit Strategy)

<img width="2000" height="1118" alt="image" src="https://github.com/user-attachments/assets/bf9dea44-dd17-443c-998d-95f084cb11c6" />


面对极限问题 $\lim_{x \to a} f(x)$，永远遵循以下逻辑路径：

### 1️⃣ 第一步：直接代入 (Direct Substitution)
- **结果是常数 $b$** → 恭喜，计算结束。
- **结果是 $b/0$** → 可能存在 **垂直渐近线 (Vertical Asymptote)**，需观察左右极限。
- **结果是 $0/0$** → 进入“未定式”解密环节。

### 2️⃣ 第二步：打破未定式 (Rewrite the Limit)
根据函数类型选择武器库：
- **A. 多项式 (Factoring)**：因式分解，约掉零因子。
- **B. 根式 (Conjugates)**：分子/分母有理化，利用 $(a-b)(a+b)$ 消去根号。
- **C. 三角函数 (Trig Identities)**：
  - 利用 $\cos 2\theta = 1 - 2\sin^2\theta$ 等公式。
  - 目标是消掉导致 $0/0$ 的那个三角项。

### 3️⃣ 第三步：重新评估
约分后的式子不再是 $0/0$，此时再次代入即可得到最终答案。





## 3/06 晨练：夹逼定理 (Squeeze Theorem)

### 📌 核心思想
当函数 $g(x)$ 的极限难以直接求解时，如果能找到两个函数 $f(x)$ 和 $h(x)$ 满足 $f(x) \le g(x) \le h(x)$，且这两者的极限都趋向同一个值 $L$，则 $g(x)$ 的极限也必然为 $L$。

### 📝 证明范式：震荡函数的消解
**题目：** $\lim_{x \to 0} x^2 \sin(1/x)$

1. **确立边界**：利用三角函数的有界性，知道 $-1 \le \sin(1/x) \le 1$。
2. **构建不等式**：同时乘以 $x^2$，得 $-x^2 \le x^2 \sin(1/x) \le x^2$。
3. **两端求极限**：
   - $\lim_{x \to 0} -x^2 = 0$
   - $\lim_{x \to 0} x^2 = 0$
4. **结论**：根据 **Squeeze Theorem**，$$\lim_{x \to 0} x^2 \sin\left(\frac{1}{x}\right) = 0$$
   <img width="406" height="172" alt="40cb04fd-4058-4dc3-b2cc-27262eb6d38b" src="https://github.com/user-attachments/assets/4eae3e2c-b29e-4abb-9f9e-485365743ef8" />


### 🧠 认知升级
- **适用场景**：通常用于处理包含 $\sin$ 或 $\cos$ 的震荡项，且该项前面乘了一个趋于 $0$ 的无穷小量。
- **直觉理解**：虽然震荡项在狂跳，但前面的 $x^2$ 像一个不断缩小的钳子，最终把震荡范围压缩到了一个点。

<img width="1820" height="852" alt="fc33a1f8-e6f4-4e6d-b09b-c9ad392aea61" src="https://github.com/user-attachments/assets/7e212561-eeb6-41a0-8c1d-0ecc050215b3" />






<img width="1990" height="1034" alt="f3429f40-3a3b-4f27-97c1-33ba9ab6c959" src="https://github.com/user-attachments/assets/6ba4fd1a-42b0-4244-981b-a82c3d6acdeb" />

<img width="1156" height="1534" alt="4de630c2-7953-41e4-b0d9-01600f1e27ca" src="https://github.com/user-attachments/assets/25ba086e-f2ae-43b9-ae91-152df31890c3" />


## 3/12 晨练：无穷大的方向性 (Direction of Infinity)

### 📌 核心认知
$\infty$ 和 $-\infty$ 绝对不是一回事。

1. **同向发散 (Agreement)**：如 $1/x^2$，左右都趋于 $\infty$，极限可视为 $\infty$。
2. **异向发散 (Disagreement)**：如 $1/x$，一正一负。这种“撕裂感”直接导致极限 **DNE (Does Not Exist)**。

### 💡 决策启示 (Logic Model)
在评估政策稳定性时，不仅要看平均值，更要看临界点是否会出现 $1/x$ 型的撕裂。如果左右极限不一致，系统在这一点上就是失效的。
<img width="1692" height="886" alt="c24d0ec3-c2b5-4823-9ac5-7c43734630b7" src="https://github.com/user-attachments/assets/c58f0cb8-6626-4dcf-845f-c2cbddce03b1" />



## 3/13 晨练：无穷极限的“抓大放小” (Dominant Term Rule)

### 📌 核心技巧
处理 $\lim_{x \to \infty}$ 的分式函数时，直接无视低阶项，只看最高次项。

### 📝 案例复盘
$$\lim_{x \to \infty} \frac{4x^5 - 3x^2 + 3}{6x^5 - 100x^2 - 10} = \frac{4}{6} = \frac{2}{3}$$

### 💡 哲学启示 (Logic Model)
在研究系统长期极限（Infinity）时，**“噪音”（低阶项）会随时间蒸发，唯有“信号”（主导项）决定方向**。这对于建立 HEOR 成本预测模型至关重要，能防止我们在细节中迷失而忽略了大趋势。

<img width="1324" height="402" alt="320866c4-eecc-46ad-b219-d7a8df345286" src="https://github.com/user-attachments/assets/c786d650-6cc6-4075-872b-0cb56dcbfbfe" />
<img width="1530" height="744" alt="9e38f654-c76c-45f9-a7f5-a10786673d54" src="https://github.com/user-attachments/assets/07338ec1-1be6-4855-a6f3-84c04a2fb6ff" />



## 介值定理 (Intermediate Value Theorem)

### 📌 核心逻辑
若 $f(x)$ 在 $[a, b]$ 连续，则它必将经过 $f(a)$ 与 $f(b)$ 之间的所有中间值。

### 🛠 判定工具：零点存在性
- 若 $f(a) < 0$ 且 $f(b) > 0$，则区间内必有 $f(c) = 0$。

### 💡 逻辑模型 (Logic Model)
在医疗政策或药物定价研究中，IVT 告诉我们：只要系统变量是连续变化的，从“亏损”到“盈利”的过程中，必然存在一个“收支平衡点”。我们虽然有时算不出确切的点，但能锁定它的存在区间。


