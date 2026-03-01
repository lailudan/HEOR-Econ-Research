# 📘 Proof of 2×2 Matrix Inverse Formula and Determinant Analysis

## I. Proposition
Let matrix $A$ be defined as:
$$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix}$$

If the determinant $\det A = ad - bc \neq 0$, then the inverse matrix $A^{-1}$ is given by:
$$A^{-1} = \frac{1}{ad - bc} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

---

## II. Proof (Direct Construction Method)
We construct an adjugate matrix $B = \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$ and calculate the product $AB$.

### Step 1: Matrix Multiplication
$$AB = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$

Calculating each entry of the resulting matrix:
* **Top-Left**: $ad + b(-c) = ad - bc$
* **Top-Right**: $a(-b) + ba = -ab + ab = 0$
* **Bottom-Left**: $cd + d(-c) = cd - dc = 0$
* **Bottom-Right**: $c(-b) + da = -cb + ad = ad - bc$

### Step 2: Simplifying the Result
$$AB = \begin{bmatrix} ad-bc & 0 \\ 0 & ad-bc \end{bmatrix} = (ad - bc) \begin{bmatrix} 1 & 0 \\ 0 & 1 \end{bmatrix} = (\det A) I$$

### Step 3: Deriving the Inverse
If $\det A \neq 0$, we can divide both sides by the scalar $\det A$:
$$A \left( \frac{1}{\det A} B \right) = I$$

Therefore:
$$A^{-1} = \frac{1}{\det A} \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$$
**Q.E.D.**

---

## III. Analysis of Determinant Cases

### Case 1: $\det A \neq 0$
**Matrix is Invertible**. Since $AB = (\det A)I$, as long as the scaling factor is non-zero, we can "rescale" the transformation back to the Identity Matrix.

### Case 2: $\det A = 0$
In this case, $AB = \mathbf{0}$. It is impossible to rescale the matrix back to $I$. Therefore, **$A$ is Singular (Non-invertible)**.

**Geometric Interpretation**:
* $\det A$ represents the area scaling factor.
* If $\det A = 0$, the area is compressed to zero. The 2D plane is "squashed" into a 1D line or a 0D point.
* **Information Loss**: Once dimensions collapse, the original input cannot be recovered.



### Case 3: $\det A < 0$
**Matrix remains Invertible**. The area is scaled by a factor of $|\det A|$, but the **orientation is flipped** (similar to a mirror reflection).

---

## IV. Structural Intuition
For a $2 \times 2$ matrix, the inverse is essentially:
$$A^{-1} = \frac{\text{adj}(A)}{\det A}$$

Where the adjugate matrix $\text{adj}(A) = \begin{bmatrix} d & -b \\ -c & a \end{bmatrix}$ provides the **direction correction**, satisfying the core identity:
$$A \cdot \text{adj}(A) = (\det A)I$$

---

## V. Key Takeaways
1.  **Determinant** is the spatial scaling factor.
2.  **$\det A = 0$** $\iff$ Singular matrix (Spatial collapse).
3.  **Inverse Matrix** = Directional Correction (Adjugate) + Scale Correction (Inverse Determinant).
