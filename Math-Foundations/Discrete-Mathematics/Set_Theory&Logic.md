
### 02/04 Discrete Math ⚖️ Logic Comparison: OR vs. XOR （正序笔记）

| Operator | Symbol | Logical Meaning | Real-world Analogy |
| :--- | :--- | :--- | :--- |
| **Inclusive OR** | $p \vee q$ | At least one is true (Both OK) | Citizenship or Permanent Residency |
| **Exclusive OR (XOR)** | $p \oplus q$ | Exactly one is true (Not both) | Coffee or Tea (Fixed Menu) |

**Truth Table Verification:**
| p | q | $p \vee q$ | $p \oplus q$ |
|:-:|:-:|:---------:|:-----------:|
| T | T | **T** | **F** (The Difference!) |
| T | F | T | T |
| F | T | T | T |
| F | F | F | F |

**Insight for Codebreaking:**
In Cryptography (like Enigma), **XOR** is the king. Most encryption algorithms rely on XOR because it is its own inverse: if you XOR something twice with the same key, you get the original back.


# 🧮 Discrete Mathematics: Core Logic Symbols Reference

This document provides a concise breakdown of essential symbols used in Propositional Logic, Predicate Logic, and Number Theory.

---

## 1. Propositional Logic: The "OR" Distinction
The most common point of confusion is the difference between an inclusive and an exclusive choice.

| Symbol | Name | Logic Operator | Definition |
| :--- | :--- | :--- | :--- |
| **$p \vee q$** | **OR (Inclusive)** | $p \cup q$ | True if $p$ is true, $q$ is true, **or both**. |
| **$p \oplus q$** | **XOR (Exclusive)** | $p \text{ XOR } q$ | True if **exactly one** of $p$ or $q$ is true. False if both are true. |



---

## 2. Predicate Logic: Quantifiers
Quantifiers define the **scope** of a logical statement within a set.

* **$\forall$ (Universal Quantifier):** "For all". The statement must hold for **every** element in the domain.
    * *Example:* $\forall n \in \mathbb{Z}, n^2 \geq 0$.
* **$\exists$ (Existential Quantifier):** "There exists". At least **one** element in the domain must satisfy the statement.
    * *Example:* $\exists x \in \mathbb{R}, x^2 = 2$.
* **$P(x) \Rightarrow Q(x)$:** Implies that if $x$ satisfies property $P$, it **must** also satisfy property $Q$.



---

## 3. Number Theory & Operations
Key operators used in modular arithmetic and algorithm analysis.

| Symbol | Read As | Definition |
| :--- | :--- | :--- |
| **$d \mid n$** | $d$ divides $n$ | $n$ is a multiple of $d$; the remainder is 0. |
| **$n \pmod d$** | $n$ mod $d$ | The integer remainder of $n$ divided by $d$. |
| **$\lfloor x \rfloor$** | Floor of $x$ | The largest integer $\leq x$. (Example: $\lfloor 3.9 \rfloor = 3$) |
| **$\lceil x \rceil$** | Ceiling of $x$ | The smallest integer $\geq x$. (Example: $\lceil 3.1 \rceil = 4$) |

---

## 4. Logic Gates (Physical Implementation)
Logic transformed into hardware architecture.

* **NAND Gate ($|$):** The "Universal Gate." Output is False **only if all** inputs are True.
* **NOR Gate ($\downarrow$):** Output is True **only if all** inputs are False.



[Image of logic gate symbols for NAND and NOR including truth tables]


---

## 5. Notation for Proof Writing

* **$x := e$** : **Assignment/Definition**. Used when defining a new variable or constant (e.g., "Let $s := a+b$").
* **$\equiv$** : **Logical Equivalence**. Used when two statements have identical truth tables.
* **$\therefore$** : **Therefore**. Used to denote the conclusion of a proof.
* **$\blacksquare$ or $\square$** : **Q.E.D.** (Quod Erat Demonstrandum). Marks the end of a formal proof.

---

> **Note to Self:** When analyzing a system (like the 8-puzzle or economic models), always check if the rules use $\vee$ or $\oplus$. Misunderstanding the "OR" type can lead to a broken invariant proof.





