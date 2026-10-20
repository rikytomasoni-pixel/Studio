---
tags: [GAL, spazi-vettoriali, generatori, esempio, rouche-capelli, lezione-13]
data: 2026-10-19
lezione: 13
fonte: "GAL_2026-2027_-_20261019_-_LEZIONE_13.pdf (slide 112-113)"
---

# Esempio: generatori di $\mathbb{R}^3$ e rappresentazioni multiple

Sia
$$S=\left\{\begin{bmatrix}1\\0\\0\end{bmatrix},\begin{bmatrix}-2\\1\\0\end{bmatrix},\begin{bmatrix}0\\1\\1\end{bmatrix},\begin{bmatrix}1\\-1\\2\end{bmatrix}\right\}\subseteq\mathbb{R}^3$$

> [!question] $S$ è un insieme di generatori di $\mathbb{R}^3$?

Catena di equivalenze:

1. $\mathbb{R}^3\subseteq\operatorname{Span}\left(\begin{bmatrix}1\\0\\0\end{bmatrix},\begin{bmatrix}-2\\1\\0\end{bmatrix},\begin{bmatrix}0\\1\\1\end{bmatrix},\begin{bmatrix}1\\-1\\2\end{bmatrix}\right)$ ?
2. $\forall\begin{bmatrix}a\\b\\c\end{bmatrix}\in\mathbb{R}^3$: $\begin{bmatrix}a\\b\\c\end{bmatrix}\in\operatorname{Span}(\dots)$ ?
3. $\forall\begin{bmatrix}a\\b\\c\end{bmatrix}\in\mathbb{R}^3$ esistono $\lambda_1,\lambda_2,\lambda_3,\lambda_4\in\mathbb{R}$ tali che
$$\begin{bmatrix}a\\b\\c\end{bmatrix}=\lambda_1\begin{bmatrix}1\\0\\0\end{bmatrix}+\lambda_2\begin{bmatrix}-2\\1\\0\end{bmatrix}+\lambda_3\begin{bmatrix}0\\1\\1\end{bmatrix}+\lambda_4\begin{bmatrix}1\\-1\\2\end{bmatrix}\ ?$$
   (è una *rappresentazione del I tipo* di un sistema, vedi [[95_Combinazioni_Lineari_e_Span]])
4. Il sistema con matrice completa
$$\left[\begin{array}{cccc|c}1&-2&0&1&a\\0&1&1&-1&b\\0&0&1&2&c\end{array}\right]$$
è risolubile?

I pivot sono nelle prime tre colonne (matrice già a scala). Per [[82_Teorema_di_Rouche_Capelli|Rouché-Capelli]] il sistema è risolubile **per ogni** $(a,b,c)$, quindi **$S$ è un insieme di generatori di $\mathbb{R}^3$**.

## Due domande
> [!question] D
> In quanti modi posso rappresentare un vettore di $\mathbb{R}^3$ come combinazione lineare dei vettori di $S$?
>
> **D'.** Quante sono le soluzioni del sistema?

**R.** (uso Rouché-Capelli) $\#\text{variabili}=4$, $\text{rango}=\#\text{pivot}=3$ $\Rightarrow$ c'è $4-3=1$ parametro libero $\Rightarrow$ **infinite soluzioni**.

> [!question] D
> Secondo voi è più un vantaggio o uno svantaggio poter rappresentare ogni elemento in tanti modi?

## Esempio: due rappresentazioni dello stesso vettore
$$\begin{bmatrix}0\\1\\3\end{bmatrix}=\mathbf{1}\begin{bmatrix}1\\0\\0\end{bmatrix}+\mathbf{1}\begin{bmatrix}-2\\1\\0\end{bmatrix}+\mathbf{1}\begin{bmatrix}0\\1\\1\end{bmatrix}+\mathbf{1}\begin{bmatrix}1\\-1\\2\end{bmatrix}=\mathbf{6}\begin{bmatrix}1\\0\\0\end{bmatrix}+\mathbf{4}\begin{bmatrix}-2\\1\\0\end{bmatrix}+(\mathbf{-1})\begin{bmatrix}0\\1\\1\end{bmatrix}+\mathbf{2}\begin{bmatrix}1\\-1\\2\end{bmatrix}$$

> [!important] Obiettivo
> Comunicare i vettori in maniera **efficiente**. Con questo obiettivo, la molteplicità delle rappresentazioni può generare ambiguità e confusione $\Rightarrow$ preferiamo avere una **rappresentazione unica** (se possibile).

Per ottenerla servono vettori [[98_Vettori_Linearmente_Indipendenti|linearmente indipendenti]]; si veda anche [[99_Dipendenza_Lineare_e_Vettori_Ridondanti]] e il [[101_Teorema_di_Unicita_della_Rappresentazione_rispetto_a_una_Base]].

## Note collegate
- [[95_Combinazioni_Lineari_e_Span]]
- [[96_Insieme_di_Generatori]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]
- Successiva: [[98_Vettori_Linearmente_Indipendenti]]
- Indice: [[14_Indice_Lezione_13]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/generatori
