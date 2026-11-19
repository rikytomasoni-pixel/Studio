---
tags:
  - AM1
  - derivate
  - prolungamento-derivata
  - controesempio
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 21-23)"
---

# Osservazioni sul prolungamento della derivata

Teorema: [[148_Teorema_di_Prolungamento_della_Derivata_Prima]].

## Il viceversa è falso

> [!note] Osservazione
> È possibile che **non esista** $\displaystyle\lim_{x\to a^+}f'(x)$ ma che esista $f'_+(a)$.

**Esempio.**
$$f(x)=\begin{cases}x^2\sin\frac1x&x\ne0\\0&x=0\end{cases}$$
- $f$ è continua in $\mathbb{R}$;
- $f$ è derivabile per ogni $x\ne0$, con $f'(x)=2x\sin\frac1x-\cos\frac1x$ per $x\ne0$;
- non esiste $\displaystyle\lim_{x\to0}f'(x)$ (il termine $\cos\frac1x$ oscilla).

Tuttavia
$$f'(0)=\lim_{h\to0}\frac{f(h)-f(0)}{h}=\lim_{h\to0}h\sin\frac1h=0$$
Quindi $f$ è derivabile in $\mathbb{R}$ con
$$f'(x)=\begin{cases}2x\sin\frac1x-\cos\frac1x&x\ne0\\0&x=0\end{cases}$$

![[xquadratosin1sux.png]]

(stesso esempio di [[138_Punti_Stazionari_e_Punti_Critici]]).

## Versioni per la derivata sinistra e per il punto interno

> [!note] Osservazione
> Vale un simile risultato di prolungamento anche per la derivata sinistra $f'_-(b)$ e per $f'(x_0)$:
> $$\exists\lim_{x\to b^-}f'(x)=m\in\overline{\mathbb{R}}\ \Rightarrow\ f'_-(b)=m\qquad(f:(a,b]\to\mathbb{R}\text{ continua, derivabile in }(a,b))$$
> $$\exists\lim_{x\to x_0}f'(x)=m\in\overline{\mathbb{R}}\ \Rightarrow\ f'(x_0)=m\qquad(f:(a,b)\to\mathbb{R}\text{ continua},\ x_0\in(a,b),\ f\text{ derivabile in }(a,x_0)\cup(x_0,b))$$

## La continuità in $x_0$ serve

**Esempio.** Serve che $f$ sia continua in $x_0$:
$$f(x)=(\operatorname{sgn}x)^2=\begin{cases}1&x\ne0\\0&x=0\end{cases}$$
$f'(x)=0$ per ogni $x\ne0$ $\Rightarrow\ \displaystyle\lim_{x\to0}f'(x)=0$. Tuttavia **non esiste** $f'(0)$, perché $f$ non è continua in $x=0$ ([[129_Derivabilita_e_Continuita]]).

## Note collegate
- [[148_Teorema_di_Prolungamento_della_Derivata_Prima]]
- [[149_Dimostrazione_del_Teorema_di_Prolungamento_della_Derivata]]
- [[151_Discontinuita_della_Funzione_Derivata]]
- [[138_Punti_Stazionari_e_Punti_Critici]]
- [[129_Derivabilita_e_Continuita]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/prolungamento-derivata-osservazioni
