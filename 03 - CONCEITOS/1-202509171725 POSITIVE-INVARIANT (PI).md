---
ID: 1-202509171725
tags:
  - nota-conceito
Referência: "[[1-202509171724 - On Positively Invariant Polyhedral Sets and Bilinear Programming for Designing Constrained Controllers]]"
Relação:
Temas: "[[1 - ENGENHARIA]]"
---
# CONCEITO
> A set $S \subset \mathbb{R}^n$ is **positive invariant (PI)** if for any initial conditions $x_0 \in S$ the state trajectory  $x_k \in S$ for all $k > 0$.

This definition basically means that if the state space trajectory starts inside a __positive invariant set__ it will remain there .

The second definition of $\lambda$-PI is that 

> A set $S \subset \mathbb{R}^n$ is **$\lambda$-contractive positive invariant (PI)** if for any $x_k \in S$, $X_{k+1} \in \lambda S$, with $0 < \lambda < 1$.

So, every step leads to a smaller set. $x_k$ is going to origin when $k \to \inf$.
