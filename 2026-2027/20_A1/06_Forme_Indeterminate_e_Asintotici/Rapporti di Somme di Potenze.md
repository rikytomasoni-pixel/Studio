---
created: 2026-10-07
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Rapporti di Somme di Potenze

**Esempio 1.**
$$a_n=\frac{3n^5-4n^3+\log n-8\arctan(n^2+1)-3}{2n^{16/3}+147\log n^{52}-\sin n}$$
Si raccoglie la potenza dominante a numeratore e a denominatore:
$$a_n=\frac{n^5\left(3-\frac4{n^2}+\frac{\log n}{n^5}-8\frac{\arctan(n^2+1)}{n^5}-\frac3{n^5}\right)}{n^{16/3}\left(2+147\cdot52\frac{\log n}{n^{16/3}}-\frac{\sin n}{n^{16/3}}\right)}=\frac1{n^{1/3}}\cdot\frac{3+\dots}{2+\dots}$$
dove tutti i termini «$\dots$» tendono a $0$ (per la [[2026-10-02 A1 Lezione 7|gerarchia degli infiniti]] e perché $\arctan$ e $\sin$ sono limitate). Quindi
$$a_n\to0\cdot\frac{3+0}{2+0}=0\ \Rightarrow\ \lim a_n=0.$$

**Osservazione generale.** Sia $a_n=\dfrac{P(n)}{Q(n)}$ con $P,Q$ somme di potenze di $n$ e di funzioni limitate in $n$ (oppure «trascurabili» rispetto a potenze di $n$). Siano $p$ e $q$ le massime potenze (positive) di $n$ in $P$ e $Q$, con coefficienti $c_P$ e $c_Q$. Allora:

| Caso | $\displaystyle\lim\frac{P(n)}{Q(n)}$ |
|---|---|
| $p<q$ | $0$ |
| $p=q$ | $\ell=\dfrac{c_P}{c_Q}\in\mathbb{R}\setminus\{0\}$ |
| $p>q$ | $\pm\infty$ (segno dato dal prodotto dei segni di $c_P$ e $c_Q$) |

**Esempio 2** ($p=q$).
$$a_n=\frac{2n^5-47n^4+\log\log n+\cos n}{5n^5+\arctan\sqrt n+(\log n)^{42}-1}=1\cdot\frac{2+\dots}{5+\dots}\to\frac25.$$
Qui si usa $\dfrac{(\log n)^{42}}{n^5}=\left(\dfrac{\log n}{n^{5/42}}\right)^{42}\to0$.

**Esempio 3** ($p>q$).
$$\lim\frac{18n^3-n^{3/2}+\sin n+\log\log n}{-2n^2+n^{3/4}-(\log n)^{18}+7}=\lim n\cdot\frac{18+\dots}{-2+\dots}=+\infty\cdot(-9)=-\infty.$$

**Esempio 4** (gerarchia).
$$\lim\frac{7\cdot2^n+\log\log n-\arctan n+n^7}{14\,n!-n^{42}+\sin n}=\lim\frac{2^n}{n!}\cdot\frac{7+\dots}{14+\dots}=0\cdot\frac7{14}=0.$$

---
Successivo: [[Aritmetizzazione dell'Infinito e Forme di Indeterminazione]]
