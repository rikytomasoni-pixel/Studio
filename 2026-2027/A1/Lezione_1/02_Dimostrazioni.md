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

Un **teorema** è un asserto di cui si vuole dimostrare la verità, partendo da delle ipotesi. Le **ipotesi** sono una o più proposizioni o predicati $P$, la **tesi** è una o più proposizioni o predicati $Q$. Dimostrare il teorema significa provare che $P \Rightarrow Q$ è vera, oppure che $\neg Q \Rightarrow \neg P$ è vera.

La **dimostrazione** è l'insieme di passaggi e deduzioni logiche che partono da $P$ vera e si concludono con $Q$ vera.

Metodi di dimostrazione: diretta (qui sotto), [[03_Dimostrazione_per_Assurdo]], [[04_Dimostrazione_per_Induzione]].

## 1. Metodo deduttivo (dimostrazione diretta)

> [!theorem]
> $\forall n \in \mathbb{N}$, se $n$ è dispari allora $n^2$ è dispari.

$$\forall n \in \mathbb{N} \quad P(n) \Rightarrow Q(n)$$

- $P(n)$: $n$ è dispari
- $Q(n)$: $n^2$ è dispari

**Dimostrazione.** Sia $n \in \mathbb{N}$ dispari. Allora $n = 2k+1$ per un (unico) $k \in \mathbb{N}$.

$$n^2 = (2k+1)^2 = 4k^2 + 4k + 1 = 2(2k^2+2k) + 1$$

Quindi $n^2$ è dispari. $\blacksquare$

## 2. Variante di dimostrazione diretta (contronominale)

$\neg Q \Rightarrow \neg P$ (equivale a $P \Rightarrow Q$)

> [!theorem]
> $\forall n \in \mathbb{N}$, se $n^2$ è pari allora $n$ è pari.

- $P(n)$: $n^2$ è pari
- $Q(n)$: $n$ è pari

**Dimostrazione.** Data la struttura logica soprastante:

- $\neg Q(n)$: $n$ è dispari
- $\neg P(n)$: $n^2$ è dispari

Pertanto $\forall n \in \mathbb{N}$, $\neg Q(n) \Rightarrow \neg P(n)$, che diventa: se $n$ è dispari allora $n^2$ è dispari — vera per il teorema precedente.

Quindi, se $\neg Q(n) \Rightarrow \neg P(n)$ è vera, lo è anche la sua equivalente $P(n) \Rightarrow Q(n)$. $\blacksquare$

## 3. Controesempio

Mostrare che $P \Rightarrow Q$ è falsa significa mostrare che $P$ è vera e $Q$ è falsa, cioè che $P \land \neg Q$ è vera.

Per un'implicazione universale $\forall x \in A,\ P(x) \Rightarrow Q(x)$, affermare che sia falsa vuol dire:

$$\exists\, x_0 \in A : P(x_0) \Rightarrow Q(x_0) \text{ sia falsa} \quad \Longleftrightarrow \quad \exists\, x_0 \in A : P(x_0) \land \neg Q(x_0) \text{ sia vera}$$

$x_0$ prende il nome di **controesempio** dell'implicazione universale $\forall x \in A,\ P(x) \Rightarrow Q(x)$, e dimostra che essa è falsa.

> [!theorem]
> $\forall n \in \mathbb{N}$, se $n$ è primo allora $n$ è dispari.

Questo teorema è **falso**: un controesempio è $n=2$, che è primo (ipotesi soddisfatta) ma è anche pari (tesi negata). $\blacksquare$

> [!warning] Aggiunte presenti nella versione precedente ma non nel PDF manoscritto
> - Dimostrazione diretta: "$m^2 = 2a+1$ con $a = 2k^2+2k$, cioè $m^2$ è dispari" (passaggio esplicito finale).
> - Controesempio: $n=2$ è l'unico controesempio possibile (osservazione vera, assente nel PDF).
> - Etichetta "(contronominale)" per la variante di dimostrazione diretta.

### Note collegate
- [[00_MOC_A1]]
- [[01_Logica]] — implicazione universale, condizioni necessarie e sufficienti
- [[03_Dimostrazione_per_Assurdo]]
- [[04_Dimostrazione_per_Induzione]]