---
ID: "202609091838"
tags:
  - 1-202609091838
Referência:
Pag. de Ref:
Relação:
Temas: "[[1 - ENGENHARIA]]"
---
# NOTA
Considerando que $h[n]$ caracteriza um sistema. Para $x[n]$ = $e^{j\omega _0 n}$ (entrada de frequência única) $y[n] = (h*x)[n]$ , que é equivalente a:

$\sum_{k=-\infty}^{\infty}h[k]e^{j\omega _0(n-k)} =\sum_{k=-\infty}^{\infty}h[k] e^{j\omega _0 n}e^{j\omega _0 -k}$

Mas como $e^{j\omega _0 n}$ é a nossa entrada, isso implica que:

$y[n] = x[n] \sum_{k=-\infty}^{\infty}h[k] e^{j\omega _0 -k}$

Onde o resultado desse somatório é um número complexo que pode alterar a fase e a magnitude de $x[n]$. 

Dessa forma se a saída de um sistema tem frequências que não tinham na entrada (isso pode ser verificado olhando o espectro) ele não é LIT.



