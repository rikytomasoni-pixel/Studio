---
tags: [GAL, sistemi-lineari, determinante, parametri, cramer, strategia]
data: 2026-10-27
lezione: esercizi
fonte: "Osservazione redatta da Claude, non presente negli appunti (collega le note 86 e 88)"
---

# Strategia: determinante per sistemi quadrati con parametro

> [!note] Osservazione (non presente negli appunti)
> Negli appunti il [[86_Teorema_di_Cramer]] è formulato col **rango** ($r(A)=n$), e il [[88_Teorema_sull_Invertibilita_della_Matrice]] dice $r(A)=n\iff\det(A)\neq0$. Dalla loro combinazione ricavo una strategia, che **non è scritta** negli appunti come regola a sé.

## Catena di implicazioni
$$\det(A)\neq0\ \overset{88}{\Longrightarrow}\ r(A)=n\ \overset{86}{\Longrightarrow}\ \text{soluzione esiste ed è unica }\forall\underline{b}$$

## Procedura per $A\underline{x}=\underline{b}$ con $A$ quadrata $n\times n$ dipendente da un parametro
1. Calcolo $\det(A)$ in funzione del parametro.
2. Per i valori con $\det(A)\neq0$: soluzione unica, nulla da fare.
3. Per ciascun valore con $\det(A)=0$ sostituisco e studio il sistema a parte con [[82_Teorema_di_Rouche_Capelli]] (confronto $r(A)$ e $r(A|\underline{b})$, ad es. col MEG: [[73_MEG_e_Rango]]).

## Cautele
- $\det(A)=0$ **non** significa sistema impossibile: può essere impossibile ([[113_Esercizio_5_4_i_Determinante_Sempre_Nullo]], $a\neq0$) o indeterminato ([[114_Esercizio_5_4_ii_Cramer_e_Caso_Singolare]], $a=-2$).
- Se la matrice non è quadrata ([[115_Esercizio_5_4_iii_Quattro_Equazioni_Tre_Incognite]]) il determinante non si applica: si usa l'eliminazione o il confronto dei ranghi.
- La formula esplicita $x_i=\det(A_i)/\det(A)$ **non** compare negli appunti.

## Note collegate
- [[112_Esercizio_5_4_Sistemi_con_Parametro]]
- [[86_Teorema_di_Cramer]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[83_Esempio_Sistema_con_Parametro_k_e_Rouche_Capelli]]

#GAL/sistemi-lineari/strategia-determinante-parametro
