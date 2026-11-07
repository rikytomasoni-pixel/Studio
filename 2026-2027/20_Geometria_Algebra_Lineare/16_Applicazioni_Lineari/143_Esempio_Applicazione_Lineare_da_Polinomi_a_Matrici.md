---
tags: [GAL, applicazioni-lineari, esempio, polinomi, matrici, base, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 153-154)"
---

# Esempio 1: applicazione lineare $\mathbb{R}[t]_{\le2}\to M_{\mathbb{R}}(2,2)$

$$V=\mathbb{R}[t]_{\le2}\qquad W=M_{\mathbb{R}}(2,2)$$
Come definisco $L:\mathbb{R}[t]_{\le2}\to M_{\mathbb{R}}(2,2)$? Con la [[142_Come_Definire_una_Applicazione_Lineare_Proposizione_17_2|Proposizione 17.2]]: scelgo una base del dominio e assegno l'immagine dei suoi vettori.

- Base: $\mathcal{B}=\{1,\ 1+t,\ 1+t+t^2\}$
- Immagini:
$$L(1)=\begin{bmatrix}1&1\\1&0\end{bmatrix}\qquad L(1+t)=\begin{bmatrix}1&-1\\0&0\end{bmatrix}\qquad L(1+t+t^2)=\begin{bmatrix}0&1\\1&0\end{bmatrix}$$

## Immagine di un polinomio qualsiasi
Devo calcolare l'immagine di $p(t)=a_0+a_1t+a_2t^2$. Serve calcolare la combinazione lineare che descrive $p(t)$ rispetto a $\mathcal{B}$:
$$a_0+a_1t+a_2t^2=\lambda_0(1)+\lambda_1(1+t)+\lambda_2(1+t+t^2)=(\lambda_0+\lambda_1+\lambda_2)+(\lambda_1+\lambda_2)t+\lambda_2t^2$$
$$\begin{cases}a_0=\lambda_0+\lambda_1+\lambda_2\\a_1=\lambda_1+\lambda_2\\a_2=\lambda_2\end{cases}\qquad\left[\begin{array}{ccc|c}1&1&1&a_0\\0&1&1&a_1\\0&0&1&a_2\end{array}\right]\ \ (\text{colonne: }\lambda_0,\lambda_1,\lambda_2)$$
$$\xrightarrow[\ \mathrm{II}-\mathrm{III}\to\mathrm{II}\ ]{\ \mathrm{I}-\mathrm{III}\to\mathrm{I}\ }\left[\begin{array}{ccc|c}1&1&0&a_0-a_2\\0&1&0&a_1-a_2\\0&0&1&a_2\end{array}\right]\xrightarrow{\ \mathrm{I}-\mathrm{II}\to\mathrm{I}\ }\left[\begin{array}{ccc|c}1&0&0&a_0-a_1\\0&1&0&a_1-a_2\\0&0&1&a_2\end{array}\right]$$
Quindi $\lambda_0=a_0-a_1$, $\lambda_1=a_1-a_2$, $\lambda_2=a_2$, e
$$L(a_0+a_1t+a_2t^2)=L\big((a_0-a_1)\cdot1+(a_1-a_2)(1+t)+a_2(1+t+t^2)\big)$$
$$=(a_0-a_1)L(1)+(a_1-a_2)L(1+t)+a_2L(1+t+t^2)$$
$$=(a_0-a_1)\begin{bmatrix}1&1\\1&0\end{bmatrix}+(a_1-a_2)\begin{bmatrix}1&-1\\0&0\end{bmatrix}+a_2\begin{bmatrix}0&1\\1&0\end{bmatrix}$$
$$=\begin{bmatrix}a_0-\cancel{a_1}+\cancel{a_1}-a_2&a_0-a_1-(a_1-a_2)+a_2\\a_0-a_1+a_2&0\end{bmatrix}=\begin{bmatrix}a_0-a_2&a_0-2a_1+2a_2\\a_0-a_1+a_2&0\end{bmatrix}$$

> [!note] Osservazione (non presente negli appunti)
> Verifica sui vettori della base: $p=1$ ($a_0=1,a_1=a_2=0$) dà $\begin{bmatrix}1&1\\1&0\end{bmatrix}$; $p=1+t$ ($a_0=a_1=1,a_2=0$) dà $\begin{bmatrix}1&-1\\0&0\end{bmatrix}$; $p=1+t+t^2$ dà $\begin{bmatrix}0&1\\1&0\end{bmatrix}$, come assegnato.

## Note collegate
- [[142_Come_Definire_una_Applicazione_Lineare_Proposizione_17_2]]
- [[144_Applicazioni_Lineari_da_Kn_a_Km_e_Matrice_Associata]]
- [[81_Risoluzione_di_un_Sistema_con_MEG_Esempio_Parametrico]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/esempio-polinomi
