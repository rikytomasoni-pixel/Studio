---
tags: [GAL, applicazioni-lineari, suriettivita, generatori, dimensione, lezione-19]
data: 2026-11-11
lezione: 19
fonte: "GAL 2026-2027 - 20261111 - LEZIONE 19.pdf (slide 162-163)"
---

# Conseguenze della suriettività: generatori e dimensione

## Conseguenze della Proposizione 19.1
$L:V\to W$ suriettiva $\iff$ $\mathrm{im}(L)=W$. Se $\{\underline{v}_1,\dots,\underline{v}_n\}$ generatori di $V$, per la [[148_Proposizione_19_1_Immagine_dei_Generatori|proposizione]]:
$$\{L(\underline{v}_1),\dots,L(\underline{v}_n)\}\ \text{generatori di}\ \mathrm{im}(L)=W.$$

> [!abstract] Morale
> Un'applicazione lineare **suriettiva** conserva la proprietà di **essere generatori**!

## Confronto tra dimensioni
Sia $\{\underline{v}_1,\dots,\underline{v}_n\}$ una **base** di $V$ (quindi $\dim V=n$). Allora $\{L(\underline{v}_1),\dots,L(\underline{v}_n)\}$ sono generatori di $\mathrm{im}(L)$; questi **possono essere ridondanti**, quindi
$$\dim\mathrm{im}(L)\le\dim V.$$
Se $L$ è suriettivo, cioè $\mathrm{im}(L)=W$, allora $\dim W\le\dim V$:
$$L:V\to W\ \text{suriettivo}\ \Rightarrow\ \dim W\le\dim V$$

> [!important] Contrapposizione
> $$L:V\to W\ \text{NON suriettivo}\ \Leftarrow\ \dim W>\dim V$$

## Caso delle matrici
$A\in M_{\mathbb{K}}(m,n)$, $L_A:\mathbb{K}^n\to\mathbb{K}^m$:
$$m>n\ \Rightarrow\ L_A\ \text{NON suriettivo}\ \Rightarrow\ L_A\ \text{NON invertibile}\ \Rightarrow\ A\ \text{NON invertibile}$$

## Note collegate
- [[148_Proposizione_19_1_Immagine_dei_Generatori]]
- [[150_Suriettivita_di_L_A_e_Spazio_delle_Colonne]]
- [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]]
- [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- Indice: [[20_Indice_Lezione_19]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/suriettivita-dimensione
