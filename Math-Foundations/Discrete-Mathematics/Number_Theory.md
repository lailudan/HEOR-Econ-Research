# 📚 MIT 6.042J 学习日志 | 2026-02-09
## Lec 4: 数论与水桶博弈 (Number Theory I)

### 1. 核心模型：水桶问题的数学化
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





### 2. 数论基本概念 (The Toolkit)
- **整除 ($d \mid n$)：** 存在整数 $k$ 使得 $n = kd$。
- **公约数：** 如果 $d \mid a$ 且 $d \mid b$，则 $d$ 是公约数。
- **线性组合 (Linear Combination)：** 形如 $sa + tb$ 的数（$s, t$ 为整数）。

### 3. 贝祖定理 (Bézout's Identity) —— 核心中的核心
- **定理内容：** $\gcd(a, b)$ 是 $a$ 和 $b$ 的**最小正线性组合**。
- **应用：** 如果你想量出 $k$ 加仑水，前提是 $\gcd(a, b) \mid k$。
- **实战：** 如果你拿 33 和 55 加仑的桶去量 4 加仑，你会炸掉，因为 $\gcd(33, 55)=11$，而 11 不整除 4。

### 4. 算法：欧几里得算法 (Euclidean Algorithm)
- 递归公式：$\text{gcd}(a, b) = \text{gcd}(b \pmod a, a)$。
- **思考：** 这是一个不断缩小搜索空间（降维）的过程。





