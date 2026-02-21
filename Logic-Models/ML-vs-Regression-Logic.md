# HEOR Logic Models: Machine Learning (ML) vs. Traditional Regression

### 0. Context & Motivation
I aim to use econometric tools to uncover the "hidden heterogeneity" within medical data that traditional models often overlook.

---

### 1. The Paradigm Shift: Policy Research vs. HEOR
Through a recent "Compare Notes" session with Dr. Menghan Shen, I've refined the distinction between these two sister fields:

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

### 3. Topography of Data: "Standard Map" vs. "High-Res LiDAR"
In the context of architectural site analysis, a flat 2D map can hide crucial terrain details that determine whether a structure will stand. Data has a similar "hidden topography".

Traditional Tools are like Standard Site Prototyping: They apply a single, uniform "master plan" to every plot of land (patient). They assume the terrain is level, focusing only on the average elevation.

ML Tools are like High-Resolution LiDAR Scanning: They "scan" the data landscape to reveal the hidden ridges, ravines, and micro-climates that a flat map misses.

In HEOR terms: ML identifies the specific "micro-terrains" (patient sub-groups) where a drug’s efficacy might peak or valley unexpectedly, which is critical for Young-Onset Parkinson's Disease (YOPD) research where patient heterogeneity is the rule, not the exception.
