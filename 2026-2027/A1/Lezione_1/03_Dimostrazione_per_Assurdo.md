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

dove nel passaggio $P \land \neg Q$ falsa $\Rightarrow \neg Q$ falsa si usa che $P$ è vera (ipotesi).

> [!theorem]
> $$\nexists\, r \in \mathbb{Q} : r^2 = 2$$

**Dimostrazione (per assurdo).** Supponiamo $\exists\, r \in \mathbb{Q} : r^2 = 2$.

$r \in \mathbb{Q} \Rightarrow r = \dfrac{m}{n}$ con $m, n \in \mathbb{Z}$, $n \neq 0$.

Possiamo assumere $m, n \in \mathbb{N}$ e, inoltre, scegliere $m, n$ relativamente primi (senza fattori primi in comune).

$$2 = r^2 = \frac{m^2}{n^2} \;\Rightarrow\; 2n^2 = m^2 \;\Rightarrow\; m^2 \text{ è pari} \;\Rightarrow\; m \text{ è pari (teorema precedente)}$$

$$m = 2k \text{ per un (unico) } k \in \mathbb{N} \;\Rightarrow\; 2n^2 = m^2 = 4k^2 \;\Rightarrow\; n^2 = 2k^2$$

$$n^2 \text{ è pari} \;\Rightarrow\; n \text{ è pari (teorema precedente)} \;\Rightarrow\; n = 2h \text{ per un (unico) } h \in \mathbb{N}$$

Allora $m$ e $n$ sono entrambi pari, cioè divisibili per 2. **Assurdo**, perché per costruzione $m$ ed $n$ non hanno fattori comuni.

$$\Rightarrow \nexists\, r \in \mathbb{Q} : r^2 = 2 \qquad \blacksquare$$

### Note collegate
- [[00_MOC_A1]]
- [[02_Dimostrazioni]] — teorema "se $m^2$ è pari allora $m$ è pari" (contronominale)
- [[00_Insiemi_Numerici]] — $\mathbb{Q}$ e numeri irrazionali
- [[02_Estremo_Superiore_Inferiore]] — $\mathbb{Q}$ non soddisfa la proprietà dell'estremo superiore
- [[04_Retta_Reale_Intervalli]] — punti della retta a cui non corrisponde alcun razionale