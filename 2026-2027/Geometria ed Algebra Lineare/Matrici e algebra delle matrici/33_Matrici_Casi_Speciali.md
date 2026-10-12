---
tags: [GAL, matrici, notazione, vettori-riga-colonna, lezione-3]
data: 2026-09-30
lezione: 3
fonte: "GAL_2026-2027_-_20260930_-_LEZIONE_3.pdf (slide 27-28)"
---

# Notazione e casi speciali di matrici

> [!warning] Def. Insieme $M_{\mathbb{K}}(m,n)$
> $M_{\mathbb{K}}(m,n) = \{\text{matrici di tipo } (m,n) \text{ (}m\text{ righe e }n\text{ colonne) con valori in } \mathbb{K}\}$ ([[32_Definizione_di_Matrice]]).

- **$m = 1,\ n = 1$:** $M_{\mathbb{K}}(1,1) = \{[a_{11}] \mid a_{11} \in \mathbb{K}\}$.
  $M_{\mathbb{K}}(1,1) \overset{1:1}{\longleftrightarrow} \mathbb{K}$, con $[a_{11}] \mapsto a_{11}$ e $[k] \leftarrow k$ — **funzione biettiva** ([[18_Iniettivita_Suriettivita_Biettivita]]).

- **$m = 1,\ n > 1$:**
  $M_{\mathbb{K}}(1,n) = \{[a_{11}\ a_{12}\ \dots\ a_{1n}] \mid a_{1j} \in \mathbb{K}\ \forall j\} = \{\text{vettori riga di lunghezza } n\}$

> [!note] Osservazione
> N.B. $M_{\mathbb{K}}(1,n) \overset{1:1}{\longleftrightarrow} \underbrace{\mathbb{K} \times \mathbb{K} \times \cdots \times \mathbb{K}}_{n \text{ volte}}$: vettori riga di lunghezza $n$ $\leftrightarrow$ lista ordinata di lunghezza $n$ ([[19_Prodotto_Cartesiano_di_Piu_Insiemi]]).
> $[a_{11}\ \dots\ a_{1n}] \mapsto (a_{11}, \dots, a_{1n})$, $\quad [k_1\ k_2\ \dots\ k_n] \leftarrow (k_1, k_2, \dots, k_n)$
> $M_{\mathbb{K}}(1,n) = \mathbb{K}^n$, $\quad M_{\mathbb{K}}(1,n) \cong \mathbb{K}^n$

- **$m > 1,\ n = 1$:**
  $$M_{\mathbb{K}}(m,1) = \left\{ \begin{bmatrix} a_{11} \\ a_{21} \\ \vdots \\ a_{m1} \end{bmatrix} \,\middle|\, a_{i1} \in \mathbb{K}\ \forall i \right\} = \{\text{vettori colonna di altezza } m\}$$
  $M_{\mathbb{K}}(m,1) \cong \mathbb{K}^m$ — liste ordinate di $m$ elementi in $\mathbb{K}$.

- **$m = n$:**
  $M_{\mathbb{K}}(n,n) = M_{\mathbb{K}}(n) = \{\text{matrici quadrate di ordine } n\}$

## Note collegate
- [[32_Definizione_di_Matrice]]
- [[19_Prodotto_Cartesiano_di_Piu_Insiemi]]
- [[18_Iniettivita_Suriettivita_Biettivita]]
- [[34_Confronto_e_Uguaglianza_tra_Matrici]]
- Indice: [[04_Indice_Lezione_3]] · [[00_MOC_GAL]]
