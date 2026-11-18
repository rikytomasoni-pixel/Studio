---
tags: [GAL, applicazioni-lineari, fibra, controimmagine, nucleo, teorema, dimostrazione, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 169-170)"
---

# Teorema 20.3 (teorema della fibra)

> [!abstract] Teorema 20.3 (della fibra)
> **HP:** $L:V\to W$ applicazione lineare; dato $\underline{w}\in\mathrm{im}(L)\subseteq W$, sia $\underline{v}_0\in L^{-1}(\underline{w})$ (cioè $L(\underline{v}_0)=\underline{w}$).
>
> **TH:** tutte e sole le controimmagini di $\underline{w}$ sono della forma $\underline{v}_0+\underline{v}_H$ con $\underline{v}_H\in\ker(L)$, cioè
> $$L^{-1}(\underline{w})=\underline{v}_0+\ker(L)=\{\underline{v}_0+\underline{v}_H\mid\underline{v}_H\in\ker(L)\}.$$

## Osservazioni
- "**Fibra** di $\underline{w}$" significa "insieme delle controimmagini di $\underline{w}$".
- Se $L$ è iniettiva, allora $\ker(L)=\{\underline{0}_V\}$ e per il teorema della fibra $\forall\,\underline{w}\in\mathrm{im}(L)$ $\exists\,\underline{v}_0$ t.c. $L(\underline{v}_0)=\underline{w}$ e $L^{-1}(\underline{w})=\underline{v}_0+\underline{v}_H$ con $\underline{v}_H\in\ker(L)$, cioè $L^{-1}(\underline{w})=\{\underline{v}_0\}$ (**un'unica** controimmagine).
- Il [[85_Teorema_di_Struttura_delle_Soluzioni|teorema di struttura delle soluzioni]] di un sistema lineare è un caso particolare di questo teorema con $L=L_A$.

## Dimostrazione
Devo mostrare $L^{-1}(\underline{w})=\{\underline{v}_0+\underline{v}_H\mid\underline{v}_H\in\ker(L)\}$, cioè le due inclusioni:

**(I)** $\{\underline{v}_0+\underline{v}_H\mid\underline{v}_H\in\ker(L)\}\subseteq L^{-1}(\underline{w})$.
$\underline{v}_0\in L^{-1}(\underline{w})$ per ipotesi, $\underline{v}_H\in\ker(L)$. Allora
$$L(\underline{v}_0+\underline{v}_H)\overset{\text{ADD}}{=}L(\underline{v}_0)+L(\underline{v}_H)=\underline{w}+\underline{0}_W=\underline{w}\ \Rightarrow\ \underline{v}_0+\underline{v}_H\in L^{-1}(\underline{w}).$$

**(II)** $L^{-1}(\underline{w})\subseteq\{\underline{v}_0+\underline{v}_H\mid\underline{v}_H\in\ker(L)\}$.
Sia $\underline{v}_1\in L^{-1}(\underline{w})$ (nuova controimmagine) e $\underline{v}_0\in L^{-1}(\underline{w})$ (per ipotesi):
$$L(\underline{v}_1-\underline{v}_0)=L(\underline{v}_1)-L(\underline{v}_0)=\underline{w}-\underline{w}=\underline{0}_W\ \Rightarrow\ \underline{v}_H:=\underline{v}_1-\underline{v}_0\in\ker(L)$$
$$\underline{v}_1-\underline{v}_0=\underline{v}_H\iff\underline{v}_1=\underline{v}_0+\underline{v}_H\qquad\blacksquare$$

![[VisualizzazioneThmFibra.png]]

## Note collegate
- [[85_Teorema_di_Struttura_delle_Soluzioni]]
- [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[152_Teorema_20_1_Criterio_di_Iniettivita]]
- [[146_Immagine_e_Controimmagine_di_Sottospazi_Vettoriali]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/teorema-fibra
