---
tags:
  - matematica
  - analisi
  - logica
  - insiemi-numerici
  - AM1
---

# Insiemi Numerici e Logica

## Insiemi Numerici

$$\mathbb{N},\ \mathbb{Z},\ \mathbb{Q},\ \mathbb{R},\ \mathbb{C}$$

- $\mathbb{N} = \{0, 1, 2, 3, \dots\}$ — numeri naturali, interi non negativi
- $\mathbb{Z} = \{\dots, -3, -2, -1, 0, 1, 2, 3, \dots\}$ — numeri interi relativi
- $$\mathbb{Q} = \left\{ \frac{m}{n} : m, n \in \mathbb{Z},\ n \neq 0 \right\} \quad \text{numeri razionali}$$

> [!info] Notazione
> - $:$ "tale che" (anche $\mid$)
> - $\forall$ "per ogni"
> - $\in$ "appartiene"
> - $\setminus$ (es. $A \setminus B$) "escluso"
> - elementi minuscoli, insiemi maiuscoli
> - $\subset$ "è contenuto"

Ogni numero razionale $x \in \mathbb{Q}$ può essere rappresentato da infinite frazioni equivalenti.

Ogni numero razionale $x \in \mathbb{Q}$ può essere rappresentato anche in formato decimale:

$$\mathbb{Q} = \left\{ x = \pm a_0,\, a_1 a_2 a_3 \dots a_k : a_0 \in \mathbb{N},\ a_k \in [0,9],\ \forall k \in \mathbb{N},\ k \neq 0 \right\}$$

