---
created: 2026-10-08
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
aliases: []
---
[[00_GAL_Indice|⬅️ Torna all'Indice GAL]]

# MEG, Matrici Elementari, Rango e Proprietà del Determinante

> Lezione 7 — 08.10.2026. Prosegue da [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss|Lezione 6]]. Argomenti: reversibilità del [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Metodo di Eliminazione di Gauss (MEG)|Metodo di Eliminazione di Gauss]], codifica con il [[2026-10-01-Prodotto-Matriciale-e-Matrice-Identita#Prodotto matriciale righe per colonne|Prodotto Matriciale]], [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Definizione 6.3 — Rango|Rango di una Matrice]] e MEG, [[#Teorema di Binet|Teorema di Binet]], proprietà del [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Determinante|Determinante]].

## Il MEG: da $A$ a $U$

$$
A \ (\text{arbitraria}) \ \overset{\text{MEG}}{\leadsto}\ U \ (\text{a scala})
$$

### Commento 1: il processo del MEG è reversibile

Ciascuna delle tre operazioni elementari si può annullare con un'operazione dello stesso tipo.

- **Scambio**: $\begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} \xrightarrow{\mathrm{I}\leftrightarrow\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix} \xrightarrow{\mathrm{I}\leftrightarrow\mathrm{II}} \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix}$
- **Moltiplicazione per uno scalare $\neq 0$**: $\begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^8} & 3 & 7 \end{bmatrix} \xrightarrow{10^4\,\mathrm{II}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^4} & 3\cdot 10^4 & 7\cdot 10^4 \end{bmatrix} \xrightarrow{\frac{1}{10^4}\,\mathrm{II}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^8} & 3 & 7 \end{bmatrix}$
- **Sostituzione**: $\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} \xrightarrow{\mathrm{II}-4\mathrm{I}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix} \xrightarrow{\mathrm{II}+4\mathrm{I}\to\mathrm{II}} \begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix}$

### Commento 2: il processo di riduzione può essere codificato con il prodotto matriciale

**Scambio.** Esiste $S \in M_{\mathbb{R}}(2,2)$ tale che

$$
S \begin{bmatrix} 0 & 1 & -1 \\ 1 & 2 & 3 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & 1 & -1 \end{bmatrix}, \qquad
S = \begin{bmatrix} 0 & 1 \\ 1 & 0 \end{bmatrix}
$$

**Moltiplicazione.**

$$
\begin{bmatrix} 1 & 0 \\ 0 & 10^4 \end{bmatrix}\begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^8} & 3 & 7 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ \tfrac1{10^4} & 3\cdot 10^4 & 7\cdot 10^4 \end{bmatrix}
$$

**Sostituzione.**

$$
\begin{bmatrix} 1 & 0 \\ -4 & 1 \end{bmatrix}\begin{bmatrix} 1 & 2 & 3 \\ 4 & 5 & 6 \end{bmatrix} = \begin{bmatrix} 1 & 2 & 3 \\ 0 & -3 & -6 \end{bmatrix}
$$

(Domani: maggiori dettagli sull'esecuzione.)

> **Morale**: $A \overset{\text{MEG}}{\leadsto} U$ $\Rightarrow$ esiste una matrice $T$ tale che $TA = U$.

### Mettiamo insieme: MEG reversibile + MEG codificato con il prodotto (a sinistra)

$$
A \overset{T}{\leadsto} U \overset{Z}{\leadsto} A, \qquad A,U \in M_{\mathbb{K}}(m,n),\quad T,Z \in M_{\mathbb{K}}(m,m)
$$

$$
\left.\begin{array}{l} U = TA \\ A = ZU \end{array}\right\} \Rightarrow A = Z(TA) \overset{\text{prop. ass.}}{=} (ZT)A
$$

Poiché $(ZT)A = A$ per ogni $A \in M_{\mathbb{K}}(m,n)$:

$$
ZT = \mathrm{Id}_m \quad\Rightarrow\quad Z \text{ è l'inverso sinistro di } T,\ \ T \text{ è l'inverso destro di } Z
$$

Analogamente, da $U = TA = T(ZU) = (TZ)U$:

$$
TZ = \mathrm{Id}_m \quad\Rightarrow\quad Z \text{ è l'inverso destro di } T,\ \ T \text{ è l'inverso sinistro di } Z
$$

Quindi $T$ è l'inverso di $Z$ e viceversa:

$$
Z = T^{-1}, \qquad T = Z^{-1}
$$

> **Abbiamo dimostrato che le matrici inverse/invertibili esistono.** (Vedi [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Matrice inversa|Matrice Invertibile]].)

