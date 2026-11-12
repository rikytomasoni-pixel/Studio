---
tags: [GAL, applicazioni-lineari, composizione, inversa, prodotto-matriciale, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 151-152)"
---

# Composizione e inversione di applicazioni lineari

## Ulteriori proprietà
- La **composizione** di applicazioni lineari è un'applicazione lineare.
- La **funzione inversa** di un'applicazione lineare invertibile è un'applicazione lineare.

## La composizione è il prodotto matriciale
$$\mathbb{K}^n\xrightarrow{\ L_A\ }\mathbb{K}^m\xrightarrow{\ L_B\ }\mathbb{K}^p\qquad A\in M_{\mathbb{K}}(m,n),\quad B\in M_{\mathbb{K}}(p,m)$$
$\forall\underline{v}\in\mathbb{K}^n$:
$$(L_B\circ L_A)(\underline{v})=L_B\big(L_A(\underline{v})\big)=L_B(A\underline{v})=B(A\underline{v})=(BA)\underline{v}=L_{BA}(\underline{v})$$

> [!abstract] Morale
> $$L_B\circ L_A=L_{BA}$$
> cioè il **prodotto matriciale codifica la composizione di applicazioni lineari**.

(Vedi [[42_Prodotto_e_Composizione_di_Funzioni]] per l'analoga osservazione di L4.)

## La matrice inversa codifica la funzione inversa
Osservazione: $\mathrm{Id}_n\in M_{\mathbb{K}}(n,n)$, $\forall\underline{v}\in\mathbb{K}^n$
$$L_{\mathrm{Id}_n}(\underline{v})=\mathrm{Id}_n\underline{v}=\underline{v}\ \Rightarrow\ L_{\mathrm{Id}_n}=\mathrm{id}$$

$L_A:\mathbb{K}^n\to\mathbb{K}^m$ è invertibile $\iff$ $A$ è invertibile. Se $A\in M_{\mathbb{K}}(n,n)$ è invertibile:
$$\begin{cases}L_A\circ L_{A^{-1}}=L_{AA^{-1}}=L_{\mathrm{Id}_n}=\mathrm{id}\\ L_{A^{-1}}\circ L_A=L_{A^{-1}A}=L_{\mathrm{Id}_n}=\mathrm{id}\end{cases}\ \Rightarrow\ L_{A^{-1}}=(L_A)^{-1}$$

> [!abstract] Morale
> Calcolare la matrice inversa è utile per calcolare le funzioni inverse!

> [!note] Osservazione (non presente negli appunti)
> Sulla slide l'equivalenza "$L_A$ invertibile $\iff$ $A$ invertibile" è scritta con $A\in M_{\mathbb{K}}(m,n)$; l'invertibilità di una matrice ha senso per matrici quadrate ($m=n$), come nella parte successiva della slide.

## Note collegate
- [[156_Isomorfismi_Definizione_20_4_e_Conservazione_delle_Basi]] (isomorfismi)
- [[41_Prodotto_Matriciale_Righe_per_Colonne]]
- [[42_Prodotto_e_Composizione_di_Funzioni]]
- [[60_Matrice_Invertibile]]
- [[87_Ricerca_della_Matrice_Inversa]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- [[137_Esempi_di_Applicazioni_Lineari_Matrici_Trasposizione_Traccia]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/composizione-inversa
