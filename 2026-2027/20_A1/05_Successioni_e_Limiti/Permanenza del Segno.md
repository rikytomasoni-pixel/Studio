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

# Permanenza del Segno

> **Teorema (permanenza del segno).**
> 1. Data $a_n$, se esiste $\lim a_n=\ell\in\overline{\mathbb{R}}$ e $\ell>0$ (cioè $\ell\in(0,+\infty]$), allora $a_n>0$ **definitivamente** in $n\in\mathbb{N}$. Similmente se $\ell<0$ ($\ell\in[-\infty,0)$) allora $a_n<0$ definitivamente.
> 2. Se esiste $\ell=\lim a_n\in\overline{\mathbb{R}}$ e $a_n\ge0$ definitivamente, allora $\ell\ge0$ ($\ell\in[0,+\infty]$). Similmente, se $a_n\le0$ definitivamente, allora $\ell\le0$.

**Osservazioni.**
- Può essere $\ell=\lim a_n\ge0$ e $a_n<0$: ad esempio $a_n=-\frac1n$ soddisfa $a_n<0\ \forall n\ge1$ e $\lim a_n\ge0$.
- Se $a_n>0$ ed esiste $\lim a_n=\ell$, allora $\ell\ge0$ ma può essere $\ell=0$: ad esempio $a_n=\frac1n>0$ e $\lim a_n=0$.

**Dimostrazione.**

*1)* Sia $\ell=\lim a_n\in(0,\infty]$. Se $\ell=+\infty$, per definizione $\forall M>0\ \exists N$ tale che $\forall n\ge N$ $a_n>M>0$, quindi $a_n>0$ definitivamente. Se $\ell\in(0,+\infty)$, per definizione $\forall\varepsilon>0\ \exists N$: $\forall n\ge N$ $\ell-\varepsilon<a_n<\ell+\varepsilon$. Si sceglie $\varepsilon=\frac\ell2>0$:
$$a_n>\ell-\varepsilon=\frac\ell2>0\quad\Rightarrow\quad a_n>0\ \text{definitivamente}.$$
Similmente se $\ell<0$.

![[permanenza-del-segno-striscia.png]]

*2)* Sia $a_n\ge0$ definitivamente ed esista $\ell=\lim a_n\in\overline{\mathbb{R}}$. Vogliamo provare $\ell\ge0$. Per assurdo sia $\ell<0$: per la parte 1 sarebbe $a_n<0$ definitivamente. **Assurdo**, perché dovrebbe essere $a_n\ge0$ e $a_n<0$ definitivamente. Quindi $\ell\ge0$. Similmente se $a_n\le0$. $\square$

---
Precedente: [[Potenze e Progressione Geometrica]] · Successivo: [[Algebra dei Limiti]]
