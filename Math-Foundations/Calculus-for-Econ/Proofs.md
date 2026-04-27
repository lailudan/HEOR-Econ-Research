# Derivative of Power Functions — Avoiding Circular Reasoning

## 🎯 Goal

Prove:
$$
\frac{d}{dx} x^n = n x^{n-1}
$$

---

## 🚨 The Concern: Circular Reasoning

A common proof uses logarithmic differentiation:

$$
y = x^n \Rightarrow \ln y = n \ln x
$$

$$
\frac{y'}{y} = \frac{n}{x} \Rightarrow y' = nx^{n-1}
$$

This relies on:
$$
\frac{d}{dx} \ln x = \frac{1}{x}
$$

If this itself depends on the power rule, we get a circular argument.

---

## 🔁 Where Circular Reasoning Appears

If we define:
$$
\ln x = \int \frac{1}{x} dx
$$

and compute integrals using power rules, then:

Power Rule → Integration → ln(x) → Power Rule

This is a logical loop (invalid).

---

## ✅ Clean Proof (No Circular Reasoning)

### Step 1: Definition of Derivative

$$
\frac{d}{dx}f(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}
$$

### Step 2: Basic Results

$$
\frac{d}{dx}x = 1, \quad \frac{d}{dx}c = 0
$$

### Step 3: Product Rule (from limits)

$$
\frac{d}{dx}(fg) = f'g + fg'
$$

### Step 4: Induction

Assume:
$$
\frac{d}{dx}x^{n-1} = (n-1)x^{n-2}
$$

Then:
$$
x^n = x \cdot x^{n-1}
$$

$$
\frac{d}{dx}x^n = x \cdot (n-1)x^{n-2} + x^{n-1}
$$

$$
= (n-1)x^{n-1} + x^{n-1} = nx^{n-1}
$$

✔ Proven without circular reasoning

---

## 🧠 Logarithmic Method (Valid Version)

Only valid if built from independent definitions.

### Step A: Define exponential

$$
e^x = \lim_{n\to\infty}\left(1+\frac{x}{n}\right)^n
$$

### Step B:

$$
\frac{d}{dx}e^x = e^x
$$

### Step C: Define logarithm

$$
\ln x = (e^x)^{-1}
$$

$$
\frac{d}{dx}\ln x = \frac{1}{x}
$$

### Step D: Apply

$$
y = x^n \Rightarrow \ln y = n \ln x
$$

$$
\frac{y'}{y} = \frac{n}{x} \Rightarrow y' = nx^{n-1}
$$

✔ No circular dependency

---

## 🔍 Dependency Structure

### ❌ Invalid

Power Rule → Integration → ln(x) → Power Rule

### ✅ Valid Path 1

Limit Definition → Product Rule → Power Rule

### ✅ Valid Path 2

Limit Definition → Exponential → Logarithm → Power Rule

---

## ✨ Key Insight

- Circular reasoning: A → B → A  
- Valid reasoning: A → deeper foundation → result

---

## 🧩 Summary

To rigorously prove:
$$
\frac{d}{dx} x^n = n x^{n-1}
$$

You must ensure:

- No hidden dependencies  
- No logical cycles  
- All steps trace back to independent definitions  

---

## 🧠 Meta Insight

This is about understanding the **dependency graph of mathematics**,  
not just computing derivatives.
