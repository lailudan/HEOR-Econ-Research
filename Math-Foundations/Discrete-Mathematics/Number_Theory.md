# 📚 MIT 6.042J 学习日志 | 2026-02-09
## Lec 4: 数论与水桶博弈 (Number Theory I)

# 1. 核心模型：水桶问题的数学化
- **情境：** 给定容积为 $a, b$ 的两个水桶，能量出多少水？
- **状态机模拟：**
  - 起始状态：$(0, 0)$
  - 转移规则：注满 (Fill)、倒空 (Empty)、倾倒 (Pour)。
- **结论：** 所有可达状态 $(x, y)$ 必须满足 $x, y$ 都是 $\gcd(a, b)$ 的倍数。

### 🚫 Case Study: The Impossibility Proof (3G & 6G vs. 4G)

**Theorem:** It is impossible to measure 4 gallons using only 3-gallon and 6-gallon jugs.

**Proof by Divisibility:**
1. Let the volumes of the jugs be $a=3$ and $b=6$.
2. Any volume $V$ that can be measured must be a linear combination of $a$ and $b$: $V = sa + tb$, where $s, t \in \mathbb{Z}$.
3. We know that $V$ must be a multiple of $\gcd(a, b)$.
4. $\gcd(3, 6) = 3$.
5. Therefore, any measurable volume $V$ must satisfy $V \equiv 0 \pmod 3$.
6. Since $4 \equiv 1 \pmod 3$, 4 is not a multiple of 3 ($3 \nmid 4$).

**Conclusion:** The state $V=4$ is outside the reachable state space of this system.

---
**PhD Note:** 在系统建模中，识别这种“结构性限制”可以节省大量无效计算。如果你知道目标的 GCD 最大公约数不对，你根本不需要去尝试任何路径。





# 2. 数论基本概念 (The Toolkit)
- **整除 ($d \mid n$)：** 存在整数 $k$ 使得 $n = kd$。
- **公约数：** 如果 $d \mid a$ 且 $d \mid b$，则 $d$ 是公约数。
- **线性组合 (Linear Combination)：** 形如 $sa + tb$ 的数（$s, t$ 为整数）。

# 3. 贝祖定理 (Bézout's Identity) —— 核心中的核心
- **定理内容：** $\gcd(a, b)$ 是 $a$ 和 $b$ 的**最小正线性组合**。
- **应用：** 如果你想量出 $k$ 加仑水，前提是 $\gcd(a, b) \mid k$。
- **实战：** 如果你拿 33 和 55 加仑的桶去量 4 加仑，你会炸掉，因为 $\gcd(33, 55)=11$，而 11 不整除 4。

## **核心结论：** 两个整数 $a$ 和 $b$ 的最大公约数 $GCD(a, b)$，是这两个数通过整数倍加减（线性组合）所能凑出的**最小正整数**。

**公式表达：**
对于任何整数 $a, b$，一定存在整数 $s, t$ 使得：
$s \cdot a + t \cdot b = GCD(a, b)$

## 视频中的“倒水”实例分析
通过控制两个桶的灌满、倒空和互倒，本质上是在做 $s \cdot a + t \cdot b$ 的运算。

## 案例 A：电影《虎胆龙威 3》原题
* **已知：** 3加仑桶 ($a=3$)，5加仑桶 ($b=5$)
* **计算：** $GCD(3, 5) = 1$
* **结论：** 最小能量出 1 加仑。因为目标 **4 加仑** 是 1 的倍数，所以**可行**。
* **数学组合：** $4 = 2 \cdot 5 + (-2) \cdot 3$ （灌满两次5加仑，倒掉两次3加仑）。

### 案例 B：失败的逻辑
* **已知：** 3加仑桶 ($a=3$)，6加仑桶 ($b=6$)
* **计算：** $GCD(3, 6) = 3$
* **结论：** 能量出的水量只能是 3 的倍数（3, 6, 9...）。由于 **4 加仑** 不是 3 的倍数，**任务无解**。

### 案例 C：恶搞版《虎胆龙威 5》
* **已知：** 33加仑桶，55加仑桶
* **计算：** $GCD(33, 55) = 11$
* **结论：** 只能凑出 11 的倍数。想要量出 4 加仑在数学上是**不可能**的。

##  总结
一个目标值是否能被两个基础单位“凑”出来，取决于该目标值是否能被这两个单位的最大公约数整除。

# 4. 算法：欧几里得算法 (Euclidean Algorithm)
- **思考：** 这是一个不断缩小搜索空间（降维）的过程。

## 1. 核心定义
辗转相除法（又称欧几里得算法）是计算两个整数 **最大公约数 (Greatest Common Divisor, GCD)** 的高效算法。

**数学原理：**
$GCD(a, b) = GCD(b \pmod a, a)$
(即：两个数的最大公约数，等于其中较小的数与两数相除余数的最大公约数。)

## 2. 视频中的计算实例
**任务：求 $GCD(105, 224)$**

| 步骤 | 计算过程 | 结论 |
| :--- | :--- | :--- |
| **Step 1** | $224 \div 105 = 2 \dots 14$ | $GCD(105, 224) = GCD(14, 105)$ |
| **Step 2** | $105 \div 14 = 7 \dots 7$ | $GCD(14, 105) = GCD(7, 14)$ |
| **Step 3** | $14 \div 7 = 2 \dots 0$ | $GCD(7, 14) = GCD(0, 7)$ |

**最终结果：** 当余数为 0 时，剩下的非零数 **7** 即为 $GCD(105, 224)$。

## 3. 计算机科学意义
这是计算机科学中最基础的算法之一。它的时间复杂度极低（对数级别），是现代加密算法（如 RSA）中必不可少的预处理步骤。





