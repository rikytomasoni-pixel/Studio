---
created: 2026-10-07
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Aritmetizzazione dell'Infinito e Forme di Indeterminazione

> [!abstract] Teorema — Aritmetizzazione parziale di $\overline{\mathbb{R}}$
> Siano $a_n, b_n$ successioni.
>
> **1)** Se $\lim_{n\to\infty} a_n = l \in\mathbb{R}$, $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} (a_n+b_n) = \pm\infty \qquad (l+(\pm\infty) = \pm\infty, \ \forall\, l\in\mathbb{R})$$
>
> **2)** Se $\lim_{n\to\infty} a_n = +\infty$, $\lim_{n\to\infty} b_n = +\infty$ (concordi in segno), allora
> $$\lim_{n\to\infty} (a_n+b_n) = +\infty$$
> (stesso segno: $(+\infty)+(+\infty)=+\infty$, $(-\infty)+(-\infty)=-\infty$)
>
> **3)** Se $\lim_{n\to\infty} a_n = l \in\mathbb{R}\setminus\{0\}$, $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} a_n b_n = \pm\infty$$
> con l'usuale regola del prodotto dei segni:
> $$l>0,\ \lim b_n=+\infty \ \Rightarrow\ \lim a_n b_n = +\infty$$
> $$l>0,\ \lim b_n=-\infty \ \Rightarrow\ \lim a_n b_n = -\infty \quad \text{(altrimenti con regola dei segni per } l<0\text{)}$$
>
> **4)** Se $\lim_{n\to\infty} a_n = a\in\mathbb{R}\setminus\{0\}$ e $\lim_{n\to\infty} b_n = 0^{\pm}$ ($b_n\neq 0$ definitivamente), allora
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = \pm\infty$$
> con l'usuale regola del prodotto dei segni: $a>0$ e $\lim b_n=0^+$ $\Rightarrow$ $\lim \dfrac{a_n}{b_n}=+\infty$; $a<0$ e $\lim b_n=0^+$ $\Rightarrow$ $\lim \dfrac{a_n}{b_n}=-\infty$ (altrimenti con regola dei segni).
>
> **5)** Se $\lim_{n\to\infty} a_n = a\in\mathbb{R}$, $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 0 \qquad \forall\, a\in\mathbb{R}$$

**Osservazione.** $0\cdot\infty$, $\infty-\infty$, $\dfrac{\infty}{\infty}$, $\dfrac{0}{0}$ sono **forme di indeterminazione**: nulla si può dire in generale.

**Esempi di forme indeterminate.**
$$a_n = n, \quad b_n = \dfrac{1}{n} \ \Rightarrow\ a_n\cdot b_n = 1 \to 1 \qquad [0\cdot\infty]$$
$$a_n = n, \quad b_n = n^2 \ \Rightarrow\ a_n - b_n = n-n^2 \to -\infty \qquad [\infty-\infty]$$
$$a_n = n, \quad b_n = n^2+n \ \Rightarrow\ a_n - b_n = -n^2 \to -\infty \qquad [\infty-\infty]$$
$$a_n = n+(-1)^n, \quad b_n = n \ \Rightarrow\ a_n - b_n = (-1)^n \text{ non ha limite} \qquad [\infty-\infty]$$

---
Precedente: [[Rapporti di Somme di Potenze]] · Successivo: [[Tecniche per le Forme Infinito meno Infinito]]
