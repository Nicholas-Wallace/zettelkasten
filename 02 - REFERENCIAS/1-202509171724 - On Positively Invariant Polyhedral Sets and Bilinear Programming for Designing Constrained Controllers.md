---
ID: 1-202509171724
tags:
  - nota-referência
Temas: "[[1 - ENGENHARIA]]"
---
# REFERÊNCIAS

# RELEVÂNCIA

# RESUMO

# CITAÇÕES E COMENTÁRIOS

> A set $S \subset \mathbb{R}^n$ is **positive invariant (PI)** if for any initial conditions $x_0 \in S$ the state trajectory  $x_k \in S$ for all $k > 0$.

This definition basically means that if the state space trajectory starts inside a __positive invariant set__ it will remain there .

The second definition of $\lambda$-PI is that 

> A set $S \subset \mathbb{R}^n$ is **$\lambda$-contractive positive invariant (PI)** if for any $x_k \in S$, $X_{k+1} \in \lambda S$, with $0 < \lambda < 1$.

So, every step leads to a smaller set. $x_k$ is going to origin when $k \to \inf$.

Constraints in a control problem can be represented by a set of linear inequalities that define a convex polyhedron as:

> $L = \{ x \in \mathbb{R}^{n_x} : Lx < l \}, \quad L \in \mathbb{R}^{rl \times n_x}, \quad 0 < l \in \mathbb{R}$

where rl is the number of constraints. 
To ensure that L will be compact (closed and bounded), $rl > n_x$. This make sense. Think in a 2d space(nx = 2), we need at least 3 inequalities to close a polygon. Also $rank(L) = n_x$. 

For a system $x_{k+1} = Ax_k$, To ensure $\lambda$-PI we need:
> $Lx_k < l \to Lx_{k+1} < \lambda l$ or $Lx_k < l \to LAx_k < \lambda l$  

There goes the *Extended Farkas’ Lemma* 

> $L2x \le l2 \to L1x \le l1$
> 	if, and only if
> 	there is a non negative matrix D, such that
> $DL2 = L1$
> $DL2 \le l1$


