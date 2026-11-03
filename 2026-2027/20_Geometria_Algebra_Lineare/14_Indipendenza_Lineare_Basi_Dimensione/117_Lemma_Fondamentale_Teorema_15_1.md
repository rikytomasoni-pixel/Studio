---
tags: [GAL, dimensione, lemma, teorema, dimostrazione, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 120-121)"
---

# Lemma fondamentale (Teorema 15.1)

> [!abstract] Teorema 15.1 (lemma fondamentale)
> **Ipotesi:**
> - $(V,+,\cdot)$ spazio vettoriale su un campo $\mathbb{K}$;
> - $T=\{\underline{v}_1,\dots,\underline{v}_m\}\subseteq V$ [[96_Insieme_di_Generatori|insieme di generatori]];
> - $S=\{\underline{w}_1,\dots,\underline{w}_n\}\subseteq V$ con $n>m$.
>
> **Tesi:** $S$ è un insieme di vettori [[98_Vettori_Linearmente_Indipendenti|linearmente dipendenti]].

In parole: se $V$ è generato da $m$ vettori, **ogni** insieme con più di $m$ vettori è linearmente dipendente.

## Dimostrazione
Sono interessato a studiare le combinazioni lineari
$$\lambda_1\underline{w}_1+\dots+\lambda_n\underline{w}_n=\underline{0}\qquad(\bigstar)$$
Per dimostrare la tesi devo far vedere che la soluzione di questo problema **non è unica**.

$T$ è un insieme di generatori, quindi ogni $\underline{w}_j$ si scrive come combinazione lineare di $\underline{v}_1,\dots,\underline{v}_m$:
$$\underline{w}_1=a_{11}\underline{v}_1+\dots+a_{m1}\underline{v}_m,\quad\dots,\quad\underline{w}_n=a_{1n}\underline{v}_1+\dots+a_{mn}\underline{v}_m$$

Sostituisco nella combinazione lineare ($\bigstar$) e raccolgo rispetto a $\underline{v}_1,\dots,\underline{v}_m$:
$$\lambda_1\left(a_{11}\underline{v}_1+\dots+a_{m1}\underline{v}_m\right)+\dots+\lambda_n\left(a_{1n}\underline{v}_1+\dots+a_{mn}\underline{v}_m\right)=\underline{0}$$
$$(a_{11}\lambda_1+\dots+a_{1n}\lambda_n)\,\underline{v}_1+(\dots)\,\underline{v}_2+\dots+(a_{m1}\lambda_1+\dots+a_{mn}\lambda_n)\,\underline{v}_m=\underline{0}$$

Se tutti i coefficienti tra parentesi sono nulli, la combinazione è nulla. Considero quindi il **sistema omogeneo** ($m$ equazioni, $n$ incognite $\lambda_1,\dots,\lambda_n$):
$$(\ast)\quad\begin{cases}a_{11}\lambda_1+\dots+a_{1n}\lambda_n=0\\ \quad\vdots\\ a_{m1}\lambda_1+\dots+a_{mn}\lambda_n=0\end{cases}$$

Ogni soluzione di $(\ast)$ è anche soluzione di ($\bigstar$): l'insieme delle soluzioni di $(\ast)$ è contenuto nell'insieme delle soluzioni del problema iniziale ($\bigstar$).
$$\operatorname{Sol}(\ast)\subseteq\operatorname{Sol}(\bigstar)\qquad\Longrightarrow\qquad(\ast)\text{ ha infinite soluzioni}\ \Rightarrow\ (\bigstar)\text{ ha infinite soluzioni}$$

Devo allora dimostrare che il sistema $(\ast)$ ha infinite soluzioni, cioè che $r(A)<n$, dove $A=(a_{ij})\in M_{\mathbb{K}}(m,n)$ è la matrice dei coefficienti:
$$r(A)\le\min(m,n)=m<n$$
$\Rightarrow$ per il [[82_Teorema_di_Rouche_Capelli|teorema di Rouché-Capelli]] ci sono almeno $n-m>0$ parametri liberi
$\Rightarrow$ i vettori $\{\underline{w}_1,\dots,\underline{w}_n\}$ sono **linearmente dipendenti**. $\blacksquare$

> [!note] Osservazione (non presente negli appunti)
> - "Infinite soluzioni" vale su campi infiniti come $\mathbb{R}$. Su un campo finito (es. [[31_Il_Campo_F2]]) $(\ast)$ ha comunque più di una soluzione (almeno $|\mathbb{K}|^{\,n-m}>1$), quindi la soluzione nulla non è l'unica e la conclusione non cambia.
> - Il diagramma a due insiemi concentrici della slide (blu: soluzioni di $(\ast)$, verde: soluzioni del problema iniziale) è reso qui con l'inclusione $\operatorname{Sol}(\ast)\subseteq\operatorname{Sol}(\bigstar)$.

## Note collegate
- [[96_Insieme_di_Generatori]]
- [[98_Vettori_Linearmente_Indipendenti]]
- [[82_Teorema_di_Rouche_Capelli]]
- [[63_Rango_di_una_Matrice]]
- Successiva: [[118_Teorema_della_Dimensione_Teorema_15_2]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/dimensione/lemma-fondamentale
