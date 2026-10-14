---
created: 2026-10-09
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/forme_indeterminate_e_asintotici
aliases: []
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Definizione di o-piccolo e Asintotico

Date $a_n,b_n$ successioni ($b_n\neq0$ definitivamente in $n\in\mathbb{N}$):

- se $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=0$ scriviamo $a_n=o(b_n)$ ("**$a_n$ è o-piccolo di $b_n$**");
- se $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=1$ scriviamo $a_n\sim b_n$ ("**$a_n$ è asintotico a $b_n$**").

### Caratterizzazione
$$a_n\sim b_n\iff a_n=b_n+o(b_n).$$

Infatti
$$a_n\sim b_n\iff\lim\frac{a_n}{b_n}=1\iff\lim\left(\frac{a_n}{b_n}-1\right)=0\iff\lim\frac{a_n-b_n}{b_n}=0\iff a_n-b_n=o(b_n)\iff a_n=b_n+o(b_n).$$

**Osservazione.** $b_n=o(1)$ per definizione: $\lim\frac{b_n}1=0$, cioè $\lim b_n=0$, cioè $b_n$ è **infinitesima**.

---
Precedente: [[Ordini di Infinito e Infinitesimo]] · Successivo: [[Relazione di Equivalenza Asintotica]]
