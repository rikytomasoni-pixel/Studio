---
tags: [GAL, sistemi-lineari, nucleo, kernel, sistema-omogeneo, lezione-10]
data: 2026-10-14
lezione: 10
fonte: "GAL_2026-2027_-_20261014_-_LEZIONE_10.pdf (slide 84-85)"
---

# Commenti a Rouché-Capelli: nucleo e sistema omogeneo associato

## Chi contribuisce a cosa nella soluzione?
Nella descrizione delle soluzioni ([[82_Teorema_di_Rouche_Capelli]])
$$\underline{x}=\underline{v}_0+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}\qquad\forall t_i\in\mathbb{K}$$
- $\underline{v}_0$ **dipende sia da $A$ che da $\underline{b}$**;
- $t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$ **dipende solo da $A$**.

## Che cosa dice la parte $t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$?
Posto $\underline{w}=\underline{v}_0+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$:
$$t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}=\underline{w}-\underline{v}_0$$

> [!warning] N.B.
> $\underline{w}$ e $\underline{v}_0$ sono **due soluzioni** di $A\underline{x}=\underline{b}$.

Sostituisco al posto di $\underline{x}$ il vettore $t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$:
$$A\left(t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}\right)=A(\underline{w}-\underline{v}_0)=A\underline{w}-A\underline{v}_0=\underline{b}-\underline{b}=\underline{0}$$

**Recap.** Il vettore $t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$ descrive le soluzioni del sistema lineare $A\underline{x}=\underline{0}$.

## Nomenclatura
> [!abstract] Definizioni
> - $A\underline{x}=\underline{0}$ si dice **sistema omogeneo associato** al sistema lineare $A\underline{x}=\underline{b}$.
> - $S=\{\text{soluzioni di }A\underline{x}=\underline{0}\}=\{\underline{x}=t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}\mid\forall t_i\in\mathbb{K}\}=\ker(A)$, detto **nucleo di $A$**.

Il risultato generale sulla struttura delle soluzioni è nel [[85_Teorema_di_Struttura_delle_Soluzioni]].

## Note collegate
- [[82_Teorema_di_Rouche_Capelli]]
- [[83_Esempio_Sistema_con_Parametro_k_e_Rouche_Capelli]]
- [[85_Teorema_di_Struttura_delle_Soluzioni]]
- [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]
- Indice: [[11_Indice_Lezione_10]] · [[00_MOC_GAL]]

#GAL/sistemi-lineari/nucleo-e-sistema-omogeneo
