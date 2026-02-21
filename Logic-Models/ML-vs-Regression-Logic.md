# HEOR Logic Models: Machine Learning (ML) vs. Traditional Regression

### 0. Context & Motivation
I aim to use econometric tools to uncover the "hidden heterogeneity" within medical data that traditional models often overlook.

---

### 1. The Paradigm Shift: Policy Research vs. HEOR
Through a recent "Compare Notes" session with Dr. Mandy Shen, I've refined the distinction between these two sister fields:

* **Policy Research**: Primarily focuses on the **Average Treatment Effect (ATE)**. It asks: "Is this policy effective for the general population?" The logic is rooted in **macro-level equity**.
* **HEOR**: Primarily focuses on the **Conditional Average Treatment Effect (CATE)** or **Heterogeneity of Treatment Effect (HTE)**. It asks: "Does this specific drug provide a significant cost-effectiveness ratio for a sub-group, such as YOPD patients under 45 with specific genetic markers?". The logic is rooted in **micro-level value** and **Precision Medicine**.

---

### 2. Deductive (Regression) vs. Inductive (ML)

| Feature | Traditional Regression (OLS/Logit) | Machine Learning (Causal Forest) |
| :--- | :--- | :--- |
| **Epistemology** | **Deductive**: Theory-driven. You must "know" the hypothesis before testing it. | **Inductive**: Data-driven. It discovers patterns humans may not have the imagination to assume. |
| **Dimensionality** | **Low-dimensional**. Struggling with "Multi-collinearity" if too many variables are added. | **High-dimensional**. Built for **Real-World Evidence (RWE)** with thousands of noisy features. |
| **Objective** | Finding the "Average" and its statistical significance. | Finding "Specialness" and the **Unknown Unknowns**. |
| **Limitation** | Highly dependent on the researcher’s existing biases and assumptions. | Can fall into the trap of "Correlation" without a solid causal framework. |

---

### 3. The "Ajin" Metaphor & Hidden Variables
In the world of big data, AI does not inherently know who the "Ajin" (those with hidden, supernatural-like physiological traits) are. 
* **Traditional Tools** are like **Standard Blueprints**: They attempt to apply the same structural formulas to every plot of land (patient).
* **ML Tools** are