<img width="1314" height="1778" alt="f6a21f84-69c0-4628-a72a-613b0e634e42" src="https://github.com/user-attachments/assets/d081fa11-4068-4a1d-8799-93d87140ee33" />


# 🗓️ 集合论核心笔记：关系、运算与逻辑子空间 updated 2026-02-26


## 一、 集合间的基本关系 (Relationships)

### 1. 子集 (Subset)
- **定义**: 如果集合 $A$ 的任意一个元素都是集合 $B$ 的元素，则称 $A$ 是 $B$ 的**子集**。
- **符号**: $A \subseteq B$（读作“A包含于B”或“B包含A”）。
- **性质**:
    - **自反性**: $A \subseteq A$。
    - **传递性**: 若 $A \subseteq B$ 且 $B \subseteq C$，则 $A \subseteq C$。
    - **空集特性**: $\varnothing \subseteq A$（空集是任何集合的子集）。

### 2. 真子集 (Proper Subset)
- **定义**: 如果 $A \subseteq B$，但存在元素 $x \in B$ 且 $x \notin A$，则称 $A$ 是 $B$ 的**真子集**。
- **符号**: $A \subsetneq B$。
- **性质**: $\varnothing$ 是任何非空集合的真子集。

### 3. 集合相等 (Equality)
- **定义**: $A \subseteq B$ 且 $B \subseteq A \iff A = B$。

---

## 二、 集合的计数规律 (Combinatorics)

对于含有 $n$ 个元素的有限集 $A$：

| 集合类型 | 计算公式 | 备注 |
| :--- | :--- | :--- |
| **子集总数** | $2^n$ | 包含空集和自身 |
| **真子集数** | $2^n - 1$ | 除去自身 |
| **非空子集数** | $2^n - 1$ | 除去空集 |
| **非空真子集数** | $2^n - 2$ | 除去空集和自身 |

---

## 三、 集合的基本运算 (Operations)

### 1. 交集 (Intersection)
- **定义**: $A \cap B = \{x \mid x \in A \text{ 且 } x \in B\}$
- **直观理解**: 两个圈重叠的部分。

### 2. 并集 (Union)
- **定义**: $A \cup B = \{x \mid x \in A \text{ 或 } x \in B\}$
- **直观理解**: 两个圈合并后的所有领土。

### 3. 补集 (Complement)
- **全集 ($U$)**: 包含研究所涉及的所有元素的集合。
- **补集定义**: $\complement_U A = \{x \mid x \in U \text{ 且 } x \notin A\}$
- **直观理解**: “非 A”的所有区域。

<img width="1542" height="850" alt="534b4f98e06f604f27fdfb793f14fdbe" src="https://github.com/user-attachments/assets/73a2bd68-f26f-4d67-9cf3-597895e9f5b3" />
<img width="1544" height="852" alt="e5facaeb336169f01ecd82ff16264325" src="https://github.com/user-attachments/assets/6fd81cf4-8f9f-4a37-b20d-baf2ba5e1a77" />
<img width="1540" height="844" alt="a111feffdeff5baff4f5b8554eed7a84" src="https://github.com/user-attachments/assets/8691dbbb-d0f7-4483-b44f-016e4225213b" />


---

## 四、 核心逻辑定律：德·摩根定律 (De Morgan's Laws)

在处理复杂的否定逻辑（如 HEOR 模型中的排除标准）时极其重要：

1. **“交的补等于补的并”**: $\complement_U(A \cap B) = (\complement_U A) \cup (\complement_U B)$
2. **“并的补等于补的交”**: $\complement_U(A \cup B) = (\complement_U A) \cap (\complement_U B)$

---

## 🧠 PhD 建模思维连接 (Ludan's Research Insight)

1. **从集合到子空间 (Subspace)**: 
   线性代数中的“子空间”其实就是一个特殊的集合。它不仅要求元素属于大集合，还要求对加法和数乘保持“封闭”。
2. **条件概率的基石**: 
   概率 $P(A|B)$ 的本质就是在 $B$ 这个子集（集合）的范围内，考察 $A \cap B$ 所占的比例。
3. **数据筛选逻辑**: 
   在 SQL 或 Python 数据处理中，`AND` 对应 $\cap$，`OR` 对应 $\cup$，`NOT` 对应 $\complement$。
