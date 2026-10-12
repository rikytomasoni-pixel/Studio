---
tags:
  - AM1
  - teoremi
  - dimostrazioni
  - controesempi
data: 2026-09-14
fonte: Lezione 1
---

# Teoremi, Dimostrazioni e Controesempi

Un **teorema** è un asserto di cui si vuole dimostrare la verità, partendo da delle ipotesi. Le **ipotesi** sono una o più proposizioni o predicati $P$, la **tesi** è una proposizione o predicato $Q$. Dimostrare il teorema significa provare che $P \Rightarrow Q$ è vera, oppure che $\neg Q \Rightarrow \neg P$ è vera.

La **dimostrazione** è l'insieme di passaggi e deduzioni logiche che partono da $P$ vera e si concludono con $Q$ vera.

Metodi di dimostrazione: diretta (qui sotto), [[04_Dimostrazione_per_Assurdo]], [[05_Dimostrazione_per_Induzione]].

## 1. Metodo deduttivo (dimostrazione diretta)

> [!theorem]
> $\forall m \in \mathbb{N}$, se $m$ è dispari allora $m^2$ è dispari.

$$\forall m \in \mathbb{N} \quad P(m) \Rightarrow Q(m)$$

- $P(m)$: $m$ è dispari
- $Q(m)$: $m^2$ è dispari

**Dimostrazione.** Sia $m \in \mathbb{N}$ dispari. Allora $m = 2k+1$ per un (unico) $k \in \mathbb{N}$.

$$m^2 = (2k+1)^2 = 4k^2 + 4k + 1 = 2(2k^2+2k) + 1$$

Quindi $m^2 = 2a+1$ con $a = 2k^2+2k$, cioè $m^2$ è dispari. $\blacksquare$

## 2. Variante di dimostrazione diretta (contronominale)

$\neg Q \Rightarrow \neg P$ (equivale a $P \Rightarrow Q$)

> [!theorem]
> $\forall m \in \mathbb{N}$, se $m^2$ è pari allora $m$ è pari.

- $P(m)$: $m^2$ è pari
- $Q(m)$: $m$ è pari

**Dimostrazione.** Data la struttura logica soprastante:

- $\neg Q(m)$: $m$ è dispari
- $\neg P(m)$: $m^2$ è dispari

Pertanto $\forall m \in \mathbb{N}$, $\neg Q(m) \Rightarrow \neg P(m)$, che diventa: se $m$ è dispari allora $m^2$ è dispari — vera per il teorema precedente.

Quindi, se $\neg Q(m) \Rightarrow \neg P(m)$ è vera, lo è anche la sua equivalente $P(m) \Rightarrow Q(m)$. $\blacksquare$

## 3. Controesempio

Mostrare che $P \Rightarrow Q$ è falsa significa mostrare che $P$ è vera e $Q$ è falsa, cioè che $P \land \neg Q$ è vera.

Per un'implicazione universale $\forall x \in A,\ P(x) \Rightarrow Q(x)$, affermare che sia falsa vuol dire:

$$\exists\, x_0 \in A : P(x_0) \Rightarrow Q(x_0) \text{ sia falsa} \quad \Longleftrightarrow \quad \exists\, x_0 \in A : P(x_0) \land \neg Q(x_0) \text{ sia vera}$$

$x_0$ prende il nome di **controesempio** dell'implicazione universale $\forall x \in A,\ P(x) \Rightarrow Q(x)$, e dimostra che essa è falsa.

> [!theorem]
> $\forall m \in \mathbb{N}$, se $m$ è primo allora $m$ è dispari.

Questo teorema è **falso**: un controesempio (unico, in questo caso) è $m=2$, che è primo (ipotesi soddisfatta) ma è anche pari (tesi negata). $\blacksquare$

### Note collegate
- [[00_MOC_A1]]
- [[02_Logica]] — implicazione universale, condizioni necessarie e sufficienti
- [[04_Dimostrazione_per_Assurdo]]
- [[05_Dimostrazione_per_Induzione]]