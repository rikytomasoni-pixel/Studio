---
created: 2026-10-01
materia: GAL
tags:
  - stato/da-revisionare
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/prodotto_matriciale
aliases: []
origine: UpdateVault
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Prodotto Righe per Colonne

> [!warning] Def. Prodotto matriciale righe per colonne
> $$\cdot : M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(n,p) \to M_{\mathbb{K}}(m,p),\qquad (A,B) \mapsto AB$$
> - $A = [a_{ij}]$, $i = 1,\dots,m$, $j = 1,\dots,n$
> - $B = [b_{ij}]$, $i = 1,\dots,n$, $j = 1,\dots,p$
> - $C = AB = [c_{ij}]$, $i = 1,\dots,m$, $j = 1,\dots,p$
> $$c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \dots + a_{in}b_{nj} = \sum_{k=1}^{n} a_{ik}\, b_{kj}$$


> [!example] Esempio 1
> $A \in M_{\mathbb{K}}(1,n)$, $B \in M_{\mathbb{K}}(n,1)$: $A = [a_{11}\ a_{12}\ \dots\ a_{1n}]$, $B = \begin{bmatrix} b_{11} \\ b_{21} \\ \vdots \\ b_{n1} \end{bmatrix}$
> $AB = C \in M_{\mathbb{K}}(1,1)$, $C = [c_{11}]$
> $$c_{11} = \sum_{k=1}^{n} a_{1k}\, b_{k1} = a_{11}b_{11} + a_{12}b_{21} + \dots + a_{1n}b_{n1}$$

> [!example] Esempio 2
> $$A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \in M_{\mathbb{K}}(2,2), \qquad B = \begin{bmatrix} 0 & 1 & -1 \\ 0 & -1 & 2 \end{bmatrix} \in M_{\mathbb{K}}(2,3), \qquad AB = C \in M_{\mathbb{K}}(2,3)$$
> - $c_{11} = [1\ \ 2]\begin{bmatrix} 0 \\ 0 \end{bmatrix} = (1\cdot0) + (2\cdot0) = 0$
> - $c_{12} = [1\ \ 2]\begin{bmatrix} 1 \\ -1 \end{bmatrix} = 1\cdot1 + 2\cdot(-1) = 1 - 2 = -1$
> - $c_{13} = [1\ \ 2]\begin{bmatrix} -1 \\ 2 \end{bmatrix} = 1\cdot(-1) + 2\cdot2 = -1 + 4 = 3$
> - $c_{21} = [3\ \ 4]\begin{bmatrix} 0 \\ 0 \end{bmatrix} = 3\cdot0 + 4\cdot0 = 0$
> - $c_{22} = [3\ \ 4]\begin{bmatrix} 1 \\ -1 \end{bmatrix} = 3\cdot1 + 4(-1) = 3 - 4 = -1$
> - $c_{23} = [3\ \ 4]\begin{bmatrix} -1 \\ 2 \end{bmatrix} = 3\cdot(-1) + 4\cdot2 = -3 + 8 = 5$
>
> $$AB = \begin{bmatrix} 0 & -1 & 3 \\ 0 & -1 & 5 \end{bmatrix}$$


> [!note] Osservazione (Domanda)
> D. perché tutto questo? → [[Prodotto e Composizione di Funzioni]]

---
Precedente: [[Opposto di una Matrice]] · Successivo: [[Prodotto e Composizione di Funzioni]]
