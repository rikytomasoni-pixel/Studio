---
tags:
  - AM1
  - serie
  - serie-a-segno-variabile
  - leibniz
  - controesempio
  - confronto-asintotico
data: 2026-10-21
fonte: "AM1 L12 26-27.pdf (pag. 19-21)"
---

# Osservazioni sul criterio di Leibniz

> [!warning] Osservazione 1
> Non si può rimuovere dal criterio di Leibniz ([[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]) l'ipotesi che $a_n$ sia **decrescente**.

> [!warning] Osservazione 2 — il confronto asintotico non funziona con segno misto
> Se $a_n\sim b_n$, $a_n,b_n>0$ e $\displaystyle\sum_{n=1}^\infty(-1)^nb_n$ converge, in generale ciò **non implica** che converga anche $\displaystyle\sum_{n=1}^\infty(-1)^na_n$.
>
> (Il criterio di convergenza del confronto asintotico, [[62_Criterio_del_Confronto_Asintotico_per_Serie]], non funziona con serie a termini di segno misto: funziona solo per serie a termini $\geq0$.)

> [!warning] Osservazione 3
> $a_n\sim b_n$ e $b_n$ monotona, in generale **non implica** che $a_n$ sia monotona.

## Esempio (controesempio alle osservazioni)
$$a_n=\frac{\sqrt n+(-1)^n}{n},\qquad b_n=\frac{1}{\sqrt n}$$

Allora:
- $a_n,b_n\geq0$ (positivi definitivamente);
- $a_n\sim\dfrac{\sqrt n}{n}=\dfrac{1}{\sqrt n}=b_n$;
- $\displaystyle\lim_{n\to\infty}a_n=\lim_{n\to\infty}b_n=0$;
- $b_n$ è decrescente;
- $\Rightarrow\displaystyle\sum_{n=1}^\infty(-1)^nb_n$ converge per Leibniz.

Vediamo ora che $\sum_{n=1}^\infty(-1)^na_n$ **non converge** e che $a_n$ non è monotona. Infatti
$$\sum_{n=1}^\infty(-1)^na_n=\sum_{n=1}^\infty(-1)^n\frac{\sqrt n+(-1)^n}{n}=\sum_{n=1}^\infty\left(\frac{(-1)^n}{\sqrt n}+\frac1n\right)=\underbrace{\sum_{n=1}^\infty\frac{(-1)^n}{\sqrt n}}_{\in\mathbb{R}\ \text{(converge per Leibniz)}}+\underbrace{\sum_{n=1}^\infty\frac1n}_{+\infty\ \text{(serie armonica)}}=+\infty$$
cioè $\sum_{n=1}^\infty(-1)^na_n$ **diverge a $+\infty$**.

- $a_n$ non può essere decrescente, perché altrimenti $\sum(-1)^na_n$ convergerebbe per Leibniz;
- $a_n$ non può essere crescente, perché $a_n>0$ e $\lim a_n=0$.

## Note collegate
- [[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]
- [[62_Criterio_del_Confronto_Asintotico_per_Serie]]
- [[55_Serie_Armonica]]
- [[77_Esempio_Serie_Alternata_con_Parametro_alpha]]
- [[00_MOC_Analisi_1]]

#AM1/serie/osservazioni-leibniz
