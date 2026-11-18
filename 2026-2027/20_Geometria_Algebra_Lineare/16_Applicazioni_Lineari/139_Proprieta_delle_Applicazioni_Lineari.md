---
tags: [GAL, applicazioni-lineari, proprieta, combinazioni-lineari, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 148-149)"
---

# Proprietà delle applicazioni lineari

## Conservazione delle combinazioni lineari
Un'applicazione lineare $L:V\to W$ **conserva le combinazioni lineari**: $\forall\underline{v}_1,\dots,\underline{v}_k\in V$, $\forall\lambda_1,\dots,\lambda_k\in\mathbb{K}$
$$L(\lambda_1\underline{v}_1+\dots+\lambda_k\underline{v}_k)\overset{\text{ADD}}{=}L(\lambda_1\underline{v}_1)+L(\lambda_2\underline{v}_2)+\dots+L(\lambda_k\underline{v}_k)\overset{\text{OMO}}{=}\lambda_1L(\underline{v}_1)+\dots+\lambda_kL(\underline{v}_k)$$

## $L(-\underline{v})=-L(\underline{v})$
$$L(-\underline{v})=L\big((-1)\underline{v}\big)\overset{\text{OMO}}{=}(-1)L(\underline{v})=-L(\underline{v})$$

## $L(\underline{0}_V)=\underline{0}_W$
$$L(\underline{0}_V)=L\big(\underline{v}+(-1)\underline{v}\big)\overset{\text{ADD}}{=}L(\underline{v})+L\big((-1)\underline{v}\big)\overset{\text{OMO}}{=}L(\underline{v})+(-1)L(\underline{v})=L(\underline{v})-L(\underline{v})=\underline{0}_W$$

> [!abstract] Conseguenza
> $L:V\to W$ applicazione lineare $\Rightarrow$ $L(\underline{0}_V)=\underline{0}_W$.
>
> Per contrapposizione: $L:V\to W$ **NON** è un'applicazione lineare $\Leftarrow$ $L(\underline{0}_V)\neq\underline{0}_W$.

La condizione $L(\underline{0}_V)=\underline{0}_W$ è quindi **necessaria ma non sufficiente** (vedi i controesempi in [[140_Esempi_e_Controesempi_di_Applicazioni_Lineari]]).

## Note collegate
- [[136_Applicazioni_Lineari_Definizione_17_1]]
- [[140_Esempi_e_Controesempi_di_Applicazioni_Lineari]]
- [[93_Proprieta_Fondamentali_degli_Spazi_Vettoriali]]
- [[95_Combinazioni_Lineari_e_Span]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/proprieta
