# American Option Pricing using Tilley's Algorithm (Monte Carlo Simulation)

The content of this notebook is based on a paper "Valuing American Options in a Path Simulation Model" by James A. Tilley. <br>

## Overview

This project implements a Monte Carlo simulation for pricing an American put option under the Geometric Brownian Motion (GBM) model.

---

## Model Assumption

The underlying stock price follows a Geometric Brownian Motion (GBM):

$$\frac{dS(t)}{S(t)} = r dt + \sigma dW(t)$$

where:
- $S(t)$: stock price at time t  
- $r$: risk-free interest rate  
- $\sigma$: volatility  
- $W(t)$: Wiener process

---

## Option Type

- American put option
- Payoff: max(K - S(t), 0)
- Maturity: T = 1
- Discretized exercise dates: \{0.1, 0.2, ..., 1\}.

---

## Method

### Tilley's Algorithm
- Simulate the path of stock prices $S(t)$ using GBM
- Backward induction
- Identify the optional excercise time

---

## Features

- GBM-based stock price simulation
- American put option pricing

---

## Tech Stack

- Python
- NumPy

---

## References

1. James A. Tilley. *Valuing American Options in a Path Simulation Model*. Transactions of the Society of Actuaries. 45. 1993.

---