## MEG e rango

> «Il rango vuole essere una misura di complessità (quanta informazione c'è) di una matrice.» «Il MEG concentra l'informazione nella parte alta e a destra della matrice.»

**Esempio.** Matrice $2\times 6$ con tutte le entrate $\frac{1}{12}$ (pivot $p_1 = \frac1{12}$). Applico il MEG: $\mathrm{II} - \frac{1/12}{1/12}\mathrm{I} \to \mathrm{II}$ (moltiplicatore $1$):

$$
\begin{bmatrix} 1 & 0 \\ -1 & 1 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix} = \begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ 0 & \cdots & 0 \end{bmatrix}
$$

Invertendo il passo ($+1$):

$$
\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}
$$

e la matrice $U$ ottenuta si scrive come

$$
\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ 0 & \cdots & 0 \end{bmatrix} = \begin{bmatrix} 1 \\ 0 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix} \qquad (\text{rango } 1)
$$

Quindi

$$
\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}\left(\begin{bmatrix} 1 \\ 0 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}\right) = \left(\begin{bmatrix} 1 & 0 \\ 1 & 1 \end{bmatrix}\begin{bmatrix} 1 \\ 0 \end{bmatrix}\right)\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix} = \begin{bmatrix} 1 \\ 1 \end{bmatrix}\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}
$$

$$
\Rightarrow\quad r\left(\begin{bmatrix} \tfrac1{12} & \cdots & \tfrac1{12} \\ \tfrac1{12} & \cdots & \tfrac1{12} \end{bmatrix}\right) = 1
$$

### Proposizione

Data $A \in M_{\mathbb{K}}(m,n)$, sia $U$ una matrice a scala ottenuta con il MEG a partire da $A$. Allora:

- $r(U) = $ numero di righe non nulle di $U$ $=$ numero di pivot di $U$;
- $r(A) = r(U)$.

> **Il MEG è il modo EFFICIENTE per calcolare il rango di una matrice!!**

**Esempio — calcolo del rango.**

$$
\begin{bmatrix} 1 & 0 & -1 & 2 \\ 2 & 0 & 3 & 1 \\ 1 & 0 & 4 & -1 \end{bmatrix}
\xrightarrow[\ \mathrm{III}-\mathrm{I}\to\mathrm{III}\ ]{\ \mathrm{II}-2\mathrm{I}\to\mathrm{II}\ }
\begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 5 & -3 \end{bmatrix}
\xrightarrow{\ \mathrm{III}-\mathrm{II}\to\mathrm{III}\ }
\begin{bmatrix} 1 & 0 & -1 & 2 \\ 0 & 0 & 5 & -3 \\ 0 & 0 & 0 & 0 \end{bmatrix}
\Rightarrow r = 2
$$

(pivot: $1$ e $5$).

![[2026-10-08-calcolo-rango-con-MEG.png]]

## MEG e determinante

### Teorema di Binet

Siano $A,B \in M_{\mathbb{K}}(n,n)$ (quindi $AB \in M_{\mathbb{K}}(n,n)$):

$$
\det(AB) = \det(A)\,\det(B)
$$

(a sinistra il prodotto matriciale; a destra il prodotto tra numeri di $\mathbb{K}$).

### Conseguenze

- In generale $AB \neq BA$ (il prodotto **non** è commutativo), ma

  $$
  \det(AB) \overset{\text{Binet}}{=} \det(A)\det(B) = \det(B)\det(A) \overset{\text{Binet}}{=} \det(BA)
  $$

  perché il prodotto in $\mathbb{K}$ è commutativo.
- Sia $A \in M_{\mathbb{K}}(n,n)$ e $B \in M_{\mathbb{K}}(n,n)$ ottenuta da $A$ con una sequenza di operazioni elementari. Allora esistono $T,Z \in M_{\mathbb{K}}(n,n)$ tali che $B = TA$ e $A = ZB$. Per il teorema di Binet:

  - (I) $\det(B) = \det(TA) = \det(T)\det(A)$
  - (II) $\det(A) = \det(ZB) = \det(Z)\det(B)$

  Da (I): $\det(A) = 0 \Rightarrow \det(B) = 0$. Da (II): $\det(B) = 0 \Rightarrow \det(A) = 0$. Quindi

  $$
  \det(A) = 0 \iff \det(B) = 0, \qquad \text{equivalentemente} \qquad \det(A) \neq 0 \iff \det(B) \neq 0
  $$

### Osservazione: calcolo del determinante con il MEG

Per $A \in M_{\mathbb{K}}(n,n)$, $A \overset{\text{MEG}}{\leadsto} U \in M_{\mathbb{K}}(n,n)$ a scala, in particolare $U$ è triangolare superiore. Con $A = ZU$:

