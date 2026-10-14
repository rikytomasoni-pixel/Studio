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

# Teorema sulle Successioni Monotone

## Versione generale: successioni monotone non necessariamente limitate

> [!abstract] Teorema
> Sia $a_n$ una successione monotona. Allora $a_n$ ammette limite, cioè $\exists\, \lim_{n\to\infty} a_n = l\in\overline{\mathbb{R}}$.
>
> - se $a_n$ cresce, allora $\lim_{n\to\infty} a_n = l^-$, con $l=\sup_{n\in\mathbb{N}} a_n \in\overline{\mathbb{R}}$
> - se $a_n$ decresce, allora $\lim_{n\to\infty} a_n = l^+$, con $l=\inf_{n\in\mathbb{N}} a_n \in\overline{\mathbb{R}}$

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ regolare.

**Dimostrazione.**

**1) Caso $a_n$ limitata.** In questo caso il teorema precedente permette di concludere direttamente: $\exists\, l\in\mathbb{R}$ tale che $\lim a_n=l$, con le stesse conclusioni viste sopra.

**2) Caso $a_n$ illimitata.** Per fissare le idee, supponiamo $a_n$ crescente (se $a_n$ è decrescente la dimostrazione è analoga).

Perché $a_n$ crescente, $a_0\leq a_n\ \ \forall\, n\in\mathbb{N}$ ($a_n$ è limitata dal basso). Quindi $a_n$ deve essere illimitata dall'alto. In particolare
$$\sup_{n\in\mathbb{N}} a_n = +\infty$$
per definizione.

Quindi $\forall\, M>0\ \exists\, n_0\in\mathbb{N}$ tale che $a_{n_0}>M$. Perché $a_n$ crescente, $\forall\, n\geq n_0$ segue che $a_n\geq a_{n_0}$.

Quindi
$$\forall\, M>0\ \exists\, n_0\in\mathbb{N} \text{ tale che } \forall\, n\geq n_0 \quad a_n\geq a_{n_0}>M$$
$$\Rightarrow \quad \forall\, M>0\ \exists\, n_0\in\mathbb{N} : \forall\, n\geq n_0 \quad a_n>M$$

che è la definizione di $\lim_{n\to\infty} a_n = +\infty$, con $\sup a_n = +\infty$. $\blacksquare$

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ regolare, ma non vale il viceversa: $a_n$ regolare $\not\Rightarrow$ $a_n$ monotona.

Ad esempio $a_n = \dfrac{(-1)^n}{n}$ è un controesempio: infatti $a_n$ non è monotona e $\lim_{n\to\infty} a_n = 0$.

---
Precedente: [[Successioni Monotone]] · Successivo: [[Convergente implica Limitata]]
