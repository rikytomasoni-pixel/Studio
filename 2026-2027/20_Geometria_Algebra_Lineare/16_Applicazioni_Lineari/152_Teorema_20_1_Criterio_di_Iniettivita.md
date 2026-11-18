---
tags: [GAL, applicazioni-lineari, iniettivita, nucleo, teorema, dimostrazione, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 166-167)"
---

# Teorema 20.1 (criterio di iniettività)

> [!abstract] Teorema 20.1
> Data un'applicazione lineare $L:V\to W$, le seguenti affermazioni sono tra loro equivalenti:
> - (I) $L$ iniettiva
> - (II) $\ker(L)=\{\underline{0}_V\}$

## Dimostrazione
**(I) $\Rightarrow$ (II).** HP: $L$ iniettivo. TH: $\ker(L)=\{\underline{0}\}$.
Vale $\underline{0}_V\in\ker(L)$. Per l'iniettività,
$$\underline{v}\neq\underline{0}_V\Rightarrow L(\underline{v})\neq L(\underline{0}_V)=\underline{0}_W\Rightarrow\underline{v}\notin\ker(L)\ \Rightarrow\ \ker(L)=\{\underline{0}_V\}.$$

**(II) $\Rightarrow$ (I).** HP: $\ker(L)=\{\underline{0}_V\}$. TH: $L$ iniettivo.
Prendo $\underline{v}_1,\underline{v}_2\in V$ tali che $L(\underline{v}_1)=L(\underline{v}_2)$:
$$L(\underline{v}_1)=L(\underline{v}_2)\iff L(\underline{v}_1)-L(\underline{v}_2)=\underline{0}_W\iff L(\underline{v}_1-\underline{v}_2)=\underline{0}_W\iff\underline{v}_1-\underline{v}_2\in\ker(L)\overset{\text{HP}}{\iff}\underline{v}_1-\underline{v}_2=\underline{0}_V\iff\underline{v}_1=\underline{v}_2\qquad\blacksquare$$

## Conseguenze per $L_A$
$L_A:\mathbb{K}^n\to\mathbb{K}^m$, $A\in M_{\mathbb{K}}(m,n)$: vedi [[153_Conseguenze_del_Criterio_di_Iniettivita_L_A_e_Rango]].

## Note collegate
- [[151_Nucleo_di_una_Applicazione_Lineare]]
- [[154_Corollario_20_2_Iniettivita_e_Indipendenza_Lineare]]
- [[155_Teorema_20_3_Teorema_della_Fibra]]
- [[139_Proprieta_delle_Applicazioni_Lineari]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/criterio-iniettivita
