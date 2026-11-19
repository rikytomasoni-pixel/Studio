---
tags: [GAL, applicazioni-lineari, nucleo, immagine, rango, dimensione, teorema, dimostrazione, nullita-piu-rango, lezione-22]
data: 2026-11-18
lezione: 22
fonte: "GAL 2026-2027 - 20261118 - LEZIONE 22.pdf (slide 181)"
---

# Teorema 22.2 (teorema di nullità più rango)

> [!abstract] Teorema 22.2 (di nullità + rango)
> **HP:** $V,W$ spazi vettoriali finitamente generati; $L:V\to W$ applicazione lineare.
>
> **TH:** $$\dim V=\dim\ker(L)+\dim\operatorname{im}(L).$$

## Dimostrazione
Considero $\ker(L)\subseteq V$ e $\operatorname{im}(L)\subseteq W$, e porto tutto in $\mathbb{K}^n,\mathbb{K}^m$ con la matrice rappresentativa $A=M_{\mathcal{B}}^{\mathcal{C}}(L)$ ([[162_Matrice_Rappresentativa_Definizione_22_1]]):

$$\begin{array}{ccc}
\ker(L)\subseteq V&\xrightarrow{\ \ L\ \ }&W\supseteq\operatorname{im}(L)\\
\mathcal{X}_{\mathcal{B}}\downarrow\uparrow\mathcal{P}_{\mathcal{B}}&&\mathcal{X}_{\mathcal{C}}\downarrow\uparrow\mathcal{P}_{\mathcal{C}}\\
\ker(A)=\ker(L_A)\subseteq\mathbb{K}^n&\xrightarrow{\ \ L_A\ \ }&\mathbb{K}^m\supseteq\operatorname{im}(L_A)=\operatorname{col}(A)
\end{array}$$

Le mappe delle coordinate sono **invertibili** e quindi "conservano le basi" ([[156_Isomorfismi_Definizione_20_4_e_Conservazione_delle_Basi]]): $\mathcal{X}_{\mathcal{B}}$ corrisponde $\ker(L)$ a $\ker(L_A)$ e $\mathcal{X}_{\mathcal{C}}$ corrisponde $\operatorname{im}(L)$ a $\operatorname{im}(L_A)$.

**A livello matriciale:**
$$\dim\ker(L_A)=\dim\ker(A)=\#\text{parametri liberi che descrivono le soluzioni di }A\underline{x}=\underline{0}$$
$$\overset{\text{TEO R.C.}}{=}\#\text{incognite}-\#\text{vincoli}=n-r(A)=\dim(\mathbb{K}^n)-\dim\operatorname{col}(A)$$
([[82_Teorema_di_Rouche_Capelli]]), cioè
$$\dim\ker(L_A)=\dim(\mathbb{K}^n)-\dim\operatorname{im}(L_A)\ \Longrightarrow\ \dim(\mathbb{K}^n)=\dim\ker(L_A)+\dim\operatorname{im}(L_A).$$

Riporto il risultato su $V$ e $W$ con $\mathcal{P}_{\mathcal{B}}$ e $\mathcal{P}_{\mathcal{C}}$ (che conservano le dimensioni):
$$\dim V=\dim\ker(L)+\dim\operatorname{im}(L)\qquad\blacksquare$$

## Note collegate
- [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[147_Immagine_di_una_Applicazione_Lineare_e_Suriettivita]]
- [[153_Conseguenze_del_Criterio_di_Iniettivita_L_A_e_Rango]]
- [[150_Suriettivita_di_L_A_e_Spazio_delle_Colonne]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- Indice: [[23_Indice_Lezione_22]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/nullita-piu-rango
