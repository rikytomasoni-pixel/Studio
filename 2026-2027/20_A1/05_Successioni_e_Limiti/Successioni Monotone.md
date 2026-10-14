---
created: 2026-09-30
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/successioni_e_limiti
aliases: []
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Successioni Monotone

**Definizione.** Una successione $a_n$ è:

| Tipo | Condizione ($\forall n$) | Equivalente |
|---|---|---|
| **crescente** | $a_n\le a_{n+1}$ | $m\le n\Rightarrow a_m\le a_n$ |
| **decrescente** | $a_n\ge a_{n+1}$ | $m\le n\Rightarrow a_m\ge a_n$ |
| **strettamente crescente** | $a_n<a_{n+1}$ | $m<n\Rightarrow a_m<a_n$ |
| **strettamente decrescente** | $a_n>a_{n+1}$ | $m<n\Rightarrow a_m>a_n$ |

Esempi: $a_n=2^n$ cresce; $a_n=\frac1{2^n}$ decresce.

> **Teorema (limite di successioni monotone e limitate).** Sia $a_n$ una successione **monotona e limitata**. Allora $\exists\lim a_n=\ell\in\mathbb{R}$. Inoltre:
> - se $a_n$ è **crescente**: $\lim a_n=\ell^-$ con $\ell=\sup_n a_n\in\mathbb{R}$;
> - se $a_n$ è **decrescente**: $\lim a_n=\ell^+$ con $\ell=\inf_n a_n\in\mathbb{R}$.

**Osservazione.** Se $a_n$ è crescente, basta chiedere che sia limitata dall'alto (dal basso lo è automaticamente: $a_n\ge a_0$). Se è decrescente, basta chiedere che sia limitata dal basso.

**Dimostrazione** (solo il caso crescente e limitata; il decrescente è analogo). Sia $\ell=\sup_{n}a_n$. Esso esiste grazie all'**assioma dell'estremo superiore** che $\mathbb{R}$ soddisfa (e $\mathbb{Q}$ no, cfr. [[2026-09-16 A1 Lezione 2|completezza]]); poiché $a_n$ è limitata dall'alto, $\ell\in\mathbb{R}$. Per definizione di estremo superiore:

1. $a_n\le\ell$ $\forall n$ ($\ell$ è maggiorante);
2. $\forall\varepsilon>0\ \exists n_0$ tale che $\ell-\varepsilon<a_{n_0}\le\ell$ ($\ell-\varepsilon$ non è maggiorante);
3. poiché $a_n$ è crescente, $\forall n\ge n_0$: $a_n\ge a_{n_0}$.

Dunque $\forall\varepsilon>0\ \exists n_0$ tale che $\forall n\ge n_0$:
$$\ell-\varepsilon<a_{n_0}\le a_n\le\ell,$$
cioè, per definizione, $\lim a_n=\ell^-$ con $\ell=\sup a_n$. $\square$

![[successione-crescente-limitata-sup.png]]

**Osservazione.** Questo teorema si appoggia sull'assioma dell'estremo superiore, che $\mathbb{R}$ soddisfa e $\mathbb{Q}$ no.

> **Teorema (limite delle successioni monotone, caso generale).** Sia $a_n$ una successione monotona. Allora ammette limite: $\exists\lim a_n=\ell\in\overline{\mathbb{R}}$.
> - Se $a_n$ cresce: $\lim a_n=\ell^-$ con $\ell=\sup_n a_n\in\mathbb{R}\cup\{+\infty\}$.
> - Se $a_n$ decresce: $\lim a_n=\ell^+$ con $\ell=\inf_n a_n\in\mathbb{R}\cup\{-\infty\}$.

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ **regolare**.

---
Precedente: [[Limiti Infiniti e Regolarità]] · Successivo: [[Teorema sulle Successioni Monotone]]