$$
\det(A) = \det(Z)\det(U) = \det(Z)\, u_{11}u_{22}\cdots u_{nn}
$$

## Proprietà del determinante

### Il determinante è normalizzato

$$
\det \mathrm{Id}_n = \det\begin{bmatrix} 1 & & 0 \\ & \ddots & \\ 0 & & 1 \end{bmatrix} = 1\cdots 1 = 1
$$

(a sinistra $\mathrm{Id}_n$ è l'elemento neutro del prodotto matriciale; $1$ a destra è l'elemento neutro del prodotto in $\mathbb{K}$).

### Il determinante è alternante

Se $A \leadsto B$ con uno **scambio di righe**, allora $\det(B) = -\det(A)$.

*Esempio*: $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\mathrm{I}\leftrightarrow\mathrm{II}} B = \begin{bmatrix} c & d \\ a & b \end{bmatrix}$: $\det(A) = ad - bc$, $\det(B) = cb - ad = -(ad - bc)$.

### Il determinante è multilineare

**Moltiplicazione.** Se moltiplico una riga di $A$ per $\lambda \neq 0 \in \mathbb{K}$ ($A \leadsto B$, $R_i \cdot \lambda$), allora $\det(B) = \lambda\det(A)$.

*Esempio*: $A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\lambda\mathrm{II}\to\mathrm{II}} B = \begin{bmatrix} a & b \\ \lambda c & \lambda d \end{bmatrix}$:

$$
\det(B) = a(\lambda d) - (\lambda c)b = \lambda(ad - bc) = \lambda\det(A)
$$

Anche se moltiplico una **colonna** per $\lambda \neq 0$ il determinante viene moltiplicato per $\lambda$: $\det\begin{bmatrix} \lambda a & b \\ \lambda c & d \end{bmatrix} = (\lambda a)d - (\lambda c)b = \lambda(ad - bc)$.

**Cosa succede se moltiplico tutta la matrice per $\lambda$?** Si moltiplicano tutte le righe, quindi

$$
\det\left(\lambda\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) = \lambda^2\det\begin{bmatrix} a & b \\ c & d \end{bmatrix}
\qquad\text{e in generale per } A \in M_{\mathbb{K}}(n,n):\quad \det(\lambda A) = \lambda^n\det(A)
$$

**Sostituzione.** $A \leadsto B$ con $R_i + \lambda R_k \to R_i$.

*Esempio*: $\begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\mathrm{II}+\lambda\mathrm{I}\to\mathrm{II}} \begin{bmatrix} a & b \\ c+\lambda a & d+\lambda b \end{bmatrix}$:

$$
\det = a(d + \lambda b) - (c + \lambda a)b = ad + \lambda ab - bc - \lambda ab = ad - bc = \det(A)
$$

> **Morale**: con la sostituzione il determinante non cambia!!!

Usando la multilinearità sulla seconda riga:

$$
\det\begin{bmatrix} a & b \\ c+\lambda a & d+\lambda b \end{bmatrix} = \det\begin{bmatrix} a & b \\ c & d \end{bmatrix} + \lambda\det\begin{bmatrix} a & b \\ a & b \end{bmatrix} = \det(A) + \lambda\cdot 0
$$

### Proprietà: due righe (o colonne) uguali

Se una matrice ha due righe (o due colonne) uguali, allora il determinante è $0$.

*Dimostrazione.* Sia $B = \begin{bmatrix} a & b \\ a & b \end{bmatrix}$ e $B'$ la matrice ottenuta da $B$ con lo scambio $\mathrm{I}\leftrightarrow\mathrm{II}$. Poiché le righe sono uguali, $B = B'$. Per l'alternanza $\det(B') = -\det(B)$. Quindi

$$
\det(B) = -\det(B) \ \Rightarrow\ 2\det(B) = 0 \ \Rightarrow\ \det(B) = 0 \qquad \blacksquare
$$

*(Il passaggio finale usa $2 \neq 0$ in $\mathbb{K}$, cioè $\mathbb{K}$ diverso da $\mathbb{F}_2$.)*

Vedi anche: [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Determinante di una matrice triangolare|Matrice Triangolare]], [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Definizione 6.6 — Matrice a scala|Matrice a Scala]], [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Definizione 6.6 — Matrice a scala|Pivot]], [[2026-10-07-Inversa-Rango-Determinante-e-Eliminazione-di-Gauss#Metodo di Eliminazione di Gauss (MEG)|Operazioni Elementari sulle Righe]], [[#Teorema di Binet|Teorema di Binet]].
