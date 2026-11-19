---
tags: [GAL, applicazioni-lineari, matrice-rappresentativa, cambio-di-base, definizione, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 188-189)"
---

# Matrice del cambio di base (Definizione 23.1)

## Relazione tra due matrici rappresentative di una applicazione lineare
$L:V\to W$. In $V$ due basi $\mathcal{B}_1$ e $\mathcal{B}_2$; in $W$ due basi $\mathcal{e}_1$ e $\mathcal{e}_2$. Ci sono quattro matrici rappresentative, che corrispondono alle quattro frecce $\mathbb{K}^n\to\mathbb{K}^m$ del diagramma:

$$M_{\mathcal{B}_1}^{\mathcal{e}_1}(L)\qquad M_{\mathcal{B}_2}^{\mathcal{e}_1}(L)\qquad M_{\mathcal{B}_1}^{\mathcal{e}_2}(L)\qquad M_{\mathcal{B}_2}^{\mathcal{e}_2}(L)$$

> [!warning] DISEGNO NON RAPPRESENTABILE (slide 188-189)
> Cerca nelle slide: il diagramma con $V\xrightarrow{L}W$ in alto; da $V$ partono $\mathcal{X}_{\mathcal{B}_2}$ e $\mathcal{X}_{\mathcal{B}_1}$ verso due copie di $\mathbb{K}^n$; da $W$ partono $\mathcal{X}_{\mathcal{e}_2}$ e $\mathcal{X}_{\mathcal{e}_1}$ verso due copie di $\mathbb{K}^m$. Le quattro frecce colorate tra le copie di $\mathbb{K}^n$ e $\mathbb{K}^m$ sono: viola $M_{\mathcal{B}_1}^{\mathcal{e}_1}(L)$, arancione $M_{\mathcal{B}_2}^{\mathcal{e}_1}(L)$, verde $M_{\mathcal{B}_1}^{\mathcal{e}_2}(L)$, rossa $M_{\mathcal{B}_2}^{\mathcal{e}_2}(L)$. Nella slide 188 il lato sinistro ($V$ con le due copie di $\mathbb{K}^n$) è evidenziato in azzurro; nella slide 189 compaiono in blu anche le frecce di cambio di base $M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})$ tra le copie di $\mathbb{K}^n$ e $M_{\mathcal{e}_2}^{\mathcal{e}_1}(\mathrm{id})$ tra le copie di $\mathbb{K}^m$.

## Il lato sinistro del diagramma
Concentriamoci sul lato sinistro: $V$ con le due mappe delle coordinate $\mathcal{X}_{\mathcal{B}_2}$ e $\mathcal{X}_{\mathcal{B}_1}$ verso $\mathbb{K}^n$. Cerco la freccia $\mathbb{K}^n\overset{?}{\dashrightarrow}\mathbb{K}^n$ che trasforma coordinate rispetto a $\mathcal{B}_2$ in coordinate rispetto a $\mathcal{B}_1$. È la matrice rappresentativa della funzione identità:
$$\begin{array}{ccc}
V&\xlongequal{\ \ \mathrm{id}\ \ }&V\\
\mathcal{X}_{\mathcal{B}_2}\downarrow&&\downarrow\mathcal{X}_{\mathcal{B}_1}\\
\mathbb{K}^n&\overset{M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})}{\dashrightarrow}&\mathbb{K}^n
\end{array}$$

> [!abstract] Definizione 23.1 (matrice del cambio di base)
> Date due basi $\mathcal{B}_1$ e $\mathcal{B}_2$ di uno spazio vettoriale $V$, la matrice $M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})$ che rappresenta la funzione identità rispetto a $\mathcal{B}_2$ (dominio) e $\mathcal{B}_1$ (codominio) si dice **matrice del cambio di base da $\mathcal{B}_2$ a $\mathcal{B}_1$**.

## Proprietà
- $\mathcal{B}_1\neq\mathcal{B}_2\ \Rightarrow\ M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})\neq\mathrm{Id}_n$.
- $M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})$ è **invertibile** e $\ M_{\mathcal{B}_2}^{\mathcal{B}_1}(\mathrm{id})^{-1}=M_{\mathcal{B}_1}^{\mathcal{B}_2}(\mathrm{id})$.
- Relazioni tra $M_{\mathcal{B}_1}^{\mathcal{e}_1}(L)$ e $M_{\mathcal{B}_1}^{\mathcal{e}_2}(L)$ (stessa base nel dominio, cambia la base nel codominio):
$$M_{\mathcal{B}_1}^{\mathcal{e}_1}(L)=M_{\mathcal{e}_2}^{\mathcal{e}_1}(\mathrm{id})\,M_{\mathcal{B}_1}^{\mathcal{e}_2}(L)$$
$$M_{\mathcal{B}_1}^{\mathcal{e}_2}(L)=M_{\mathcal{e}_2}^{\mathcal{e}_1}(\mathrm{id})^{-1}\,M_{\mathcal{B}_1}^{\mathcal{e}_1}(L)$$

> [!todo] Per casa
> Scrivere tutte le relazioni tra due matrici rappresentative di $L$ (non svolto).

## Note collegate
- [[165_Dipendenza_della_Matrice_Rappresentativa_dalle_Basi]]
- [[162_Matrice_Rappresentativa_Definizione_22_1]]
- [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]]
- [[171_Endomorfismi_e_Matrici_Rappresentative]]
- [[60_Matrice_Invertibile]]
- [[141_Composizione_e_Inversione_di_Applicazioni_Lineari]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/matrice-rappresentativa/cambio-di-base
