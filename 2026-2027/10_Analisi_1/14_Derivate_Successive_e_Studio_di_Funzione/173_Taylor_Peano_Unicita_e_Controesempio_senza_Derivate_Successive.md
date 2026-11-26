---
tags:
  - AM1
  - taylor
  - resto-di-peano
  - osservazione
  - controesempio
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 3-4, 8-10)"
---

# Unicità del polinomio e controesempio senza derivate successive

## Osservazioni sull'unicità

> [!abstract] Osservazione
> Esiste **al più** un polinomio $Q(x)$ di grado al più $n$ tale che
> $$\lim_{x\to x_0}\frac{f(x)-Q(x)}{(x-x_0)^n}=0\iff f(x)=Q(x)+o\big((x-x_0)^n\big)\quad x\to x_0$$
> Se $f$ è derivabile $n$ volte in $x_0$, ne esiste **uno e uno solo** ed è
> $$Q(x)=P_n(x)=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$$
> (esistenza: [[170_Dimostrazione_del_Teorema_di_Taylor_con_Resto_di_Peano]]).

> [!note] Osservazione (non presente negli appunti)
> Per questo, fissato $n$, i coefficienti di uno sviluppo $f(x)=Q(x)+o((x-x_0)^n)$ sono determinati da $f$: sviluppi ottenuti per altra via (composizione, prodotto di sviluppi) coincidono con quelli di Taylor, come negli esempi [[176_Esempio_Limite_con_Sviluppi_di_Taylor]] e [[177_Esempio_Sviluppo_di_e_alla_x_quadro]].

## Può esistere $Q$ senza che $f$ abbia $n$ derivate

> [!warning] Attenzione
> Può accadere che per $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, esista un polinomio $Q$ di grado al più $n$, con $n\ge2$, tale che $f(x)=Q(x)+o((x-x_0)^n)$ per $x\to x_0$, **senza** che $f$ ammetta $n$ derivate in $x_0$.
> Il caso $n=1$ è particolare: $f$ è derivabile in $x_0$ **se e solo se** è differenziabile in $x_0$.

## Esempio

$$f(x)=\begin{cases}x^2+x^3\sin\dfrac1x&x\ne0\\[2mm]0&x=0\end{cases}$$

- Per $x\to0$: $f(x)=x^2+o(x^2)$. Infatti
  $$\lim_{x\to0}\frac{f(x)-x^2}{x^2}=\lim_{x\to0}x\sin\frac1x=0$$
  e $Q(x)=x^2$ è un polinomio di grado 2.
- $f$ è continua in $\mathbb{R}$, con $f(0)=0$.
- $$f'(x)=\begin{cases}2x+3x^2\sin\dfrac1x-x\cos\dfrac1x&x\ne0\\[2mm]0&x=0\end{cases}$$
  quindi $f$ è derivabile **una volta** in tutto $\mathbb{R}$, con $f'(0)=0$.
- Per $x\ne0$: $f''(x)=2+6x\sin\dfrac1x-4\cos\dfrac1x-\dfrac1x\sin\dfrac1x$.
- $f''(0)$ **non esiste**, perché
  $$\lim_{h\to0}\frac{f'(h)-f'(0)}{h}=\lim_{h\to0}\Big(2+3h\sin\frac1h-\cos\frac1h\Big)\quad\text{non esiste.}$$

Quindi $f$ ammette lo sviluppo di ordine 2 senza essere derivabile due volte in $0$.

## Note collegate
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[170_Dimostrazione_del_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[138_Punti_Stazionari_e_Punti_Critici]] (stesso tipo di funzione, con $x^2\sin\frac1x$)
- [[164_Punti_di_Cambio_di_Concavita]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/unicita-controesempio