Le rappresentazioni decimali dei numeri razionali sono tutte **o finite** (c'è solo un numero finito di cifre decimali $\neq 0$) **o infinite e periodiche** (numero infinito di cifre decimali che però ad un certo punto si ripetono periodicamente).

> [!note] Osservazione
> Mancano gli infiniti non periodici — cioè i numeri la cui rappresentazione decimale è infinita e *non* periodica: sono i numeri irrazionali (vedi sotto).

$$\mathbb{R} = \left\{ x = \pm a_0,\, a_1 a_2 a_3 \dots a_k : a_0 \in \mathbb{N},\ a_k \in [0,9],\ \forall k \in \mathbb{N},\ k \neq 0 \right\} \quad \text{numeri reali}$$

con rappresentazione decimale finita o infinita, periodica o no.

I numeri in $\mathbb{R} \setminus \mathbb{Q}$, cioè i numeri $x \in \mathbb{R} : x \notin \mathbb{Q}$, si dicono **irrazionali**.

$$\mathbb{C} = \{ z = a + ib : a, b \in \mathbb{R},\ i^2 = -1 \} \quad \text{numeri complessi}$$

$$\mathbb{N} \subset \mathbb{Z} \subset \mathbb{Q} \subset \mathbb{R} \subset \mathbb{C}$$

---

## Elementi di Logica

> [!warning] Def. Proposizione
> Una **proposizione** è un enunciato non contenente variabili libere a cui si possa attribuire in maniera univoca il valore vero o falso. Si indicano con $P, Q, \dots$

> [!warning] Def. Predicato
> Un **predicato** è un enunciato contenente variabili libere, il cui valore di verità (vero o falso) dipende dal valore delle variabili. Tuttavia, per ogni assegnazione delle variabili, il predicato deve collassare su una proposizione, quindi essere oggettivamente vero o falso. Si indicano con $P(x,y,\dots)$, $Q(x,y,\dots)$, dove $x, y, \dots$ sono le variabili libere.

> [!note] Osservazione
> L'insieme (o gli insiemi) in cui variano le variabili è parte della definizione del predicato.

### Connettivi Logici

| Simbolo           | Significato     | Definizione                                                                                                                                                        |
| ----------------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| $\land$           | "e"             | Date $P,Q$ proposizioni, $P \land Q$ è vera se sono vere entrambe, falsa altrimenti                                                                                |
| $\lor$            | "o"             | Date $P,Q$ proposizioni, $P \lor Q$ è vera se almeno una è vera                                                                                                    |
| $\neg$            | "non"           | Data $P$ proposizione, $\neg P$ è vera se $P$ è falsa e viceversa                                                                                                  |
| $\Rightarrow$     | "se ... allora" | Date $P,Q$ proposizioni, $P \Rightarrow Q$ è vera se $P$ è vera e $Q$ è vera, oppure se $P$ è falsa (qualunque sia il valore di verità di $Q$); è falsa altrimenti |
| $\Leftrightarrow$ | "se e solo se"  | Date $P,Q$ proposizioni, $P \Leftrightarrow Q$ è vera se $P$ e $Q$ sono entrambe vere o entrambe false, falsa altrimenti                                           |

### Quantificatori

Per assegnare un valore di verità ad un predicato è necessario "saturare" le variabili libere. In tal modo si ottiene una proposizione con il suo valore di verità, vero o falso. Ciò può essere fatto fissando il valore delle variabili oppure con l'uso di quantificatori:

- $\forall$ "per ogni"
- $\exists$ "esiste"
- $\exists!$ "esiste ed è unico"
- $\nexists$ "non esiste"

> [!warning] Def. Implicazione universale
> Un enunciato che presenta la struttura
> $$\forall x \in A \quad P(x) \Rightarrow Q(x)$$
> con $A$ insieme, $P(x)$ e $Q(x)$ predicati per $x \in A$, prende il nome di **implicazione universale**.

> [!warning] Def. Condizione necessaria e sufficiente
> Date $P, Q$ proposizioni (predicati), se $P \Rightarrow Q$ è vera, diremo che $P$ è condizione **sufficiente** affinché $Q$, e $Q$ è condizione **necessaria** per $P$.
>
> Se $P \Leftrightarrow Q$ è vera, diremo che $P$ è necessaria e sufficiente affinché $Q$, e viceversa.

> [!example] Esempio
> $P$: il triangolo è equilatero
> $Q$: il triangolo è isoscele
>
> $P \Rightarrow Q$ vera $\;\Rightarrow\;$ $P$ è sufficiente per $Q$, e $Q$ è necessaria per $P$

---

## Teoremi, Dimostrazioni e Controesempi

Un **teorema** è un asserto di cui si vuole dimostrare la verità, partendo da delle ipotesi. Le **ipotesi** sono una o più proposizioni o predicati $P$, la **tesi** è una proposizione o predicato $Q$. Dimostrare il teorema significa provare che $P \Rightarrow Q$ è vera, oppure che $\neg Q \Rightarrow \neg P$ è vera.

La **dimostrazione** è l'insieme di passaggi e deduzioni logiche che partono da $P$ vera e si concludono con $Q$ vera.

### 1. Metodo deduttivo (dimostrazione diretta)

> [!theorem]
> $\forall m \in \mathbb{N}$, se $m$ è dispari allora $m^2$ è dispari.

$$\forall m \in \mathbb{N} \quad P(m) \Rightarrow Q(m)$$

- $P(m)$: $m$ è dispari
- $Q(m)$: $m^2$ è dispari

**Dimostrazione.** Sia $m \in \mathbb{N}$ dispari. Allora $m = 2k+1$ per un (unico) $k \in \mathbb{N}$.

$$m^2 = (2k+1)^2 = 4k^2 + 4k + 1 = 2(2k^2+2k) + 1$$

Quindi $m^2 = 2a+1$ con $a = 2k^2+2k$, cioè $m^2$ è dispari. $\blacksquare$

### 2. Variante di dimostrazione diretta (contronominale)

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

### 3. Controesempio

Mostrare che $P \Rightarrow Q$ è falsa significa mostrare che $P$ è vera e $Q$ è falsa, cioè che $P \land \neg Q$ è vera.

Per un'implicazione universale $\forall x \in A,\ P(x) \Rightarrow Q(x)$, affermare che sia falsa vuol dire:

$$\exists\, x_0 \in A : P(x_0) \Rightarrow Q(x_0) \text{ sia falsa} \quad \Longleftrightarrow \quad \exists\, x_0 \in A : P(x_0) \land \neg Q(x_0) \text{ sia vera}$$

$x_0$ prende il nome di **controesempio** dell'implicazione universale $\forall x \in A,\ P(x) \Rightarrow Q(x)$, e dimostra che essa è falsa.

> [!theorem]
> $\forall m \in \mathbb{N}$, se $m$ è primo allora $m$ è dispari.

Questo teorema è **falso**: un controesempio (unico, in questo caso) è $m=2$, che è primo (ipotesi soddisfatta) ma è anche pari (tesi negata). $\blacksquare$

### 4. Dimostrazione per assurdo

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

### 5. Dimostrazione per induzione

Si usa per dimostrare la verità di un'implicazione universale della forma $\forall m \in \mathbb{N},\ P(m)$ vera. Si articola in due passi:

1. si dimostra che $P(0)$ è vera ($m=0$);
2. si dimostra che **se** $P(m)$ è vera **allora** è vera anche $P(m+1)$, cioè $\forall m \in \mathbb{N},\ P(m) \Rightarrow P(m+1)$.

$P(m)$ prende il nome di **ipotesi di induzione**.

Informalmente: $P(0) \text{ vera} \xrightarrow{i} P(1) \text{ vera} \xrightarrow{ii} P(2) \text{ vera} \xrightarrow{iii} \dots$

> [!theorem] Disuguaglianza di Bernoulli
> $\forall m \in \mathbb{N},\ \forall x \in \mathbb{R}$ con $x > -1$:
> $$(1+x)^m \geq 1+mx$$

**Dimostrazione (per induzione).** Sia $P(m)$: $\forall x \in \mathbb{R}$ con $x>-1$, $(1+x)^m \geq 1+mx$.

**i) Verifichiamo $P(0)$ vera**

$$(1+x)^0 \geq 1+0\cdot x \;\Longleftrightarrow\; 1 \geq 1 \quad \text{vera}$$

**ii) Verifichiamo $P(m) \Rightarrow P(m+1)$ vera $\forall m \in \mathbb{N}$**

$$P(m+1): \quad (1+x)^{m+1} \geq 1+(m+1)x$$

Assumendo $P(m)$ vera, partiamo da:

$$(1+x)^{m+1} = (1+x)^m (1+x)$$

dove $(1+x)>0$ e $(1+x)^m \geq 1+mx$ per ipotesi di induzione $P(m)$. Quindi:

$$(1+x)^{m+1} = (1+x)^m(1+x) \geq (1+mx)(1+x) = 1+mx+x+mx^2 = 1+(m+1)x+\underbrace{mx^2}_{\geq 0}$$

da cui $1+(m+1)x+mx^2 \geq 1+(m+1)x$, quindi:

$$(1+x)^{m+1} \geq (1+mx)(1+x) \geq 1+(m+1)x$$

cioè $P(m+1)$ è vera. Pertanto $P(m) \Rightarrow P(m+1)$ è vera $\forall m \in \mathbb{N}$, e per induzione $P(m)$ è vera $\forall m \in \mathbb{N}$. $\blacksquare$
