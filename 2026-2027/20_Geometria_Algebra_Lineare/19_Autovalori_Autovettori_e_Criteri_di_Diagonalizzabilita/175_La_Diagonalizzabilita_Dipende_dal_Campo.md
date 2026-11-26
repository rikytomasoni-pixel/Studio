---
tags: [GAL, diagonalizzabilita, campo, endomorfismi, esempio, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 196)"
---

# La diagonalizzabilità dipende dal campo

> [!abstract] Definizione 23.3 (richiamo)
> Una matrice $A\in M_{\mathbb{K}}(n,n)$ si dice **diagonalizzabile su $\mathbb{K}$** se esiste una matrice diagonale $D\in M_{\mathbb{K}}(n,n)$ simile ad $A$, cioè esiste $P\in M_{\mathbb{K}}(n,n)$ invertibile tale che $D=P^{-1}AP$. ([[174_Matrici_Diagonalizzabili_Definizione_23_3]])

## Osservazioni

- La definizione attribuisce alla diagonalizzabilità una **dipendenza dal campo** sul quale lavoriamo!
- Se consideriamo un **endomorfismo** $L:V\to V$, diremo che $L$ è **diagonalizzabile** se può essere rappresentato da una matrice diagonale ([[171_Endomorfismi_e_Matrici_Rappresentative]]).
- Ripensando agli esempi della scorsa settimana: la matrice della simmetria assiale
  $$A=\begin{bmatrix}\cos(2\theta)&\sin(2\theta)\\\sin(2\theta)&-\cos(2\theta)\end{bmatrix}$$
  è diagonalizzabile su $\mathbb{R}$ ([[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]).

## Esempio: tre domande

$$A=\begin{bmatrix}0&-1\\1&0\end{bmatrix}$$
ha entrate in $\mathbb{Z}\subseteq\mathbb{Q}\subseteq\mathbb{R}\subseteq\mathbb{C}$. Tre domande: $A$ è diagonalizzabile su $\mathbb{Q}$? su $\mathbb{R}$? su $\mathbb{C}$?

Nella slide sono elencate le **possibilità** compatibili con le inclusioni (✓ = diagonalizzabile, ✗ = no):

| | possibilità 1 | possibilità 2 | possibilità 3 | possibilità 4 |
|---|:-:|:-:|:-:|:-:|
| su $\mathbb{Q}$ | ✓ | ✗ | ✗ | ✗ |
| su $\mathbb{R}$ | ✓ | ✓ | ✗ | ✗ |
| su $\mathbb{C}$ | ✓ | ✓ | ✓ | ✗ |

La risposta si trova nelle slide di L26: [[183_Esempio_2_Rotazione_senza_Autovalori_su_Q_e_R]] e [[184_Esempio_2_Diagonalizzazione_della_Rotazione_su_C]].

## Note collegate
- [[174_Matrici_Diagonalizzabili_Definizione_23_3]]
- [[171_Endomorfismi_e_Matrici_Rappresentative]]
- [[167_Simmetria_Assiale_Base_Adattata_e_Matrice_Diagonale]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/diagonalizzabilita/campo
