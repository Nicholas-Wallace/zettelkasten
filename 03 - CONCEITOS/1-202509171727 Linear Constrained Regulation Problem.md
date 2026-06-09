---
ID: 1-202509171727
tags:
  - nota-conceito
Referência: "[[1-202510191810 - Output feedback design for discrete-time constrained systems subject to persistent disturbances via bilinear programming]]"
Relação: "[[1-202509171726 EXTENDED FARKAS' LEMMA]]"
Temas:
---
# CONCEITO

We can formulate a Linear Programming problem to check if a polyhedron is PI using the Extended Farkas' Lemma.

Consider now a controlled linear time-invariant (LTI) model:

$x_{k+1} = Ax_k + Bu_k$ 
$y_k = Cx_k$

The state constraint polyhedron can be defined as a set, such that  $\{x \in \mathbb{R}^{nx} : Xx \le \phi\}$, with $\phi > 0$ . 
note: If this polyhedron contains the origin we can normalize in a way that $\phi$ be a ones vector, which facilitates the implementation.

We can also have another set of constraints in the input, like {$u \in \mathbb{R}^{nu} : Uu \le \varphi$}.

To see if an polyhedron $L$ is PI and satisfact the constraints we need to ensure that

- L needs to be contractive-PI, what means $x_k \in L \to x_{k+1} \in \lambda L$ 
- X must contain L  $x_k \in L  \to x_k \in X$
- U must contain L $x_k \in L  \to x_k \in U$

We can verify if this conditions can be achieved  using the Extended Farkas' Lemma, turning this problem in a LP.

So, considering a SOF control $u_k = Ky_k = KCx_k$ and a closed loop system $x_{k+1} = (A + BKC)x_k$ we can say that L is PI if

