---
created: 2026-10-01
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/prodotto_matriciale
aliases: []
---
[[00_GAL_Prodotto_Matriciale|⬅️ Torna a Prodotto Matriciale]]

# Prodotto Righe per Colonne

$$
\cdot : M_{\mathbb{K}}(m,n) \times M_{\mathbb{K}}(n,p) \to M_{\mathbb{K}}(m,p), \qquad (A,B) \longmapsto AB
$$

Il numero di colonne di $A$ deve coincidere con il numero di righe di $B$. Con $A = [a_{ij}]$ ($i=1,\dots,m$; $j=1,\dots,n$), $B = [b_{ij}]$ ($i=1,\dots,n$; $j=1,\dots,p$) e $C = AB = [c_{ij}]$ ($i=1,\dots,m$; $j=1,\dots,p$):

$$
c_{ij} = a_{i1}b_{1j} + a_{i2}b_{2j} + \dots + a_{in}b_{nj} = \sum_{k=1}^{n} a_{ik}\, b_{kj}
$$

### Esempi

**Riga per colonna.** Se $A \in M_{\mathbb{K}}(1,n)$ e $B \in M_{\mathbb{K}}(n,1)$, allora $AB = C \in M_{\mathbb{K}}(1,1)$, $C = [c_{11}]$:

$$
c_{11} = \sum_{k=1}^{n} a_{1k}\, b_{k1} = a_{11}b_{11} + a_{12}b_{21} + \dots + a_{1n}b_{n1}
$$

**Esempio numerico.** $A = \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \in M_{\mathbb{K}}(2,2)$, $B = \begin{bmatrix} 0 & 1 & -1 \\ 0 & -1 & 2 \end{bmatrix} \in M_{\mathbb{K}}(2,3)$, quindi $AB = C \in M_{\mathbb{K}}(2,3)$. L'elemento $c_{ij}$ è il prodotto della riga $i$ di $A$ per la colonna $j$ di $B$:

$$
\begin{aligned}
c_{11} &= \begin{bmatrix}1 & 2\end{bmatrix}\begin{bmatrix}0\\0\end{bmatrix} = 1\cdot 0 + 2\cdot 0 = 0 \\
c_{12} &= \begin{bmatrix}1 & 2\end{bmatrix}\begin{bmatrix}1\\-1\end{bmatrix} = 1\cdot 1 + 2\cdot(-1) = -1 \\
c_{13} &= \begin{bmatrix}1 & 2\end{bmatrix}\begin{bmatrix}-1\\2\end{bmatrix} = 1\cdot(-1) + 2\cdot 2 = 3 \\
c_{21} &= \begin{bmatrix}3 & 4\end{bmatrix}\begin{bmatrix}0\\0\end{bmatrix} = 0 \\
c_{22} &= \begin{bmatrix}3 & 4\end{bmatrix}\begin{bmatrix}1\\-1\end{bmatrix} = 3\cdot 1 + 4\cdot(-1) = -1 \\
c_{23} &= \begin{bmatrix}3 & 4\end{bmatrix}\begin{bmatrix}-1\\2\end{bmatrix} = 3\cdot(-1) + 4\cdot 2 = 5
\end{aligned}
$$

$$
AB = \begin{bmatrix} 0 & -1 & 3 \\ 0 & -1 & 5 \end{bmatrix}
$$

> **Figura (disegno senza immagine disponibile):**
>
> Schema colorato: $A$ (2×2) con la prima riga evidenziata in verde e la seconda in blu; $B$ (2×3) con le tre colonne evidenziate in rosso, viola e giallo; la matrice $C = AB$ (2×3) ha ogni cella all'incrocio tra la striscia-riga di $A$ e la striscia-colonna di $B$ corrispondenti.

---
Precedente: [[Opposto di una Matrice]] · Successivo: [[Prodotto e Composizione di Funzioni]]
