---
tags: [GAL, base, teorema, dimostrazione, unicita, lezione-13]
data: 2026-10-19
lezione: 13
fonte: "GAL_2026-2027_-_20261019_-_LEZIONE_13.pdf (slide 117-118)"
---

# Teorema di unicità della rappresentazione rispetto a una base

> [!abstract] Teorema 13.5 (unicità della rappresentazione rispetto a una base)
> **Ipotesi:** $B=\{\underline{v}_1,\dots,\underline{v}_n\}$ è una [[100_Base_di_uno_Spazio_Vettoriale|base]] di $V$.
>
> **Tesi:** ogni vettore $\underline{v}\in V$ si scrive in modo **unico** come combinazione lineare di $\{\underline{v}_1,\dots,\underline{v}_n\}$.

## Dimostrazione
**Esistenza.** I vettori $\{\underline{v}_1,\dots,\underline{v}_n\}$ sono generatori, quindi $V=\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$. Dunque $\forall\,\underline{v}\in V$ esistono $\lambda_1,\dots,\lambda_n\in\mathbb{K}$ tali che
$$\underline{v}=\lambda_1\underline{v}_1+\lambda_2\underline{v}_2+\dots+\lambda_n\underline{v}_n.$$

**Unicità.** Ora devo dimostrare che questa è l'unica rappresentazione. Supponiamo che ce ne siano due:
$$\underline{v}=\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n\qquad\qquad\underline{v}=\mu_1\underline{v}_1+\dots+\mu_n\underline{v}_n$$
Allora
$$\underline{0}=\underline{v}-\underline{v}=(\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n)-(\mu_1\underline{v}_1+\dots+\mu_n\underline{v}_n)=(\lambda_1-\mu_1)\underline{v}_1+(\lambda_2-\mu_2)\underline{v}_2+\dots+(\lambda_n-\mu_n)\underline{v}_n.$$
Per l'**indipendenza lineare** ([[98_Vettori_Linearmente_Indipendenti]]):
$$\lambda_1-\mu_1=0,\ \dots,\ \lambda_n-\mu_n=0\iff\lambda_1=\mu_1,\ \dots,\ \lambda_n=\mu_n\qquad\blacksquare$$

> [!tip] Idea
> Se due rappresentazioni dello stesso vettore differissero, la loro differenza darebbe una combinazione lineare nulla con coefficienti non tutti nulli, contro l'indipendenza lineare.

I coefficienti $\lambda_1,\dots,\lambda_n$ sono quindi univocamente determinati dalla base: risolvono il problema di ambiguità posto in [[97_Esempio_Generatori_di_R3_e_Rappresentazioni_Multiple]].

## Note collegate
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[98_Vettori_Linearmente_Indipendenti]]
- [[96_Insieme_di_Generatori]]
- [[93_Proprieta_Fondamentali_degli_Spazi_Vettoriali]]
- Successiva: [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- Indice: [[14_Indice_Lezione_13]] · [[00_MOC_GAL]]

#GAL/base/unicita-rappresentazione
