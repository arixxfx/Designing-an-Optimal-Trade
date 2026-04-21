# Optimal Trade Design: Size, Leverage, and Execution

This project develops a calculus-based framework to optimize three key trading decisions:

- Trade size under market impact
- Optimal leverage (Kelly criterion)
- Execution timing

## 🧠 Motivation

In quantitative trading, profitability is not just about predicting returns — it's about **optimizing how trades are executed** under real-world constraints like:

- Market impact
- Transaction costs
- Risk and volatility
- Execution timing

---

## ⚙️ Models

### 1. Trade Size Optimization

Profit function:

P(x) = αx - βx² - cx

Closed-form solution:

x* = (α - c) / (2β)

---

### 2. Leverage Optimization (Kelly)

Maximizing:

R(ℓ) = ℓμ - (1/2)ℓ²σ²

Optimal leverage:

ℓ* = μ / σ²

---

### 3. Execution Time Optimization

Cost function:

C(t) = k/t + λt

Optimal execution time:

t* = sqrt(k / λ)

---

## 📊 Results

- Trade size increases with alpha and decreases with market impact
- Optimal leverage strongly depends on volatility
- Execution time follows a U-shaped cost structure

---

## 🚀 How to Run

```bash
pip install -r requirements.txt
jupyter notebook
