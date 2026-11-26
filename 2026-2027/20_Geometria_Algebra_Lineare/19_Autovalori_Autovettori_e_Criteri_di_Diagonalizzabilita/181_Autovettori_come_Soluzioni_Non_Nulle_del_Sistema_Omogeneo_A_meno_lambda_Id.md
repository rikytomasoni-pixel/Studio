---
tags: [GAL, autovettori, autovalori, sistemi-omogenei, determinante, rouche-capelli, lezione-25]
data: 2026-11-25
lezione: 25
fonte: "GAL 2026-2027 - 20261125 - LEZIONE 25.pdf (slide 202-203)"
---

# Autovettori come soluzioni non nulle di $(A-\lambda\,\mathrm{Id})\underline x=\underline 0$

Passo 1 dell'[[180_Obiettivo_Concreto_Ricerca_degli_Autovettori_e_Esempio_1|Esempio 1]]: cerco gli autovettori di $L$. Sia $p(t)=a_0+a_1t+a_2t^2+a_3t^3$, con $\mathcal{X}_{\mathcal{B}}(p)=\begin{bmatrix}a_0\\a_1\\a_2\\a_3\end{bmatrix}$.

$p(t)$ è un autovettore di $L$ se esiste $\lambda\in\mathbb{K}$ tale che

$$L(p(t))=\lambda p(t)\iff A\,\mathcal{X}_{\mathcal{B}}(p)=\lambda\,\mathcal{X}_{\mathcal{B}}(p)\iff A\begin{bmatrix}a_0\\a_1\\a_2\\a_3\end{bmatrix}=\lambda\begin{bmatrix}a_0\\a_1\\a_2\\a_3\end{bmatrix}$$

Assomiglia a un **sistema lineare nelle incognite $a_0,\dots,a_3$ dipendente da un parametro $\lambda$**. Infatti

$$A\underline a=\lambda\underline a\iff A\underline a-\lambda\underline a=\underline 0\iff A\underline a-\lambda(\mathrm{Id}_n\underline a)=\underline 0\iff(A-\lambda\mathrm{Id}_n)\,\underline a=\underline 0$$

> [!info] Rappresentazione
> È la rappresentazione del tipo di un **sistema lineare omogeneo** con matrice dei coefficienti $A-\lambda\mathrm{Id}$.

**Obiettivo:** trovare gli autovettori $=$ trovare le soluzioni **non nulle** del sistema.

## Per quali $\lambda$ c'è una soluzione non nulla?

> [!question] Domanda
> Per quali valori di $\lambda\in\mathbb{K}$ il sistema omogeneo con matrice dei coefficienti $A-\lambda\mathrm{Id}$ ha almeno una soluzione non nulla?

**Risposta.**
1. Sto chiedendo almeno 2 soluzioni $\Rightarrow$ sto chiedendo **infinite** soluzioni $\Rightarrow$ sto chiedendo almeno **un parametro libero**.
2. Per [[82_Teorema_di_Rouche_Capelli|Rouché-Capelli]]: $\#\text{parametri liberi}=\#\text{incognite}-r(A-\lambda\mathrm{Id})>0\Rightarrow\#\text{incognite}>r(A-\lambda\mathrm{Id})$, cioè $4>r(A-\lambda\mathrm{Id})$.
3. $r(A-\lambda\mathrm{Id})<4\iff r(A-\lambda\mathrm{Id})$ **non massimo** $\overset{\text{teo. invertibilità}}{\iff}\det(A-\lambda\mathrm{Id})=0$ ([[88_Teorema_sull_Invertibilita_della_Matrice]]).

> [!success] Criterio
> $\lambda\in\mathbb{K}$ è un autovalore di $A\in M_{\mathbb{K}}(n,n)$ $\iff\det(A-\lambda\mathrm{Id})=0$.

## Applicazione all'Esempio 1

$$\det(A-\lambda\mathrm{Id})=\det\begin{bmatrix}-\lambda&-1&0&0\\0&-\lambda&0&0\\0&0&-\lambda&3\\0&0&0&-\lambda\end{bmatrix}=(-\lambda)^4=\lambda^4$$

L'**unico** valore di $\lambda$ per cui avrò infinite soluzioni è $\lambda=0$: gli unici autovettori che posso trovare hanno come autovalore $\lambda=0$ ([[182_Esempio_1_Autovettori_di_Autovalore_0_e_Non_Diagonalizzabilita]]).

## Note collegate
- [[185_Definizione_26_1_Polinomio_Caratteristico]] (il polinomio $\det(A-x\mathrm{Id})$ sarà chiamato polinomio caratteristico)
- [[82_Teorema_di_Rouche_Capelli]]
- [[88_Teorema_sull_Invertibilita_della_Matrice]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[65_Determinante_Sviluppo_di_Laplace]]
- Indice: [[26_Indice_Lezione_25]] · [[00_MOC_GAL]]

#GAL/autovalori/sistema-omogeneo
