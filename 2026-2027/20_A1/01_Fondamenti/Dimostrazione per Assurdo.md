---
created: 2026-09-14
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/1
  - argomento/fondamenti
aliases: []
---
[[00_A1_Fondamenti|⬅️ Torna a Fondamenti]]

# Dimostrazione per Assurdo

Per dimostrare che $P \Rightarrow Q$ è vera assumiamo $P$ vera (l'ipotesi) e che la tesi $Q$ sia falsa (cioè che sia vera la sua negazione $\neg Q$). La negazione di $Q$, $\neg Q$, prende il nome di **ipotesi di assurdo**. Tramite dimostrazione diretta, assumendo vere $P$ e $\neg Q$, si vuole arrivare a dimostrare una **contraddizione**, cioè che una certa proposizione $S$ che sappiamo essere vera (falsa) deve anche essere falsa (vera):

$$
P \wedge \neg Q \text{ vera} \Rightarrow \text{contraddizione } (S \text{ vera} \wedge \neg S \text{ vera}) \Rightarrow P \wedge \neg Q \text{ falsa} \Rightarrow \neg Q \text{ falsa} \Rightarrow Q \text{ vera}
$$

(dove si usa che $P$ è vera per ipotesi).

**Teorema**: $\nexists\, r \in \mathbb{Q}$ tale che $r^2 = 2$.

*Dim.* Per assurdo $\exists r \in \mathbb{Q} : r^2 = 2$. $r \in \mathbb{Q} \Rightarrow r = \frac{m}{n}$ con $n,m \in \mathbb{Z}$, $n \neq 0$. Possiamo assumere $m,n \in \mathbb{N}$ e inoltre possiamo scegliere $m,n$ **relativamente primi**, cioè senza fattori primi in comune. Allora

$$
2 = r^2 = \frac{m^2}{n^2} \Rightarrow m^2 = 2n^2 \Rightarrow m^2 \text{ è pari} \Rightarrow m \text{ è pari (teorema precedente)} \Rightarrow m = 2k,\ k \in \mathbb{N}
$$

$$
\Rightarrow 2n^2 = m^2 = 4k^2 \Rightarrow n^2 = 2k^2 \Rightarrow n^2 \text{ è pari} \Rightarrow n \text{ è pari (teorema precedente)} \Rightarrow n = 2h,\ h \in \mathbb{N}
$$

Allora $m$ e $n$ sono entrambi pari, cioè entrambi divisibili per 2. **Assurdo**, perché per costruzione sono privi di fattori primi comuni. $\Rightarrow \nexists\, r \in \mathbb{Q} : r^2 = 2$. $\square$

---
Precedente: [[Metodi di Dimostrazione]] · Successivo: [[Dimostrazione per Induzione e Bernoulli]]
