---
created: 2026-10-02
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/successioni_e_limiti
aliases: []
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Convergente implica Limitata

> **Teorema.** Se $a_n$ è convergente, cioè $\exists\ell=\lim a_n\in\mathbb{R}$, allora $a_n$ è **limitata**.

Il viceversa è **falso**: $a_n=(-1)^n$ è irregolare ma limitata.

**Dimostrazione.** Poiché $\ell=\lim a_n\in\mathbb{R}$, $\forall\varepsilon>0\ \exists N$ tale che $\forall n\ge N$: $\ell-\varepsilon<a_n<\ell+\varepsilon$. Scegliendo $\varepsilon=1$: $\exists N$ tale che $\forall n\ge N$ $\ \ell-1<a_n<\ell+1$. Siano
$$M=\max\{a_0,a_1,\dots,a_N\},\qquad m=\min\{a_0,a_1,\dots,a_N\},$$
che esistono in $\mathbb{R}$ perché $\{a_0,\dots,a_N\}$ è un insieme **finito e non vuoto**. Posti
$$L=\max\{M,\ell+1\},\qquad P=\min\{m,\ell-1\},$$
vale $P\le a_n\le L$ per ogni $n\in\mathbb{N}$: quindi $a_n$ è limitata. $\square$

![[convergente-implica-limitata.png]]

---
Precedente: [[Teorema sulle Successioni Monotone]] · Successivo: [[Potenze e Progressione Geometrica]]
