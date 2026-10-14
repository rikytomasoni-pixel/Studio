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

# Teorema sulle Successioni Monotone

> **Teorema (sul limite delle successioni monotone).** Sia $a_n$ monotona. Allora ammette limite: $\exists\lim_{n\to\infty}a_n=\ell\in\overline{\mathbb{R}}$.
> - Se $a_n$ cresce: $\lim a_n=\ell^-$ con $\ell=\sup_n a_n\in\mathbb{R}\cup\{+\infty\}$.
> - Se $a_n$ decresce: $\lim a_n=\ell^+$ con $\ell=\inf_n a_n\in\mathbb{R}\cup\{-\infty\}$.

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ regolare.

**Dimostrazione.**

*1) Caso $a_n$ limitata.* Per il teorema sul limite di successioni monotone e limitate (già visto) $\exists\ell\in\mathbb{R}$ con $\lim a_n=\ell$; se crescente $\lim a_n=\ell^-$, $\ell=\sup a_n$; se decrescente $\lim a_n=\ell^+$, $\ell=\inf a_n$.

*2) Caso $a_n$ illimitata.* Per semplicità sia $a_n$ crescente (il decrescente è analogo). Poiché $a_n$ è crescente, $\forall n\ge0$ si ha $a_n\ge a_0$, cioè è limitata dal basso. Quindi deve essere illimitata dall'alto, e per definizione $\sup_{n\in\mathbb{N}}a_n=+\infty$. Dunque $\forall M>0\ \exists n_0\in\mathbb{N}$ tale che $a_{n_0}>M$. Poiché $a_n$ è crescente, $\forall n\ge n_0$: $a_n\ge a_{n_0}>M$. Segue che $\forall M>0\ \exists n_0$ tale che $\forall n\ge n_0$ $a_n>M$, cioè $\lim a_n=+\infty$ con $\sup a_n=+\infty$. $\square$

**Osservazioni.**
- $a_n$ monotona $\Rightarrow$ $a_n$ regolare;
- $a_n$ regolare $\not\Rightarrow$ $a_n$ monotona. Controesempio: $a_n=\dfrac{(-1)^n}{n}$ non è monotona e $\lim\dfrac{(-1)^n}n=0$.

---
Precedente: [[Successioni Monotone]] · Successivo: [[Convergente implica Limitata]]
