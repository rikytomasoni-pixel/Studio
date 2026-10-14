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

# Casi Speciali di Matrici

$M_{\mathbb{K}}(m,n) = \{\text{matrici di tipo } (m,n) \text{ (}m\text{ righe e }n\text{ colonne) con valori in } \mathbb{K}\}$.

- **$M_{\mathbb{K}}(1,1)$** $= \{[a_{11}] \mid a_{11} \in \mathbb{K}\}$. C'è una corrispondenza 1:1 (**funzione biettiva**) $M_{\mathbb{K}}(1,1) \leftrightarrow \mathbb{K}$, con $[a_{11}] \mapsto a_{11}$ e $[k] \leftarrow k$.
- **$m=1$, $n>1$**: $M_{\mathbb{K}}(1,n) = \{[a_{11}\ a_{12}\ \dots\ a_{1n}] \mid a_{1j} \in \mathbb{K}\ \forall j\} = \{\text{vettori riga di lunghezza } n\}$.

  > N.B. $M_{\mathbb{K}}(1,n) \overset{1:1}{\longleftrightarrow} \underbrace{\mathbb{K} \times \mathbb{K} \times \dots \times \mathbb{K}}_{n \text{ volte}}$, cioè vettori riga di lunghezza $n$ $\leftrightarrow$ liste ordinate di lunghezza $n$: $[a_{11} \dots a_{1n}] \mapsto (a_{11},\dots,a_{1n})$ e $[k_1\ k_2 \dots k_n] \leftarrow (k_1,k_2,\dots,k_n)$. Quindi $M_{\mathbb{K}}(1,n) = \mathbb{K}^n$ (più precisamente $M_{\mathbb{K}}(1,n) \cong \mathbb{K}^n$).
- **$m>1$, $n=1$**: $M_{\mathbb{K}}(m,1) = \left\{ \begin{bmatrix} a_{11} \\ a_{21} \\ \vdots \\ a_{m1} \end{bmatrix} \,\middle|\, a_{i1} \in \mathbb{K}\ \forall i \right\} = \{\text{vettori colonna di altezza } m\}$, e $M_{\mathbb{K}}(m,1) \cong \mathbb{K}^m$ (liste ordinate di $m$ elementi in $\mathbb{K}$).
- **$m=n$**: $M_{\mathbb{K}}(n,n) = M_{\mathbb{K}}(n) = \{\text{matrici quadrate di ordine } n\}$.

---
Precedente: [[Definizione di Matrice]] · Successivo: [[Uguaglianza tra Matrici]]
