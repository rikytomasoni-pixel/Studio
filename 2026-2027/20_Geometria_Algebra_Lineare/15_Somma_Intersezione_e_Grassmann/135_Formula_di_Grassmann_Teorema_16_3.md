---
tags: [GAL, sottospazi, dimensione, grassmann, teorema, dimostrazione, lezione-16]
data: 2026-11-04
lezione: 16
fonte: "GAL 2026-2027 - 20261104 - LEZIONE 16.pdf (slide 141-144)"
---

# Formula di Grassmann (Teorema 16.3)

> [!abstract] Teorema 16.3 (formula di Grassmann)
> **Ipotesi.** $(V,+,\cdot)$ spazio vettoriale su un campo $\mathbb{K}$; $H_1,H_2$ sottospazi vettoriali finitamente generati.
>
> **Tesi.**
> $$\dim(H_1+H_2)=\dim(H_1)+\dim(H_2)-\dim(H_1\cap H_2)$$

## Dimostrazione
Osservo che l'ipotesi $H_1,H_2$ finitamente generati garantisce che anche $H_1\cap H_2$ e $H_1+H_2$ siano finitamente generati.

Devo costruire una **base per ogni sottospazio coinvolto** nell'equazione. Parto dal sottospazio più piccolo: $H_1\cap H_2$. Suppongo $\dim(H_1\cap H_2)=n$, cioè
$$H_1\cap H_2=\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)\qquad\underline{v}_1,\dots,\underline{v}_n\text{ generatori linearmente indipendenti}$$

**Base di $H_1$.** $H_1\cap H_2\subseteq H_1$. Costruisco una base di $H_1$ partendo dalla base di $H_1\cap H_2$ e completandola (cioè aggiungendo i vettori necessari, [[125_Completamento_ad_una_Base]]):
$$\mathcal{B}=\{\underline{v}_1,\dots,\underline{v}_n\}\ \text{base di }H_1\cap H_2,\qquad\mathcal{B}_1=\mathcal{B}\cup\{\underline{w}_1,\dots,\underline{w}_p\}\ \text{base di }H_1\ \Rightarrow\ \dim(H_1)=n+p$$

**Base di $H_2$.** In maniera analoga, completando la base di $H_1\cap H_2$:
$$\mathcal{B}_2=\mathcal{B}\cup\{\underline{u}_1,\dots,\underline{u}_q\}\ \text{base di }H_2\ \Rightarrow\ \dim(H_2)=n+q$$

![[SchemaGrassmann.png]]

**Sostituzione nella formula.**
$$\dim(H_1+H_2)\overset{?}{=}\dim(H_1)+\dim(H_2)-\dim(H_1\cap H_2)=(n+p)+(n+q)-n=n+p+q$$
Per concludere devo esibire una **base di $H_1+H_2$ formata da $n+p+q$ elementi**.

**Generatori di $H_1+H_2$.** Applico la definizione di sottospazio somma ([[134_Unione_di_Sottospazi_e_Sottospazio_Somma]]): $H_1+H_2$ è generato dall'unione di due insiemi di generatori di $H_1$ e $H_2$:
$$H_1+H_2=\operatorname{Span}(\mathcal{B}_1\cup\mathcal{B}_2)=\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n,\underline{w}_1,\dots,\underline{w}_p,\cancel{\underline{v}_1,\dots,\underline{v}_n},\underline{u}_1,\dots,\underline{u}_q)=\operatorname{Span}(\underbrace{\underline{v}_1,\dots,\underline{v}_n}_{n},\underbrace{\underline{w}_1,\dots,\underline{w}_p}_{p},\underbrace{\underline{u}_1,\dots,\underline{u}_q}_{q})$$

**Indipendenza lineare.** Devo mostrare che i vettori generatori rimasti non hanno ulteriore ridondanza, cioè sono linearmente indipendenti. Considero la combinazione lineare
$$x_1\underline{v}_1+\dots+x_n\underline{v}_n+y_1\underline{w}_1+\dots+y_p\underline{w}_p+z_1\underline{u}_1+\dots+z_q\underline{u}_q=\underline{0}\qquad(\bigstar)$$
Chiamo $\underline{z}$ il vettore $z_1\underline{u}_1+\dots+z_q\underline{u}_q$.
- $\underline{z}\in\operatorname{Span}(\underline{u}_1,\dots,\underline{u}_q)\Rightarrow\underline{z}\in H_2$.
- Da $(\bigstar)$: $\underline{z}=-(x_1\underline{v}_1+\dots+x_n\underline{v}_n+y_1\underline{w}_1+\dots+y_p\underline{w}_p)\in\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n,\underline{w}_1,\dots,\underline{w}_p)\Rightarrow\underline{z}\in H_1$.

Quindi $\underline{z}\in H_1\cap H_2$. Allora scrivo $\underline{z}$ mediante la base di $H_1\cap H_2$:
$$\underline{z}\in\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)\ \Rightarrow\ \underline{z}=\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n$$
$$z_1\underline{u}_1+\dots+z_q\underline{u}_q=\underline{z}=\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n\ \Rightarrow\ z_1\underline{u}_1+\dots+z_q\underline{u}_q-\lambda_1\underline{v}_1-\dots-\lambda_n\underline{v}_n=\underline{0}$$
$\{\underline{v}_1,\dots,\underline{v}_n,\underline{u}_1,\dots,\underline{u}_q\}$ è la base $\mathcal{B}_2$ di $H_2$, quindi i vettori sono linearmente indipendenti $\Rightarrow z_1=\dots=z_q=0$ (e $\lambda_1=\dots=\lambda_n=0$).

Sostituisco in $(\bigstar)$:
$$x_1\underline{v}_1+\dots+x_n\underline{v}_n+y_1\underline{w}_1+\dots+y_p\underline{w}_p+0\underline{u}_1+\dots+0\underline{u}_q=\underline{0}$$
$\{\underline{v}_1,\dots,\underline{v}_n,\underline{w}_1,\dots,\underline{w}_p\}$ sono linearmente indipendenti (base $\mathcal{B}_1$ di $H_1$) $\Rightarrow x_1=\dots=x_n=y_1=\dots=y_p=0$.

Quindi $\{\underline{v}_1,\dots,\underline{v}_n,\underline{w}_1,\dots,\underline{w}_p,\underline{u}_1,\dots,\underline{u}_q\}$ è una base di $H_1+H_2$ con $n+p+q$ elementi. $\blacksquare$

## Note collegate
- [[134_Unione_di_Sottospazi_e_Sottospazio_Somma]]
- [[133_Intersezione_di_Sottospazi_Vettoriali]]
- [[132_Significato_della_Dimensione_Seconda_Parte]]
- [[118_Teorema_della_Dimensione_Teorema_15_2]]
- [[125_Completamento_ad_una_Base]]
- [[100_Base_di_uno_Spazio_Vettoriale]]
- [[98_Vettori_Linearmente_Indipendenti]]
- Indice: [[17_Indice_Lezione_16]] · [[00_MOC_GAL]]

#GAL/sottospazi/grassmann
