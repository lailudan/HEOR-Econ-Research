# 🗓 3/4 Light Loading: Probability Literature
> **Goal**: Build intuition without the heavy lifting of calculus.

### 📖 Reading List:
1. *Naked Statistics* - Best for Big Picture & Intuition.
2. *The Signal and the Noise* - Best for Bayesian Prediction.
3. *The Drunkard's Walk* - Best for understanding Randomness.

### 💡 PhD Insight:
- High-level modeling isn't just about solving equations; it's about knowing **which** model fits the real-world mess. 
- These books provide the "Story" behind the "Math".

<br>
<br>
<br>
<br>


# 🗓 3/5 Probability Warm-up: Binomial Basics
> **Question**: $P(\text{Exactly 2 Heads in 3 flips})$

### 🧩 1. The Math
- **Total Outcomes**: $2^n = 2^3 = 8$.
- **Successful Outcomes**: $\binom{3}{2} = 3$ (HHT, HTH, THH).
- **Probability**: $3/8 = 0.375$.

### 🧠 Ludan's Insight (Structural Logic)
- This is a **Binomial Distribution (二项分布)** in its simplest form.
- In HEOR, this is like calculating the probability that 2 out of 3 patients react positively to a treatment, given a 50/50 chance.
- **The "Exactly" Trap**: If the question was "At least 2 heads", we would need to add the HHH case ($3/8 + 1/8 = 4/8$).
