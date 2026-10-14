---
created: 2026-10-09
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Definizione di o-piccolo e Asintotico

Richiamo: date $a_n, b_n$ successioni ($b_n\neq 0$ definitivamente in $n\in\mathbb{N}$):
$$\lim_{n\to\infty}\dfrac{a_n}{b_n}=0 \ \Rightarrow\ a_n=o(b_n) \ \text{ per } n\to\infty \qquad \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \ \Rightarrow\ a_n\sim b_n$$
(vedi [[Ordini di Infinito e Infinitesimo]])

## Caratterizzazione dell'equivalenza asintotica

> [!abstract] Proposizione
> $$a_n\sim b_n \quad\Longleftrightarrow\quad a_n=b_n+o(b_n)$$

**dim:**
$$a_n\sim b_n \iff \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \iff \lim_{n\to\infty}\left(\dfrac{a_n}{b_n}-1\right)=0 \iff \lim_{n\to\infty}\dfrac{a_n-b_n}{b_n}=0 \iff a_n-b_n=o(b_n) \iff a_n=b_n+o(b_n)$$

**Oss:** $b_n=o(1)$ per $n\to\infty$ $\iff$ $\lim_{n\to\infty} b_n=0$ $\iff$ $b_n$ è infinitesima.

---
Precedente: [[Ordini di Infinito e Infinitesimo]] · Successivo: [[Relazione di Equivalenza Asintotica]]
