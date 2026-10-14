---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/matrici
aliases: []
---
[[00_GAL_Matrici|⬅️ Torna a Matrici]]

# Matrici come Rappresentazione di Funzioni

**Obiettivo**: «valutare»/«quantificare» gli elementi di un [[Prodotto Cartesiano|Prodotto Cartesiano]].

### Esempio 1 — voto finale

$T = \{\text{voti sufficienti della prova teorica}\}$, $E = \{\text{voti sufficienti della prova di esercizi}\}$.

$$
T \times E = \{(16,16),(16,17),\dots,(16,32),\ (17,16),(17,17),\dots,(17,32),\ \dots,\ (32,16),\dots,(32,32)\}
$$

$$
V : T \times E \to \mathbb{N}, \qquad (t,e) \longmapsto \left\lceil \frac{30}{100}\,t + \frac{70}{100}\,e \right\rceil
$$

**Obiettivo**: cercare una rappresentazione alternativa di $V$ (che sia più efficace/comunicativa).

> **Figura (disegno senza immagine disponibile):**
>
> Tabella a doppia entrata a colori: le **righe** (verticale, «TEORIA 30%») corrispondono agli elementi di $T$ (da 16 a 32); le **colonne** («ESERCIZI 70%») corrispondono agli elementi di $E$ (da 16 a 32). Ogni cella contiene il voto finale arrotondato; le celle in alto a sinistra (rosse) sono insufficienti (16–17), le altre verdi, fino a 30L in basso a destra.

### Esempio 2 — moneta e dado

$M = \{\text{esiti lancio di una moneta}\}$, $D = \{\text{esiti lancio di un dado}\}$, $M \times D = \{\text{coppie (ordinate) di esiti del lancio di una moneta e un dado}\} = \{(T,1),(T,2),\dots\}$.

$$
\mathbb{P} : M \times D \to [0,1] \subseteq \mathbb{R}, \qquad \mathbb{P}((m,d)) = \frac{\#\text{esiti favorevoli}}{\#\text{totale di esiti possibili}} = \frac{1}{12}
$$

Come primo passo posso rappresentare la funzione mediante una tabella:

| | 1 | 2 | 3 | 4 | 5 | 6 |
|---|---|---|---|---|---|---|
| **T** | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 |
| **C** | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 | 1/12 |

Questa tabella si chiama **matrice di probabilità congiunta** di $M$ e $D$.

### Esempio 3 — grafico di una funzione

Sia $f : \mathbb{R} \to \mathbb{R}$. Il suo grafico è

$$
\Gamma(f) = \{(x,y) \mid y = f(x)\} \subseteq \mathbb{R} \times \mathbb{R}
$$

Si definisce la funzione indicatrice

$$
v : \mathbb{R} \times \mathbb{R} \to \{0,1\}, \qquad
v(x,y) = \begin{cases} 1 & \text{se } (x,y) \in \Gamma(f) \\ 0 & \text{se } (x,y) \notin \Gamma(f) \end{cases}
$$

> **Figura (disegno senza immagine disponibile):**
>
> Disegno 3D prospettico: un piano azzurro con assi $x$ (verso l'osservatore, in basso a sinistra) e $y$ (verso destra). Sul piano è tracciata in rosso la curva $y = f(x)$ per $f(x) = x^2$; da essa partono segmenti verticali che si congiungono, in alto, a una curva blu che rappresenta $v(x,y)$ (vale 1 sul grafico). La parte tratteggiata rossa prosegue la curva oltre il tratto disegnato.

### Esempio 4 — frutta e iniziali

$A = \{\text{anguria, limone, lampone}\}$, $B = \{\text{"a"},\text{"b"},\text{"l"}\}$, $f : A \to B$, «$\ldots \in A$ ha come iniziale $\ldots \in B$»:

$$
f(\text{anguria}) = \text{"a"},\quad f(\text{limone}) = \text{"l"},\quad f(\text{lampone}) = \text{"l"}
$$

$$
\Gamma(f) = \{(\text{anguria},\text{"a"}),(\text{limone},\text{"l"}),(\text{lampone},\text{"l"})\} \subseteq A \times B
$$

$$
v : A \times B \to \{0,1\}, \qquad
v(\text{frutta},\text{lettera}) = \begin{cases} 1 & \text{se } (\text{frutta},\text{lettera}) \in \Gamma(f) \\ 0 & \text{se } (\text{frutta},\text{lettera}) \notin \Gamma(f) \end{cases}
$$

Utilizziamo una tabella:

| | anguria | lampone | limone |
|---|---|---|---|
| **"a"** | 1 | 0 | 0 |
| **"b"** | 0 | 0 | 0 |
| **"l"** | 0 | 1 | 1 |

---
Successivo: [[Il Campo F2]]
