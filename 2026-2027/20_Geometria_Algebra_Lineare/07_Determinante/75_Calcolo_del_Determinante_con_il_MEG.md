---
tags: [GAL, matrici, determinante, MEG, triangolari, lezione-7]
data: 2026-10-08
lezione: 7
fonte: "GAL_2026-2027_-_20261008_-_LEZIONE_7.pdf (slide 69)"
---

# Calcolo del determinante con il MEG

> [!note] Osservazione
> $A \in M_{\mathbb{K}}(n,n) \overset{\text{MEG}}{\leadsto} U \in M_{\mathbb{K}}(n,n)$ a scala ([[68_Metodo_di_Eliminazione_di_Gauss]]); $U$ è triangolare superiore ([[66_Matrici_Triangolari]]).
> $$A = ZU = Z \begin{bmatrix} u_{11} & \cdots & u_{1n} \\ 0 & u_{22} & & \ast \\ \vdots & & \ddots & \\ 0 & \cdots & 0 & u_{nn} \end{bmatrix}$$
> $$\det(A) = \det(Z)\det(U) = \det(Z)\, u_{11}u_{22}\cdots u_{nn}$$
> (primo passaggio per il [[74_Teorema_di_Binet]]; $Z$ come in [[72_Esistenza_della_Matrice_Inversa]])

> [!example] Esempio numerico
> Con $U$ ottenuta usando solo scambi di righe e sostituzioni vale $\det(A)=(-1)^s\,u_{11}\cdots u_{nn}$, con $s$ numero di scambi ([[76_Determinante_Normalizzato_e_Alternante]], [[78_Determinante_e_Sostituzione]]). Esempio completo con $\det=-25$: [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]]; confronto con gli altri metodi: [[107_Confronto_Metodi_Calcolo_Determinante]].

## Note collegate
- [[74_Teorema_di_Binet]]
- [[66_Matrici_Triangolari]]
- [[72_Esistenza_della_Matrice_Inversa]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- [[103_Esercizio_5_1_Calcolo_del_Determinante]]
- [[104_Determinante_con_il_MEG_Esempio_con_Scambio_di_Righe]]
- [[107_Confronto_Metodi_Calcolo_Determinante]]
- Indice: [[08_Indice_Lezione_7]] · [[00_MOC_GAL]]

#GAL/determinante/calcolo-del-determinante-con-il-meg
