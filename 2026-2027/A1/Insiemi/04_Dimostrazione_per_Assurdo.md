---
tags:
  - AM1
  - dimostrazioni
  - assurdo
data: 2026-09-14
fonte: Lezione 1
---

# Dimostrazione per assurdo

Per dimostrare $P \Rightarrow Q$ vera, assumiamo $P$ vera (l'ipotesi) e $Q$ (la tesi) falsa, cioè che la sua negazione $\neg Q$ sia vera. La negazione di $Q$ prende il nome di **ipotesi d'assurdo**.

Tramite dimostrazione diretta, assumendo vere $P$ e $\neg Q$, si vuole arrivare a dimostrare una contraddizione, cioè che una proposizione $S$ che sappiamo essere vera (falsa) deve essere anche falsa (vera):

$$P \land \neg Q \text{ vera} \;\Rightarrow\; \text{contraddizione}\ (S \text{ vera} \land \neg S \text{ vera}) \;\Rightarrow\; P \land \neg Q \text{ falsa} \;\Rightarrow\; \neg Q \text{ falsa} \;\Rightarrow\; Q \text{ vera}$$

> [!theorem]
> $$\nexists\, x \in \mathbb{Q} : x^2 = 2$$

**Dimostrazione (per assurdo).** Supponiamo $\exists\, x \in \mathbb{Q} : x^2 = 2$.

$x \in \mathbb{Q} \Rightarrow x = \dfrac{m}{n}$ con $m, n \in \mathbb{Z}$, $n \neq 0$.

Possiamo assumere $m, n \in \mathbb{N}$ e, inoltre, scegliere $m, n$ relativamente primi (senza fattori primi in comune).

$$2 = x^2 = \frac{m^2}{n^2} \;\Rightarrow\; 2n^2 = m^2 \;\Rightarrow\; m^2 \text{ è pari} \;\Rightarrow\; m \text{ è pari (teorema precedente)}$$

$$m = 2k \text{ per un (unico) } k \in \mathbb{N} \;\Rightarrow\; 2n^2 = m^2 = 4k^2 \;\Rightarrow\; n^2 = 2k^2$$

$$n^2 \text{ è pari} \;\Rightarrow\; n \text{ è pari} \;\Rightarrow\; n = 2h \text{ per un (unico) } h \in \mathbb{N}$$

Allora $m$ e $n$ sono entrambi pari, cioè divisibili per 2. **Assurdo**, perché per costruzione $m$ ed $n$ non hanno fattori comuni.

$$\Rightarrow \nexists\, x \in \mathbb{Q} : x^2 = 2 \qquad \blacksquare$$

### Note collegate
- [[00_MOC_A1]]
- [[03_Dimostrazioni]] — teorema "se $m^2$ è pari allora $m$ è pari" (contronominale)
- [[01_Insiemi_Numerici]] — $\mathbb{Q}$ e numeri irrazionali
- [[08_Estremo_Superiore_Inferiore]] — $\mathbb{Q}$ non soddisfa la proprietà dell'estremo superiore
- [[10_Retta_Reale_Intervalli]] — punti della retta a cui non corrisponde alcun razionale