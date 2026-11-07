---
tags:
  - AM1
  - limiti-di-funzioni
  - asintotico
  - proposizione
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 8-11)"
---

# Proprietà dell'asintotico (per funzioni)

> [!abstract] Proposizione
> 1. Se $f_1\sim f_2$ e $g_1\sim g_2$ per $x\to x_0$, allora
>    $$f_1\cdot g_1\sim f_2\cdot g_2,\qquad\frac{f_1}{g_1}\sim\frac{f_2}{g_2},\qquad(f_1)^\alpha\sim(f_2)^\alpha\qquad\text{per }x\to x_0$$
>    (con $(f_1)^\alpha,(f_2)^\alpha$ ben definite in un intorno di $x_0$, salvo al più in $x_0$).
> 2. Se $f\sim g$ per $x\to x_0$, allora $\exists\displaystyle\lim_{x\to x_0}f(x)\in\overline{\mathbb{R}}$ se e solo se $\exists\displaystyle\lim_{x\to x_0}g(x)\in\overline{\mathbb{R}}$. Inoltre se i due limiti esistono essi sono uguali.

## Dimostrazione
**1)** Nelle ipotesi, per $x\to x_0$ e per l'algebra dei limiti ([[102_Algebra_dei_Limiti_di_Funzioni]]):
- $\dfrac{f_1(x)g_1(x)}{f_2(x)g_2(x)}=\Big(\dfrac{f_1(x)}{f_2(x)}\Big)\Big(\dfrac{g_1(x)}{g_2(x)}\Big)\to1\cdot1=1\ \Rightarrow\ f_1g_1\sim f_2g_2$
- $\dfrac{f_1(x)/g_1(x)}{f_2(x)/g_2(x)}=\dfrac{f_1(x)\,g_2(x)}{f_2(x)\,g_1(x)}=\Big(\dfrac{f_1(x)}{f_2(x)}\Big)\Big(\dfrac{g_1(x)}{g_2(x)}\Big)^{-1}\to1\ \Rightarrow\ \dfrac{f_1}{g_1}\sim\dfrac{f_2}{g_2}$
- $\dfrac{(f_1(x))^\alpha}{(f_2(x))^\alpha}=\Big(\dfrac{f_1(x)}{f_2(x)}\Big)^\alpha\to1\ \Rightarrow\ (f_1)^\alpha\sim(f_2)^\alpha$

**2)** Per $x\to x_0$ scriviamo $f(x)=\dfrac{f(x)}{g(x)}\cdot g(x)$. Poiché $\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=1$, se $\exists\displaystyle\lim_{x\to x_0}g(x)=\ell\in\overline{\mathbb{R}}$ per algebra dei limiti/aritmetizzazione di $\infty$ vale
$$\lim_{x\to x_0}f(x)=\lim_{x\to x_0}\frac{f(x)}{g(x)}\cdot g(x)=1\cdot\ell=\ell\in\overline{\mathbb{R}}$$
Invertendo i ruoli di $f,g$ e ripetendo l'argomento troviamo che se $\exists\displaystyle\lim_{x\to x_0}f(x)=\ell\in\overline{\mathbb{R}}$ allora $\exists\displaystyle\lim_{x\to x_0}g(x)=\ell\in\overline{\mathbb{R}}$. Segue la tesi. $\square$

> [!warning] Attenzione
> Se $f_1\sim f_2$, $g_1\sim g_2$ per $x\to x_0$, in generale **non** vale
> $$f_1\pm g_1\sim f_2\pm g_2,\qquad\log f_1\sim\log f_2,\qquad e^{f_1}\sim e^{f_2}$$

## Note collegate
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/proprieta-asintotici
