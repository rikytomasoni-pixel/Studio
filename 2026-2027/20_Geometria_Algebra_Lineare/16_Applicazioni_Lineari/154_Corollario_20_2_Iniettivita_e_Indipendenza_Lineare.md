---
tags: [GAL, applicazioni-lineari, iniettivita, indipendenza-lineare, dimostrazione, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 168)"
---

# Corollario 20.2: iniettività e indipendenza lineare

> [!abstract] Corollario 20.2
> **HP:** $L:V\to W$ applicazione lineare **iniettiva**; $\{\underline{v}_1,\dots,\underline{v}_n\}$ vettori linearmente indipendenti.
>
> **TH:** $\{L(\underline{v}_1),\dots,L(\underline{v}_n)\}$ vettori linearmente indipendenti.

> [!abstract] Morale
> L'iniettività di un'applicazione lineare conserva la proprietà di **essere linearmente indipendenti**.

## Dimostrazione
$$\lambda_1L(\underline{v}_1)+\dots+\lambda_nL(\underline{v}_n)=\underline{0}_W\ \overset{L\ \text{lineare}}{\iff}\ L(\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n)=\underline{0}_W\iff\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n\in\ker(L)$$
$$\overset{L\ \text{iniettivo}}{\Rightarrow}\ \lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n=\underline{0}_V\ \overset{\text{IND. LIN.}}{\Rightarrow}\ \lambda_1=\dots=\lambda_n=0\qquad\blacksquare$$

(Analogo, per l'iniettività, di [[149_Conseguenze_della_Suriettivita_Generatori_e_Dimensione]], dove la suriettività conserva i generatori.)

## Note collegate
- [[152_Teorema_20_1_Criterio_di_Iniettivita]]
- [[148_Proposizione_19_1_Immagine_dei_Generatori]]
- [[98_Vettori_Linearmente_Indipendenti]]
- [[156_Isomorfismi_Definizione_20_4_e_Conservazione_delle_Basi]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/iniettivita-indipendenza
