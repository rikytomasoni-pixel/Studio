---
created: 2026-09-30
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
aliases: []
---
[[00_GAL_Indice|⬅️ Torna all'Indice GAL]]

# Matrici: Definizione, Somma e Prodotto per uno Scalare

> Lezione 3 — 30.09.2026. Argomenti: [[#Definizione di Matrice|Matrice]], [[#Somma tra matrici|Somma tra Matrici]], [[#Prodotto di una matrice per uno scalare|Prodotto di una Matrice per uno Scalare]].

## Motivazione: rappresentare funzioni su prodotti cartesiani

**Obiettivo**: «valutare»/«quantificare» gli elementi di un [[2026-09-16-Prodotto-Cartesiano-e-Relazioni#Prodotto Cartesiano|Prodotto Cartesiano]].

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

## Campi numerici e $\mathbb{F}_2$

Ora definiamo le matrici in generale.

**Caratteristiche comuni**: abbiamo studiato funzioni con dominio un prodotto cartesiano di insiemi **finiti**; il codominio delle funzioni è sempre stato un insieme di numeri. D'ora in poi prenderemo come codominio un **campo numerico**: $\mathbb{Q}$, $\mathbb{R}$, $\mathbb{C}$, $\mathbb{F}_2$ (campo finito).

**Notazione**: $[m] = \{1,2,\dots,m\}$ e $[n] = \{1,2,\dots,n\}$, quindi

$$
[m] \times [n] = \{(1,1),(1,2),\dots,(1,n),\ (2,1),(2,2),\dots,(2,n),\ \dots,\ (m,1),(m,2),\dots,(m,n)\}
$$

### Il campo $\mathbb{F}_2 = \{0,1\}$

$0$ = falso (interruttore aperto), $1$ = vero (interruttore chiuso).

- **XOR** («o uno o l'altro ma non entrambi»): realizzato con due deviatori in serie; la lampadina è accesa se i due deviatori sono in posizioni diverse. Corrisponde alla **somma** $+$ in $\mathbb{F}_2$.
- **AND** («sia l'uno che l'altro»): realizzato con due interruttori in serie; la lampadina è accesa solo se entrambi sono chiusi. Corrisponde al **prodotto** $\cdot$ in $\mathbb{F}_2$.

> **Figura (disegno senza immagine disponibile):**
>
> Due schemi di circuito (batteria "+ −", due elementi in serie, lampadina). Sopra il circuito XOR con due *deviatori* e sotto il circuito AND con due *interruttori*, ciascuno con la tabella a doppia entrata (0 rosso = interruttore aperto/falso, 1 verde = chiuso/vero) e lampadina accesa/spenta. Per XOR: $0,0 \to 0$; $0,1 \to 1$; $1,0 \to 1$; $1,1 \to 0$. Per AND: acceso solo per $1,1$.

Operazioni in $\mathbb{F}_2$:

| $+$ | 0 | 1 |
|:-:|:-:|:-:|
| **0** | 0 | 1 |
| **1** | 1 | 0 |

| $\cdot$ | 0 | 1 |
|:-:|:-:|:-:|
| **0** | 0 | 0 |
| **1** | 0 | 1 |

## Definizione di Matrice

### Definizione 3.1

Una **matrice** $A$ è una funzione

$$
A : [m] \times [n] \to \mathbb{K}
$$

dove $\mathbb{K}$ è un campo numerico ($\mathbb{Q}, \mathbb{R}, \mathbb{C}, \mathbb{F}_2, \dots$). Ovvero $A$ è una tabella con $m$ righe e $n$ colonne contenente valori in $\mathbb{K}$:

$$
A = \begin{bmatrix} A(1,1) & A(1,2) & \cdots & A(1,n) \\ \vdots & & & \vdots \\ A(m,1) & A(m,2) & \cdots & A(m,n) \end{bmatrix}
= \begin{bmatrix} a_{11} & a_{12} & a_{13} & \cdots & a_{1n} \\ \vdots & & & & \vdots \\ a_{m1} & a_{m2} & & \cdots & a_{mn} \end{bmatrix}
$$

con $a_{ij} = A(i,j)$, dove $i$ è l'**indice di riga** e $j$ l'**indice di colonna**.

### Notazione e casi speciali

$M_{\mathbb{K}}(m,n) = \{\text{matrici di tipo } (m,n) \text{ (}m\text{ righe e }n\text{ colonne) con valori in } \mathbb{K}\}$.

- **$M_{\mathbb{K}}(1,1)$** $= \{[a_{11}] \mid a_{11} \in \mathbb{K}\}$. C'è una corrispondenza 1:1 (**funzione biettiva**) $M_{\mathbb{K}}(1,1) \leftrightarrow \mathbb{K}$, con $[a_{11}] \mapsto a_{11}$ e $[k] \leftarrow k$.
- **$m=1$, $n>1$**: $M_{\mathbb{K}}(1,n) = \{[a_{11}\ a_{12}\ \dots\ a_{1n}] \mid a_{1j} \in \mathbb{K}\ \forall j\} = \{\text{vettori riga di lunghezza } n\}$.

  > N.B. $M_{\mathbb{K}}(1,n) \overset{1:1}{\longleftrightarrow} \underbrace{\mathbb{K} \times \mathbb{K} \times \dots \times \mathbb{K}}_{n \text{ volte}}$, cioè vettori riga di lunghezza $n$ $\leftrightarrow$ liste ordinate di lunghezza $n$: $[a_{11} \dots a_{1n}] \mapsto (a_{11},\dots,a_{1n})$ e $[k_1\ k_2 \dots k_n] \leftarrow (k_1,k_2,\dots,k_n)$. Quindi $M_{\mathbb{K}}(1,n) = \mathbb{K}^n$ (più precisamente $M_{\mathbb{K}}(1,n) \cong \mathbb{K}^n$).
- **$m>1$, $n=1$**: $M_{\mathbb{K}}(m,1) = \left\{ \begin{bmatrix} a_{11} \\ a_{21} \\ \vdots \\ a_{m1} \end{bmatrix} \,\middle|\, a_{i1} \in \mathbb{K}\ \forall i \right\} = \{\text{vettori colonna di altezza } m\}$, e $M_{\mathbb{K}}(m,1) \cong \mathbb{K}^m$ (liste ordinate di $m$ elementi in $\mathbb{K}$).
- **$m=n$**: $M_{\mathbb{K}}(n,n) = M_{\mathbb{K}}(n) = \{\text{matrici quadrate di ordine } n\}$.

## Uguaglianza di matrici

A cosa servono le matrici? Per scoprirne l'utilità dobbiamo ripercorrere un po' la storia, tornando all'interpretazione delle matrici come funzioni. Con funzioni $f : \mathbb{R} \to \mathbb{R}$ siamo soliti: confrontare/distinguere le funzioni, sommare funzioni, moltiplicare funzioni (e moltiplicare una funzione per un numero), comporre funzioni.

**Confronto**: siano $A \in M_{\mathbb{K}}(m,n)$ e $B \in M_{\mathbb{K}}(p,q)$.

- Se $m \neq p$ oppure $n \neq q$ $\Rightarrow$ $A \neq B$.
- Se $A, B \in M_{\mathbb{K}}(m,n)$:

$$
A = B \iff A(i,j) = B(i,j)\ \forall (i,j) \iff a_{ij} = b_{ij}\ \ \forall i = 1,\dots,m,\ \forall j = 1,\dots,n
$$

## Somma tra matrici

«Se voglio sommare due funzioni, queste devono avere lo stesso dominio.» Ad esempio per $f(x) = \frac{1}{x^2-1}$ e $g(x) = e^x$ il valore $(f+g)(1)$ non è definito.

### Definizione

$$
+ : M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(m,n) \to M_{\mathbb{K}}(m,n), \qquad (A,B) \longmapsto A+B
$$

Con $A = [a_{ij}]$ e $B = [b_{ij}]$:

$$
A + B = [a_{ij} + b_{ij}]
$$

(«somma posizione per posizione», «somma puntuale»).

**Esempio**

$$
\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} -1 & 1 \\ 4 & 7 \end{bmatrix}
= \begin{bmatrix} 1+(-1) & -2+1 \\ 0+4 & 3+7 \end{bmatrix}
= \begin{bmatrix} 0 & -1 \\ 4 & 10 \end{bmatrix}
$$

### Proprietà della somma

«Ereditiamo le proprietà della somma del campo.» $\forall A,B,C \in M_{\mathbb{K}}(m,n)$:

- **Proprietà associativa**: $(A+B)+C = A+(B+C) = A+B+C$.
- **Proprietà commutativa**: $A+B = B+A$.
- **Esistenza dell'elemento neutro**: $\exists N \in M_{\mathbb{K}}(m,n)$ tale che $\forall A \in M_{\mathbb{K}}(m,n)$, $A+N = N+A = A$. *Chi è $N$?* La **matrice nulla**:

  $$N = \begin{bmatrix} 0 & \cdots & 0 \\ \vdots & & \vdots \\ 0 & \cdots & 0 \end{bmatrix}$$

  Ad esempio $\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix} = \begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix}$.
- **Esistenza dell'elemento opposto**: $\forall A \in M_{\mathbb{K}}(m,n)$ $\exists A' \in M_{\mathbb{K}}(m,n)$ tale che $A + A' = A' + A = $ matrice nulla. *Chi è $A'$?* Se $A = [a_{ij}]$, allora $A' = [-a_{ij}]$. Esempio: $\begin{bmatrix} 1 & -2 \\ 0 & 3 \end{bmatrix} + \begin{bmatrix} -1 & 2 \\ 0 & -3 \end{bmatrix} = \begin{bmatrix} 0 & 0 \\ 0 & 0 \end{bmatrix}$.

## Prodotto di una matrice per uno scalare

$$
\cdot : \mathbb{K} \times M_{\mathbb{K}}(m,n) \to M_{\mathbb{K}}(m,n), \qquad (\lambda, A) \longmapsto \lambda A
$$

($\lambda$ è la lettera greca *lambda* minuscola.) Con $A = [a_{ij}]$:

$$
\lambda A = [\lambda a_{ij}]
$$

**Esempio** ($\lambda = 2$):

$$
2 \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}
= \begin{bmatrix} 2\cdot 1 & 2\cdot 2 & 2\cdot 3 \\ 2\cdot 4 & 2\cdot 5 & 2\cdot 6 \end{bmatrix}
= \begin{bmatrix} 2 & 4 & 6 \\ 8 & 10 & 12 \end{bmatrix}
$$

### Proprietà (ereditate dal prodotto nel campo $\mathbb{K}$)

- **Distributiva a destra**: $\forall \lambda \in \mathbb{K}$, $\forall A,B \in M_{\mathbb{K}}(m,n)$: $\lambda(A+B) = \lambda A + \lambda B$.
- **Distributiva a sinistra**: $\forall \lambda,\mu \in \mathbb{K}$ ($\mu$ = *mu* minuscola), $\forall A \in M_{\mathbb{K}}(m,n)$: $(\lambda+\mu)A = \lambda A + \mu A$.
- **Associativa**: $\forall \lambda,\mu \in \mathbb{K}$, $\forall A$: $(\lambda\mu)A = \mu(\lambda A) = \lambda(\mu A)$.
- **Esistenza dell'elemento neutro**: $\forall A$: $1A = A$ (dove $1$ è l'elemento $1$ di $\mathbb{K}$).

> **Osservazione**: potremmo anche definire un prodotto tra due matrici posizione per posizione, ma questa operazione non ha grande utilità.

## Perché elencare le proprietà delle operazioni?

Sono estremamente significative per l'**efficienza computazionale**! La complessità di un calcolo viene spesso stimata calcolando quanti prodotti tra numeri devo calcolare.

*(Nell'esempio a mano: la somma $1123 + 625 = 1748$ richiede solo addizioni di cifre, mentre il prodotto $1123 \times 625$ richiede il calcolo di tre righe parziali: $5615$, $2246$ (traslato), $6738$ (traslato di due posizioni), da sommare.)*

**Esempio — distributiva a destra** $\lambda(A+B) = \lambda A + \lambda B$. Prendiamo due matrici $A,B \in M_{\mathbb{R}}(m,n)$:

- Quanti prodotti calcolo in $\lambda(A+B)$? $A+B \in M_{\mathbb{K}}(m,n)$, quindi $m \cdot n$ prodotti.
- Quanti prodotti calcolo in $\lambda A + \lambda B$? $2\, m \cdot n$ prodotti.

### Valutazione empirica

> **Figura (disegno senza immagine disponibile):**
>
> Due grafici per matrici di tipo $(1000,1500)$. Sinistra «Confronto tra le strategie»: asse $x$ = numero di ripetizioni (0–1000), asse $y$ = tempo in secondi; due rette crescenti, $\lambda(A+B)$ (blu, circa 5 s a 1000 ripetizioni) e $\lambda A + \lambda B$ (arancione, circa 7,5 s). Destra «Rapporto tra i tempi di esecuzione»: rapporto Strategia 2 / Strategia 1 in funzione del numero di ripetizioni; parte da circa 0,6 per 0 ripetizioni, sale rapidamente e si stabilizza intorno a 1,5.

Conclusione empirica: la strategia $\lambda(A+B)$ è circa $1.5$ volte più veloce di $\lambda A + \lambda B$.

Vedi anche: Campo Numerico, [[#Notazione e casi speciali|Matrice Nulla]], [[2026-09-17-Relazioni-d-Ordine-e-Funzioni#Iniettività e surgettività delle funzioni|Funzione Biettiva]].
