---
tags: [GAL, applicazioni-lineari, immagine, generatori, dimostrazione, lezione-19]
data: 2026-11-11
lezione: 19
fonte: "GAL 2026-2027 - 20261111 - LEZIONE 19.pdf (slide 161-162)"
---

# Proposizione 19.1: immagine di un insieme di generatori

> [!note] Numerazione
> Sulla slide la proposizione è scritta "Proposizione 13.1"; per la numerazione delle lezioni (Lezione 19) è qui indicata come 19.1.

> [!abstract] Proposizione 19.1
> **HP:** $L:V\to W$ applicazione lineare; $\{\underline{v}_1,\dots,\underline{v}_n\}$ è un insieme di generatori di $V$.
>
> **TH:** $\{L(\underline{v}_1),\dots,L(\underline{v}_n)\}$ è un insieme di generatori per $\mathrm{im}(L)$.

## Dimostrazione
Voglio far vedere che
$$\mathrm{im}(L)=\mathrm{Span}\big(L(\underline{v}_1),\dots,L(\underline{v}_n)\big)\iff\begin{cases}\subseteq\\ \supseteq\end{cases}$$

- ($\mathrm{im}(L)\supseteq\mathrm{Span}$) $\forall\,\underline{v}_i\in V$: $L(\underline{v}_i)\in\mathrm{im}(L)=L(V)$ $\Rightarrow$ $\mathrm{Span}\big(L(\underline{v}_1),\dots,L(\underline{v}_n)\big)\subseteq\mathrm{im}(L)$.
- ($\mathrm{im}(L)\subseteq\mathrm{Span}$) $\forall\,\underline{w}\in\mathrm{im}(L)$, cioè $\exists\,\underline{v}\in V$ t.c. $L(\underline{v})=\underline{w}$: poiché gli $\underline{v}_i$ generano $V$, esistono $\lambda_1,\dots,\lambda_n\in\mathbb{K}$ tali che $\underline{v}=\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n$. Allora
$$\underline{w}=L(\underline{v})=L(\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n)\overset{\text{ADD, OMO}}{=}\lambda_1L(\underline{v}_1)+\dots+\lambda_nL(\underline{v}_n)\ \Rightarrow\ \underline{w}\in\mathrm{Span}\big(L(\underline{v}_1),\dots,L(\underline{v}_n)\big)\qquad\blacksquare$$

Conseguenze: [[149_Conseguenze_della_Suriettivita_Generatori_e_Dimensione]].

## Note collegate
- [[147_Immagine_di_una_Applicazione_Lineare_e_Suriettivita]]
- [[96_Insieme_di_Generatori]]
- [[95_Combinazioni_Lineari_e_Span]]
- [[139_Proprieta_delle_Applicazioni_Lineari]]
- Indice: [[20_Indice_Lezione_19]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/immagine-generatori
