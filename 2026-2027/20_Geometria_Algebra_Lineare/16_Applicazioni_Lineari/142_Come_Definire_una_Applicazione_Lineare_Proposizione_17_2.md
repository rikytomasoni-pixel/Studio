---
tags: [GAL, applicazioni-lineari, base, proposizione, dimostrazione, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 152-153)"
---

# Come definire un'applicazione lineare (Proposizione 17.2)

> [!abstract] Proposizione 17.2
> **Ipotesi.**
> - $V,W$ spazi vettoriali finitamente generati su un campo $\mathbb{K}$
> - $\mathcal{B}=\{\underline{v}_1,\dots,\underline{v}_n\}$ base di $V$
> - $S=\{\underline{w}_1,\dots,\underline{w}_n\}$ vettori (ordinati) di $W$
>
> **Tesi.** Esiste un'**unica** applicazione lineare $L:V\to W$ tale che
> $$L(\underline{v}_1)=\underline{w}_1,\ \dots,\ L(\underline{v}_n)=\underline{w}_n$$

> [!note] Osservazioni
> - L'**ordine** degli elementi è cruciale.
> - Posso controllare interamente la funzione mediante il controllo di un numero **finito** di elementi.

## Dimostrazione
Voglio calcolare l'immagine di un vettore $\underline{v}\in V$ arbitrario.

**(I)** So che $\mathcal{B}$ è una base di $V$, quindi (unica rappresentazione possibile, [[101_Teorema_di_Unicita_della_Rappresentazione_rispetto_a_una_Base]])
$$\underline{v}=\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n\qquad\lambda_i\in\mathbb{K}$$

**(II)** Uso le proprietà di $L$:
$$L(\underline{v})=L(\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n)\overset{\text{ADD}}{=}L(\lambda_1\underline{v}_1)+\dots+L(\lambda_n\underline{v}_n)\overset{\text{OMO}}{=}\lambda_1L(\underline{v}_1)+\dots+\lambda_nL(\underline{v}_n)$$

**(III)** Uso l'associazione prescritta dall'enunciato:
$$L(\underline{v})=\lambda_1\underline{w}_1+\lambda_2\underline{w}_2+\dots+\lambda_n\underline{w}_n\qquad\blacksquare$$

> [!note] Osservazione (non presente negli appunti)
> I passi (I)-(III) mostrano che **se** $L$ esiste, allora l'immagine di ogni $\underline{v}$ è forzata (unicità) e vale la formula $L(\underline{v})=\sum\lambda_i\underline{w}_i$. Per l'esistenza basta controllare che questa formula, con $\lambda_i$ le coordinate di $\underline{v}$ rispetto a $\mathcal{B}$, definisca davvero una funzione additiva e omogenea: le coordinate sono univoche e si sommano/scalano come i vettori.

## Applicazioni
- [[143_Esempio_Applicazione_Lineare_da_Polinomi_a_Matrici]]
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]

## Note collegate
- [[136_Applicazioni_Lineari_Definizione_17_1]]
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[101_Teorema_di_Unicita_della_Rappresentazione_rispetto_a_una_Base]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/definizione-su-base
