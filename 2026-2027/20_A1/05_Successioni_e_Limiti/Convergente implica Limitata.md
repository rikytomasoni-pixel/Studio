---
created: 2026-10-02
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/successioni_e_limiti
aliases: []
origine: UpdateVault
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Convergente implica Limitata

> [!abstract] Teorema
> Data una successione $a_n$ convergente, cioè $\exists\, l=\lim_{n\to\infty} a_n \in\mathbb{R}$, allora $a_n$ è limitata.

**Osservazione.** Il viceversa non vale: $a_n$ limitata $\not\Rightarrow$ $\exists\, \lim_{n\to\infty} a_n = l\in\mathbb{R}$.

Ad esempio $a_n=(-1)^n$ è irregolare, ma è limitata.

**Dimostrazione.** Perché $l=\lim_{n\to\infty} a_n\in\mathbb{R}$ esiste, per definizione
$$\forall\, \varepsilon>0\ \exists\, N\in\mathbb{N} \text{ tale che } \forall\, n\geq N \quad l-\varepsilon<a_n<l+\varepsilon$$

Scegliendo $\varepsilon=1$: $\exists\, N\in\mathbb{N}$ tale che $\forall\, n\geq N$
$$l-1<a_n<l+1$$

Siano
$$M = \max\{a_0,a_1,a_2,\dots,a_N\}, \qquad m = \min\{a_0,a_1,a_2,\dots,a_N\}$$
Essi esistono (massimo e minimo) perché $\{a_0,a_1,\dots,a_N\}$ è un insieme finito e non vuoto di valori.

Siano
$$L = \max\{M, l+1\} \in\mathbb{R}, \qquad P = \min\{m, l-1\} \in\mathbb{R}$$

allora $\forall\, n\in\mathbb{N}$
$$P \leq a_n \leq L$$

![[convergente-implica-limitata.png]]

Quindi $a_n$ è limitata. $\blacksquare$

---
Precedente: [[Teorema sulle Successioni Monotone]] · Successivo: [[Potenze e Progressione Geometrica]]
