---
created: 2026-10-08
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/rango_e_determinante
aliases: []
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Proprietà del Determinante

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

---
Precedente: [[Calcolo del Determinante con il MEG]]
