---
tags:
  - AM1
  - derivate
  - differenziabilita
  - approssimazione-lineare
  - o-piccolo
  - dimostrazione
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 17-21)"
---

# Differenziabilità e approssimazione lineare

Risposta al Problema 3 di [[121_Problemi_Motivanti_delle_Derivate]].

## Derivabilità riscritta con l'o piccolo
Siano $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$. Osserviamo che $f$ è derivabile in $x_0$ se e solo se
$$\exists\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}=f'(x_0)\in\mathbb{R}$$
$$\iff\lim_{x\to x_0}\Big(\frac{f(x)-f(x_0)}{x-x_0}-f'(x_0)\Big)=0\iff\lim_{x\to x_0}\frac{f(x)-f(x_0)-f'(x_0)(x-x_0)}{x-x_0}=0$$
$$\iff f(x)-f(x_0)-f'(x_0)(x-x_0)=o(x-x_0)\quad\text{per }x\to x_0$$
$$\iff f(x)=f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)\quad\text{per }x\to x_0$$
In particolare ([[106_Asintotico_e_o_piccolo_per_Funzioni]]) se $f'(x_0)\neq0$
$$f(x)-f(x_0)\sim f'(x_0)(x-x_0)\qquad x\to x_0$$

## Definizione
> [!abstract] Definizione — differenziabilità
> Data $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, diremo che $f$ è **differenziabile in $x_0$** se $\exists\,m\in\mathbb{R}$ tale che
> $$f(x)=f(x_0)+m(x-x_0)+o(x-x_0)\qquad\text{per }x\to x_0$$

> [!note] Osservazione
> Questa è la richiesta che esista un polinomio di grado al più $1$ in $x$ che approssima bene la funzione $f(x)$ vicino a $x_0$, nel senso
> $$f(x)-\big(f(x_0)+m(x-x_0)\big)=o(x-x_0)\ \text{ per }x\to x_0,\ \text{ cioè }\ \lim_{x\to x_0}\frac{f(x)-\big(f(x_0)+m(x-x_0)\big)}{x-x_0}=0$$

## Proposizione
> [!abstract] Proposizione (derivabile $\iff$ differenziabile)
> Sia $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$. Allora $f$ è derivabile in $x_0$ se e solo se $f$ è differenziabile in $x_0$. In tal caso
> $$f(x)=f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)\quad\text{per }x\to x_0\qquad(*)$$
> (cioè $m=f'(x_0)$).

**Dimostrazione.** Abbiamo già visto che se $f$ è derivabile allora $f$ è differenziabile in $x_0$ e vale $(*)$, cioè $m=f'(x_0)$.

Viceversa, sia $f$ differenziabile in $x_0$, cioè $\exists\,m\in\mathbb{R}$ tale che $f(x)=f(x_0)+m(x-x_0)+o(x-x_0)$, $x\to x_0$. Ma allora
$$\frac{f(x)-f(x_0)}{x-x_0}=m+\frac{o(x-x_0)}{x-x_0}\qquad x\to x_0$$
$$\Rightarrow\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}=m+0=m\in\mathbb{R}$$
$\Rightarrow$ esiste finito il limite, $f'(x_0)=\displaystyle\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}=m$: $f$ è derivabile in $x_0$ e vale $(*)$. $\square$

## Osservazioni
> [!note] Osservazione — due punti di vista
> Derivabilità e differenziabilità di $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$ in $x_0\in(a,b)$ sono **equivalenti**.
> - Porre l'accento sulla **derivabilità** vuol dire interessarsi al tasso di variazione istantaneo di $y=f(x)$ al variare di $x$ in $x_0$.
> - Porre l'accento sulla **differenziabilità** significa interessarsi al problema di approssimare $f$ con un polinomio di grado al più $1$ in $x$, "vicino" a $x_0$ (cioè per $x\to x_0$).
>
> Le due nozioni **non** sono equivalenti per funzioni di più variabili.

> [!note] Osservazione — miglior approssimazione lineare
> Se $f$ è derivabile/differenziabile in $x_0\in(a,b)$, il miglior polinomio di grado al più $1$ che approssima $f$ per $x\to x_0$ è
> $$y=f(x_0)+f'(x_0)(x-x_0)$$
> espressione analitica della retta tangente al grafico di $f$ in $P_0=(x_0,f(x_0))$.

## Note collegate
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[129_Derivabilita_e_Continuita]]
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[128_Derivate_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/differenziabilita
