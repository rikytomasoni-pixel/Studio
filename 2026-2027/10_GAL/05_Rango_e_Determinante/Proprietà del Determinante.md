---
created: 2026-10-08
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/7
  - argomento/rango_e_determinante
aliases: []
origine: UpdateVault
---
[[00_GAL_Rango_e_Determinante|⬅️ Torna a Rango e Determinante]]

# Proprietà del Determinante

## Proprietà del determinante

> [!abstract] Teorema (Proprietà — il determinante è normalizzato)
> $$\det \mathrm{Id}_n = \det \begin{bmatrix} 1 & & 0 \\ & \ddots & \\ 0 & & 1 \end{bmatrix} = 1 \cdots 1 = 1$$
> [annotazioni: $\mathrm{Id}_n$ = elemento neutro del prodotto matriciale; $1$ = elemento neutro del prodotto in $\mathbb{K}$]

> [!abstract] Teorema (Proprietà — il determinante è alternante)
> $A \overset{\text{scambio di righe}}{\leadsto} B \Rightarrow \det(B) = -\det(A)$

> [!example] Esempio
> $$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } B = \begin{bmatrix} c & d \\ a & b \end{bmatrix}$$
> $\det(A) = ad - bc$, $\qquad \det(B) = cb - ad = -(ad - bc)$

Una conseguenza dell'alternanza è in [[Proprietà del Determinante]].

## Determinante multilineare

> [!abstract] Teorema (Proprietà — il determinante è multilineare)
> **MOLTIPLICAZIONE** — se moltiplico una riga di $A$ per $\lambda \neq 0 \in \mathbb{K}$:
> $A \overset{\text{moltiplico } R_i \text{ per } \lambda}{\leadsto} B$, allora
> $$\det(B) = \lambda \det(A)$$

> [!example] Esempio
> $$A = \begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\ \lambda\,\mathrm{II} \to \mathrm{II}\ } \begin{bmatrix} a & b \\ \lambda c & \lambda d \end{bmatrix} = B$$
> $\det(A) = ad - bc$
> $\det(B) = a(\lambda d) - (\lambda c)b = \lambda(ad - bc) = \lambda \det A$

> [!note] Osservazione
> Anche se moltiplico una colonna per $\lambda \neq 0 \in \mathbb{K}$ il determinante viene moltiplicato per $\lambda$:
> $$\det\begin{bmatrix} \lambda a & b \\ \lambda c & d \end{bmatrix} = (\lambda a)d - (\lambda c)b = \lambda(ad - bc)$$

> [!note] Osservazione (Domanda)
> D. cosa succede se moltiplico tutta la matrice per $\lambda$?
> $$\det\left(\lambda \begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) = \det\left(\begin{bmatrix} \lambda a & \lambda b \\ \lambda c & \lambda d \end{bmatrix}\right)$$
> $$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow[\ \lambda\,\mathrm{II} \to \mathrm{II}\ ]{\ \lambda\,\mathrm{I} \to \mathrm{I}\ } \begin{bmatrix} \lambda a & \lambda b \\ \lambda c & \lambda d \end{bmatrix}$$
> $$\det\left(\lambda \begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) = \lambda^2 \det\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right)$$
> $A \in M_{\mathbb{K}}(n,n)$: $\quad \det(\lambda A) = \lambda^{n}\det(A)$

## Determinante e operazione di sostituzione

**SOSTITUZIONE** — $A \overset{R_i + \lambda R_k \to R_i}{\leadsto} B$

> [!example] Esempio
> $$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\ \mathrm{II} + \lambda\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} a & b \\ c + \lambda a & d + \lambda b \end{bmatrix}$$
> $$\det\left(\begin{bmatrix} a & b \\ c + \lambda a & d + \lambda b \end{bmatrix}\right) = a(d + \lambda b) - (c + \lambda a)b = ad + \lambda ab - bc - \lambda ab = \det(A)$$
> [nell'originale i termini $\lambda ab$ sono barrati]

> [!abstract] Teorema (Morale)
> **MORALE:** con la sostituzione il determinante non cambia!!!

> [!note] Osservazione
> Con la multilinearità ([[Proprietà del Determinante]]):
> $$\det\left(\begin{bmatrix} a & b \\ c + \lambda a & d + \lambda b \end{bmatrix}\right) = \det\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) + \lambda \det\left(\begin{bmatrix} a & b \\ a & b \end{bmatrix}\right)$$
> [annotazioni: il primo addendo è $\det(A)$; il secondo termine $\det\left(\begin{bmatrix} a & b \\ a & b \end{bmatrix}\right)$ è accompagnato da «$= 0\,?$» → [[Proprietà del Determinante]]]

## Determinante con righe uguali

> [!abstract] Teorema (Proprietà)
> Se una matrice ha due righe (o due colonne) uguali allora il determinante è $0$.

> [!example] Esempio (caso $2 \times 2$)
> $$B = \begin{bmatrix} a & b \\ a & b \end{bmatrix} \xrightarrow{\ \mathrm{I} \leftrightarrow \mathrm{II}\ } \begin{bmatrix} a & b \\ a & b \end{bmatrix} = B'$$
> $B = B'$ (perché le righe sono uguali).
> (ALTERNANZA, [[Proprietà del Determinante]]) $\quad \det(B') = -\det(B)$
> $$\left.\begin{matrix} B = B' \\ \det(B') = -\det(B) \end{matrix}\right\} \Rightarrow \det(B) = -\det(B) \Rightarrow 2\det(B) = 0 \Rightarrow \det(B) = 0$$

Uso nella proprietà di sostituzione: [[Proprietà del Determinante]].

---
Precedente: [[Calcolo del Determinante con il MEG]]
