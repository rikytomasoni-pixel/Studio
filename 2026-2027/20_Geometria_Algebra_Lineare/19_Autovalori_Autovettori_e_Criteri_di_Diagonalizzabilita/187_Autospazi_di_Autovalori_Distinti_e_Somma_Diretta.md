---
tags: [GAL, autospazio, autovalori, somma-diretta, grassmann, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 211)"
---

# Autospazi di autovalori distinti: intersezione nulla e somma diretta

> [!abstract] Proposizione
> Siano $\lambda\ne\mu$ due autovalori di $A$. Allora
> $$V_\lambda\cap V_\mu=\{\underline 0\}$$

## Dimostrazione

$$\underline v\in V_\lambda\cap V_\mu\iff\begin{cases}\underline v\in V_\lambda\\\underline v\in V_\mu\end{cases}\iff\begin{cases}A\underline v=\lambda\underline v\\A\underline v=\mu\underline v\end{cases}$$
quindi
$$\underline v\in V_\lambda\cap V_\mu\iff\lambda\underline v=\mu\underline v\iff\lambda\underline v-\mu\underline v=\underline 0\iff(\lambda-\mu)\underline v=\underline 0\ \Rightarrow\ \underline v=\underline 0$$
perché $\lambda-\mu\ne0$. $\square$

## Conseguenza: somma diretta

Per la [[135_Formula_di_Grassmann_Teorema_16_3|formula di Grassmann]]:
$$\dim(V_\lambda+V_\mu)=\dim V_\lambda+\dim V_\mu-\dim(V_\lambda\cap V_\mu)=\dim V_\lambda+\dim V_\mu$$
perché $\dim(V_\lambda\cap V_\mu)=0$: **la somma tra $V_\lambda$ e $V_\mu$ è diretta**, $V_\lambda\oplus V_\mu$.

Se $V_\lambda=\mathrm{Span}(\underline v_1,\dots,\underline v_{g_\lambda})$ e $V_\mu=\mathrm{Span}(\underline w_1,\dots,\underline w_{g_\mu})$ (basi dei due autospazi), allora
$$\{\underline v_1,\dots,\underline v_{g_\lambda},\underline w_1,\dots,\underline w_{g_\mu}\}\ \text{è un insieme di vettori linearmente indipendenti!}$$

> [!tip] Perché serve
> È ciò che garantisce che, mettendo insieme basi di autospazi diversi, si trovano $g_{\lambda_1}+\dots+g_{\lambda_s}$ autovettori indipendenti: base della dimostrazione del [[188_Teorema_26_3_Secondo_Criterio_di_Diagonalizzabilita|secondo criterio]].

## Note collegate
- [[186_Definizione_26_2_Molteplicita_Algebrica_Autospazio_Molteplicita_Geometrica]]
- [[135_Formula_di_Grassmann_Teorema_16_3]]
- [[133_Intersezione_di_Sottospazi_Vettoriali]]
- [[134_Unione_di_Sottospazi_e_Sottospazio_Somma]]
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/autovalori/autospazi-distinti
