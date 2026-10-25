---
tags: [GAL, indipendenza-lineare, esempio, meg, vettore-ridondante, lezione-13]
data: 2026-10-19
lezione: 13
fonte: "GAL_2026-2027_-_20261019_-_LEZIONE_13.pdf (slide 114-117)"
---

# Dipendenza lineare e vettori ridondanti (esempio)

Esempio (come prima, vedi [[97_Esempio_Generatori_di_R3_e_Rappresentazioni_Multiple]]):
$$S=\left\{\begin{bmatrix}1\\0\\0\end{bmatrix},\begin{bmatrix}-2\\1\\0\end{bmatrix},\begin{bmatrix}0\\1\\1\end{bmatrix},\begin{bmatrix}1\\-1\\2\end{bmatrix}\right\}$$

> [!question] $S$ è un insieme di vettori linearmente indipendenti?
> Equivale a chiedersi se il sistema $\lambda_1\begin{pmatrix}1\\ 0\\ 0\end{pmatrix}+\lambda_2\begin{pmatrix}-2\\ 1\\ 0\end{pmatrix}+\lambda_3\begin{pmatrix}0\\ 1\\ 1\end{pmatrix}+\lambda_4\begin{pmatrix}1\\ -1\\ 2\end{pmatrix}=\underline{b}$ ha un'unica soluzione?

**Risposta: NO**, perché lo abbiamo già visto: ogni vettore $\begin{bmatrix}a\\b\\c\end{bmatrix}$ ha infinite rappresentazioni. **$S$ non è un insieme di vettori linearmente indipendenti.**

## Studio delle soluzioni: relazioni tra i vettori
Studiamo le soluzioni del sistema **omogeneo** per indagare le relazioni tra i vettori. Si aggiunge la riga $\lambda_4=t$ (parametro libero) e si applica il [[68_Metodo_di_Eliminazione_di_Gauss|MEG]]:

$$\left[\begin{array}{cccc|c}1&-2&0&1&0\\0&1&1&-1&0\\0&0&1&2&0\\0&0&0&1&t\end{array}\right]
\xrightarrow{\ \text{I}-\text{IV}\to\text{I},\ \text{II}+\text{IV}\to\text{II},\ \text{III}-2\text{IV}\to\text{III}\ }
\left[\begin{array}{cccc|c}1&-2&0&0&-t\\0&1&1&0&t\\0&0&1&0&-2t\\0&0&0&1&t\end{array}\right]$$

$$\xrightarrow{\ \text{II}-\text{III}\to\text{II}\ }
\left[\begin{array}{cccc|c}1&-2&0&0&-t\\0&1&0&0&3t\\0&0&1&0&-2t\\0&0&0&1&t\end{array}\right]
\xrightarrow{\ \text{I}+2\text{II}\to\text{I}\ }
\left[\begin{array}{cccc|c}1&0&0&0&5t\\0&1&0&0&3t\\0&0&1&0&-2t\\0&0&0&1&t\end{array}\right]$$

Quindi $\forall t\in\mathbb{R}$:
$$(5t)\begin{bmatrix}1\\0\\0\end{bmatrix}+(3t)\begin{bmatrix}-2\\1\\0\end{bmatrix}+(-2t)\begin{bmatrix}0\\1\\1\end{bmatrix}+t\begin{bmatrix}1\\-1\\2\end{bmatrix}=\begin{bmatrix}0\\0\\0\end{bmatrix}$$

> [!tip] OSS
> Le soluzioni del sistema omogeneo descrivono le **relazioni** (combinazioni lineari) tra le colonne della matrice dei coefficienti.

Pongo $t=1$ e separo la colonna della variabile indipendente dalle altre:
$$\begin{bmatrix}1\\-1\\2\end{bmatrix}=(-5)\begin{bmatrix}1\\0\\0\end{bmatrix}+(-3)\begin{bmatrix}-2\\1\\0\end{bmatrix}+2\begin{bmatrix}0\\1\\1\end{bmatrix}
\ \Rightarrow\ \begin{bmatrix}1\\-1\\2\end{bmatrix}\in\operatorname{Span}\left(\begin{bmatrix}1\\0\\0\end{bmatrix},\begin{bmatrix}-2\\1\\0\end{bmatrix},\begin{bmatrix}0\\1\\1\end{bmatrix}\right)$$

## Eliminare il vettore ridondante
Sostituendo nella prima rappresentazione di $\begin{bmatrix}0\\1\\3\end{bmatrix}$ (tutti coefficienti $1$):
$$\begin{bmatrix}0\\1\\3\end{bmatrix}=1\underline{v}_1+1\underline{v}_2+1\underline{v}_3+1\left(-5\underline{v}_1-3\underline{v}_2+2\underline{v}_3\right)=(-4)\begin{bmatrix}1\\0\\0\end{bmatrix}+(-2)\begin{bmatrix}-2\\1\\0\end{bmatrix}+3\begin{bmatrix}0\\1\\1\end{bmatrix}$$

e nella seconda (coefficienti $6,4,-1,2$):
$$\begin{bmatrix}0\\1\\3\end{bmatrix}=6\underline{v}_1+4\underline{v}_2+(-1)\underline{v}_3+2\left(-5\underline{v}_1-3\underline{v}_2+2\underline{v}_3\right)=(-4)\underline{v}_1+(-2)\underline{v}_2+3\underline{v}_3$$

Le due rappresentazioni coincidono. Inoltre
$$\operatorname{Span}(\underline{v}_1,\underline{v}_2,\underline{v}_3,\underline{v}_4)=\operatorname{Span}(\underline{v}_1,\underline{v}_2,\underline{v}_3)\ \Rightarrow\ \underline{v}_4=\begin{bmatrix}1\\-1\\2\end{bmatrix}\text{ è un vettore }\textbf{ridondante}.$$

> [!important] Morale
> Se la rappresentazione non è unica, posso rimuovere un vettore. Ripeto fino a raggiungere una collezione di vettori linearmente indipendenti.

## Verifica: i tre vettori rimasti sono indipendenti?
È vero che $\begin{bmatrix}1\\0\\0\end{bmatrix},\begin{bmatrix}-2\\1\\0\end{bmatrix},\begin{bmatrix}0\\1\\1\end{bmatrix}$ sono linearmente indipendenti? Si studia
$$\lambda_1\begin{bmatrix}1\\0\\0\end{bmatrix}+\lambda_2\begin{bmatrix}-2\\1\\0\end{bmatrix}+\lambda_3\begin{bmatrix}0\\1\\1\end{bmatrix}=\begin{bmatrix}0\\0\\0\end{bmatrix}
\quad\leadsto\quad
\left[\begin{array}{ccc|c}1&-2&0&0\\0&1&1&0\\0&0&1&0\end{array}\right]$$
Tre pivot su tre colonne $\Rightarrow$ nessun parametro libero $\Rightarrow$ unica soluzione $\lambda_1=\lambda_2=\lambda_3=0$: **sono linearmente indipendenti**. Essendo anche generatori di $\mathbb{R}^3$, formano una [[100_Base_di_uno_Spazio_Vettoriale|base]].

## Note collegate
- [[98_Vettori_Linearmente_Indipendenti]]
- [[97_Esempio_Generatori_di_R3_e_Rappresentazioni_Multiple]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- Successiva: [[100_Base_di_uno_Spazio_Vettoriale]]
- Indice: [[14_Indice_Lezione_13]] · [[00_MOC_GAL]]

#GAL/indipendenza-lineare/dipendenza
