# Group Theory (群论) 学习笔记 2026-02-16

**Source Material:**
1. [What is Group Theory? (Ep. 1)](https://youtu.be/KufsL2VgELo)
2. [Simplifying problems with isomorphisms (Ep. 2)](https://www.youtube.com/watch?v=VZiLpYC0t5E)

---

## 1. 群的定义 (Definition of a Group)

群论研究的是集合及其运算规则的代数结构。一个群 $(G, \cdot)$ 由一个集合 $G$ 和一个二元运算 $\cdot$ 组成，必须满足以下**四条公理 (Axioms)**：

### 1.1 四大公理
1.  **封闭性 (Closure)**
    对于任意 $a, b \in G$，运算结果 $a \cdot b$ 必须仍在集合 $G$ 中。
2.  **结合律 (Associativity)**
    对于任意 $a, b, c \in G$，有 $(a \cdot b) \cdot c = a \cdot (b \cdot c)$。这意味着运算顺序（括号的位置）不改变结果，因此通常可以省略括号。
3.  **单位元 (Identity / Neutral Element)**
    群中存在唯一的元素 $e$（或写作 $1, 0$），对于任意 $a \in G$，满足 $a \cdot e = e \cdot a = a$。
    * *注：单位元在群中是唯一的。*
4.  **逆元 (Inverse)**
    对于任意 $a \in G$，存在唯一的元素 $a^{-1}$，满足 $a \cdot a^{-1} = a^{-1} \cdot a = e$。
    * *注：逆元在群中是唯一的，且 $(a^{-1})^{-1} = a$。*

### 1.2 常见群示例
| 群名称 | 符号 | 运算 | 说明 |
| :--- | :--- | :--- | :--- |
| **整数群** | $(\mathbb{Z}, +)$ | 加法 | 单位元是 0，逆元是 $-a$。 |
| **有理数群** | $(\mathbb{Q} \setminus \{0\}, \times)$ | 乘法 | 必须排除 0，单位元是 1，逆元是 $1/a$。 |
| **循环群** | $C_n$ 或 $\mathbb{Z}_n$ | 模加法 | 像时钟一样循环（例如 $\mathbb{Z}_6$ 中 $4+5=3$）。 |
| **二面体群** | $D_n$ | 变换 | 正 $n$ 边形的对称变换（旋转 + 翻转）。**不可交换** (Non-commutative)。 |

---

## 2. 子群与结构 (Subgroups & Structure)

### 2.1 子群 (Subgroups)
若群 $G$ 的子集 $H$ 在 $G$ 的运算下也满足群的四大公理，则 $H$ 是 $G$ 的子群。
* **生成子群 (Generated Subgroup)**: 由元素 $a$ 的所有幂次（$a, a^2, a^3...$）构成的子群，记为 $\langle a \rangle$。

### 2.2 陪集 (Cosets)
陪集是子群的“平移”副本。对于子群 $H$ 和元素 $g \in G$，陪集定义为 $gH = \{gh \mid h \in H\}$。
* **性质**：陪集将整个群 $G$ 分割成若干个大小相等且互不重叠的部分。

### 2.3 拉格朗日定理 (Lagrange's Theorem)
对于有限群 $G$ 和其子群 $H$：
$$|H| \text{ divides } |G|$$
即：**子群的阶（元素个数）整除群的阶**。
* **推论**: 阶数为质数 $p$ 的群只有唯一的结构，即循环群 $C_p$。

---

## 3. 群的变换与映射 (Morphisms)

这一部分主要讨论如何通过映射来简化问题或识别结构。

### 3.1 同态 (Homomorphism) —— "Simplification"
同态是保持运算结构的映射 $\phi: G \to H$。
* **一致性条件 (Consistency Condition)**:
    若 $a \cdot b = c$，则 $\phi(a) \cdot \phi(b) = \phi(c)$。
* **作用**: 将复杂问题转化为简单问题。
    * *例子*: 通过映射 $\mathbb{Z} \to \mathbb{Z}_2$ (Odd/Even) 来判断大数求和的奇偶性。
    * *性质*: 单位元映射到单位元 ($e_G \to e_H$)，逆元映射到逆元。

### 3.2 同构 (Isomorphism) —— "Renaming"
同构是双射（一一对应）的同态，记为 $G \cong H$。
* **含义**: 两个群在结构上完全相同，只是元素的“标签”不同。
* **威力**: 可以将未解决的问题从一个群转移到另一个已知的同构群中解决，再映射回来。
* **经典案例**:
    * $\mathbb{Z}_{11}^*$ (模11乘法群) $\cong \mathbb{Z}_{10}$ (模10加法群)。
    * 利用此性质，证明了在 $\mathbb{Z}_p^*$ 中，平方数（Quadratic Residues）恰好占一半，这被应用于密码学和公平抛硬币协议。

### 3.3 自同构 (Automorphism) —— "Symmetry"
自同构是从群 $G$ 到它自身的同构 ($\phi: G \to G$)。
* **含义**: 对群内元素进行重新标记（Relabeling），但保持原有结构不变。
* **自同构群 (Automorphism Group)**: 一个群的所有自同构集合本身也构成一个群，记为 $\text{Aut}(G)$。
    * $\text{Aut}(G)$ 是一种“元系统” (Meta-system)，即“群的群”。
* **应用**: 图同构问题 (Graph Isomorphism Problem) 可以转化为寻找图的自同构群。

---

## 4. 核心总结 (Key Takeaways)

1.  **抽象化**: 群论通过四条简单公理，统一了数字、几何变换、矩阵等多种数学对象的研究。
2.  **对称性**: 群是描述对称性的语言（如 $D_n$ 描述几何对称，$\text{Aut}(G)$ 描述代数结构的内部对称）。
3.  **问题简化**:
    * 利用 **Lagrange Theorem** 排除不可能的子群结构。
    * 利用 **Homomorphism** 忽略细节（如只看奇偶性）。
    * 利用 **Isomorphism** 在不同模型间迁移解题方法。
