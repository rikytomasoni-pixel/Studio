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

# Metodi di Dimostrazione

Un **teorema** è un asserto di cui si vuole dimostrare la verità, partendo da delle ipotesi. Le **ipotesi** sono una o più proposizioni (o predicati) $P$, la **tesi** è una o più proposizioni (o predicati) $Q$. Dimostrare il teorema significa provare che $P \Rightarrow Q$ è vera (o equivalentemente che $\neg Q \Rightarrow \neg P$ è vera). La **dimostrazione** è l'insieme di passaggi e deduzioni logiche che partono da $P$ vera e si concludono con $Q$ vera.

## Alcuni metodi di dimostrazione

### 1) Metodo deduttivo (dimostrazione diretta)

**Teorema**: $\forall n \in \mathbb{N}$, se $n$ è dispari allora $n^2$ è dispari. ($P(n)$: $n$ è dispari; $Q(n)$: $n^2$ è dispari.)

*Dim.* $n \in \mathbb{N}$ dispari $\Rightarrow$ $n = 2k+1$ per un (unico) $k \in \mathbb{N}$ $\Rightarrow$

$$
n^2 = (2k+1)^2 = 4k^2 + 4k + 1 = 2(2k^2 + 2k) + 1
$$

$\Rightarrow$ $n^2$ dispari. $\square$

### 2) Variante della dimostrazione diretta (contronominale)

$\neg Q \Rightarrow \neg P$ (equivale a $P \Rightarrow Q$).

**Teorema**: $\forall n \in \mathbb{N}$, se $n^2$ è pari allora $n$ è pari. ($P(n)$: $n^2$ è pari; $Q(n)$: $n$ è pari.)

*Dim.* Data la struttura logica di cui sopra, $\neg Q(n)$: «$n$ è dispari»; $\neg P(n)$: «$n^2$ è dispari». Pertanto $\forall n \in \mathbb{N}$, $\neg Q(n) \Rightarrow \neg P(n)$ diventa «$\forall n \in \mathbb{N}$, $n$ dispari implica $n^2$ dispari». Questa proposizione è vera per il teorema precedente. Quindi è vera anche $\forall n \in \mathbb{N}$, $P(n) \Rightarrow Q(n)$, che è il teorema in esame. $\square$

### 3) Controesempi

Mostrare che $P \Rightarrow Q$ è falsa significa mostrare che $P$ è vera e $Q$ è falsa, cioè che $P \wedge \neg Q$ è vera. Per una implicazione universale $\forall x \in A\ P(x) \Rightarrow Q(x)$, affermare che sia falsa vuol dire

$$
\exists x_0 \in A : \big(P(x_0) \Rightarrow Q(x_0)\big) \text{ sia falsa}, \quad \text{cioè} \quad \exists x_0 \in A : P(x_0) \wedge \neg Q(x_0) \text{ sia vera}
$$

$x_0$ prende il nome di **controesempio** all'implicazione universale e dimostra che essa è falsa.

*Esempio*. «$\forall n \in \mathbb{N}$, se $n$ è primo allora $n$ è dispari» è **falso**: un controesempio è $n = 2$, che è primo (soddisfa le ipotesi) ma è pari (nega la tesi).

---
Precedente: [[Condizioni Necessarie e Sufficienti]] · Successivo: [[Dimostrazione per Assurdo]]
