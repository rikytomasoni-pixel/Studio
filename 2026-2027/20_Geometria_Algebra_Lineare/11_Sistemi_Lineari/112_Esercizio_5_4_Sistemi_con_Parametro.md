---
tags: [GAL, sistemi-lineari, esercizio, parametri, rouche-capelli]
data: 2026-10-27
lezione: esercizi
fonte: "Esercizio 5.4 (testo fornito in chat); svolgimento redatto da Claude, non presente negli appunti"
---

# Esercizio 5.4: sistemi con parametro

> [!question] Testo (Esercizio 5.4)
> Determina per quali valori del parametro $a\in\mathbb{R}$ i seguenti sistemi hanno *almeno* una soluzione.
>
> **(i)** $\begin{cases}y+az=1\\ ax-y=a-1\\ x+y+(1+a)z=1\end{cases}$
>
> **(ii)** $\begin{cases}(a+5)x+y=1\\ 2x+2ay+az=a^2\\ -x+2y+z=a\end{cases}$
>
> **(iii)** $\begin{cases}x_1+x_2+ax_3=1\\ x_1+x_2+a^3x_3=3\\ 2x_1+x_2+2x_3=0\\ x_1+x_2+x_3=0\end{cases}$

> [!note] Osservazione (non presente negli appunti)
> Lo svolgimento di tutte le note di questo esercizio è mio: gli appunti non contengono questo esercizio. Metodo: [[82_Teorema_di_Rouche_Capelli]] (almeno una soluzione $\iff r(A)=r(A|\underline{b})$) e, per i sistemi quadrati, [[116_Strategia_Determinante_per_Sistemi_con_Parametro]].

## Risultati

| Sistema | Valori di $a$ con almeno una soluzione | Soluzioni | Nota |
|---|---|---|---|
| (i) | $a=0$ | $\infty^1$ | [[113_Esercizio_5_4_i_Determinante_Sempre_Nullo]] |
| (ii) | $\forall a\in\mathbb{R}$ | unica se $a\neq-2$, $\infty^1$ se $a=-2$ | [[114_Esercizio_5_4_ii_Cramer_e_Caso_Singolare]] |
| (iii) | $a=-2$ | unica: $\left(\tfrac13,0,-\tfrac13\right)$ | [[115_Esercizio_5_4_iii_Quattro_Equazioni_Tre_Incognite]] |

## Note collegate
- [[82_Teorema_di_Rouche_Capelli]]
- [[83_Esempio_Sistema_con_Parametro_k_e_Rouche_Capelli]]
- [[86_Teorema_di_Cramer]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- [[116_Strategia_Determinante_per_Sistemi_con_Parametro]]
- [[00_MOC_GAL]]

#GAL/sistemi-lineari/esercizio-5-4
