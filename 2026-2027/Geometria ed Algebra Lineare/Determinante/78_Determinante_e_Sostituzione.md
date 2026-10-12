---
tags: [GAL, matrici, determinante, proprieta, sostituzione, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 71)"
---

# Determinante e operazione di sostituzione

**SOSTITUZIONE** — $A \overset{R_i + \lambda R_k \to R_i}{\leadsto} B$

> [!example] Esempio
> $$\begin{bmatrix} a & b \\ c & d \end{bmatrix} \xrightarrow{\ \mathrm{II} + \lambda\,\mathrm{I} \to \mathrm{II}\ } \begin{bmatrix} a & b \\ c + \lambda a & d + \lambda b \end{bmatrix}$$
> $$\det\left(\begin{bmatrix} a & b \\ c + \lambda a & d + \lambda b \end{bmatrix}\right) = a(d + \lambda b) - (c + \lambda a)b = ad + \lambda ab - bc - \lambda ab = \det(A)$$
> [nell'originale i termini $\lambda ab$ sono barrati]

> [!abstract] Teorema (Morale)
> **MORALE:** con la sostituzione il determinante non cambia!!!

> [!note] Osservazione
> Con la multilinearità ([[77_Determinante_Multilineare]]):
> $$\det\left(\begin{bmatrix} a & b \\ c + \lambda a & d + \lambda b \end{bmatrix}\right) = \det\left(\begin{bmatrix} a & b \\ c & d \end{bmatrix}\right) + \lambda \det\left(\begin{bmatrix} a & b \\ a & b \end{bmatrix}\right)$$
> [annotazioni: il primo addendo è $\det(A)$; il secondo termine $\det\left(\begin{bmatrix} a & b \\ a & b \end{bmatrix}\right)$ è accompagnato da «$= 0\,?$» → [[79_Determinante_con_Righe_Uguali]]]

## Note collegate
- [[77_Determinante_Multilineare]]
- [[79_Determinante_con_Righe_Uguali]]
- [[67_Operazioni_Elementari_sulle_Righe]]
- [[75_Calcolo_del_Determinante_con_il_MEG]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]
