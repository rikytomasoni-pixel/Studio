---
tags: [GAL, applicazioni-lineari, nucleo, iniettivita, lezione-20]
data: 2026-11-12
lezione: 20
fonte: "GAL 2026-2027 - 20261112 - LEZIONE 20.pdf (slide 166)"
---

# Nucleo di un'applicazione lineare

## Iniettività: due formulazioni
$L:V\to W$ **iniettivo** $\iff$
- (I) $L(\underline{v}_1)=L(\underline{v}_2)\Rightarrow\underline{v}_1=\underline{v}_2$
- (II) $\underline{v}_1\neq\underline{v}_2\Rightarrow L(\underline{v}_1)\neq L(\underline{v}_2)$

$L$ applicazione lineare **iniettiva** $\Rightarrow$ $L(\underline{0}_V)=\underline{0}_W$ e inoltre
$$\underline{v}\neq\underline{0}_V\Rightarrow L(\underline{v})\neq\underline{0}_W.$$

## Definizione / notazione
$L:V\to W$ applicazione lineare.
$$\ker(L)=L^{-1}(\{\underline{0}_W\})=\{\underline{v}\in V\mid L(\underline{v})=\underline{0}_W\}$$
si chiama **nucleo** di $L$ (è il caso particolare di controimmagine di $\{\underline{0}_W\}$ visto in [[146_Immagine_e_Controimmagine_di_Sottospazi_Vettoriali]]: è un sottospazio di $V$).

## Esempio: $L_A$
$L_A:\mathbb{K}^n\to\mathbb{K}^m$, $A\in M_{\mathbb{K}}(m,n)$:
$$\ker(L_A)=\{\underline{v}\in\mathbb{K}^n\mid L_A(\underline{v})=\underline{0}\}=\{\underline{v}\in\mathbb{K}^n\mid A\underline{v}=\underline{0}\}=\{\underline{v}\in\mathbb{K}^n\mid\text{soluzioni di }A\underline{x}=\underline{0}\}=\ker(A)$$

## Note collegate
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[152_Teorema_20_1_Criterio_di_Iniettivita]]
- [[146_Immagine_e_Controimmagine_di_Sottospazi_Vettoriali]]
- [[18_Iniettivita_Suriettivita_Biettivita]]
- [[139_Proprieta_delle_Applicazioni_Lineari]]
- Indice: [[21_Indice_Lezione_20]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/nucleo
