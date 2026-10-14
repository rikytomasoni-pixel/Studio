---
created: 2026-09-30
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/successioni_e_limiti
aliases: []
origine: UpdateVault
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Successioni Monotone

> [!warning] Definizione — Successione monotona
> Una successione $a_n$ si dice **monotona**:
> - **crescente** se $a_n \leq a_m \ \ \forall\, n<m$ ($n,m\in\mathbb{N}$)
> - **decrescente** se $a_n \geq a_m \ \ \forall\, n<m$
> - **strettamente crescente** se $a_n < a_m \ \ \forall\, n<m$
> - **strettamente decrescente** se $a_n > a_m \ \ \forall\, n<m$

**Esempi.** $a_n=n$ cresce; $a_n=\dfrac{1}{n}$ decresce.

## Teorema sul limite di successioni monotone e limitate

> [!abstract] Teorema
> Sia $a_n$ una successione monotona e limitata. Allora $\exists\, \lim_{n\to\infty} a_n = l\in\mathbb{R}$.
>
> Inoltre:
> - se $a_n$ è **crescente**: $\lim_{n\to\infty} a_n = l^-$, con $l=\sup_{n\in\mathbb{N}} a_n \in\mathbb{R}$
> - se $a_n$ è **decrescente**: $\lim_{n\to\infty} a_n = l^+$, con $l=\inf_{n\in\mathbb{N}} a_n \in\mathbb{R}$

**Osservazione.** Se $a_n$ crescente, basta chiedere $a_n$ limitata dall'alto. Se $a_n$ decrescente, basta chiedere $a_n$ limitata dal basso (dall'altro lato lo sono automaticamente).

**Dimostrazione.** Solo il caso $a_n$ limitata crescente (il caso decrescente è analogo).

Perché $a_n$ crescente, $a_n$ è automaticamente limitata dal basso: $a_0\leq a_n \ \ \forall\, n\in\mathbb{N}$.

Sia $l=\displaystyle\sup_{n\in\mathbb{N}} a_n \in \mathbb{R}\cup\{+\infty\}$. Esso esiste grazie all'assioma dell'estremo superiore, che $\mathbb{R}$ soddisfa.

Perché per ipotesi $a_n$ è limitata dall'alto, deve essere $l=\sup a_n\in\mathbb{R}$ ($l$ è un maggiorante di $\{a_n\}$).

Per definizione di estremo superiore:

① $l$ è maggiorante di $\{a_n\}$: $a_n\leq l \ \ \forall\, n\in\mathbb{N}$

② $\forall\, \varepsilon>0\ \exists\, N_0\in\mathbb{N}$ tale che $l-\varepsilon<a_{N_0}\leq l$ ($l-\varepsilon$ non è maggiorante)

Perché $a_n$ crescente, $\forall\, n\geq N_0$ $a_n\geq a_{N_0}$ ③

Segue, da ②③, che
$$\forall\, \varepsilon>0\ \exists\, N_0\in\mathbb{N} \text{ tale che } l-\varepsilon<a_{N_0}\leq a_n \leq l \qquad \forall\, n\geq N_0$$

$$\Rightarrow \quad \forall\, \varepsilon>0\ \exists\, N_0\in\mathbb{N} : \forall\, n\geq N_0 \quad l-\varepsilon<a_n\leq l$$

$$\Rightarrow \quad \text{per definizione} \quad \lim_{n\to\infty} a_n = l^-, \quad l=\sup_{n\in\mathbb{N}} a_n \qquad \blacksquare$$

![[successione-crescente-limitata-sup.png]]

**Osservazione.** Questo teorema si poggia sull'assioma dell'estremo superiore, che $\mathbb{R}$ soddisfa (e $\mathbb{Q}$ no).

---
Precedente: [[Limiti Infiniti e Regolarità]] · Successivo: [[Teorema sulle Successioni Monotone]]
