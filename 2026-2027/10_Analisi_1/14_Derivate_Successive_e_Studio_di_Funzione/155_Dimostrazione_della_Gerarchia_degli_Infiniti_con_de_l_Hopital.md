---
tags:
  - AM1
  - derivate
  - de-l-hopital
  - gerarchia-degli-infiniti
  - dimostrazione
  - limiti-di-funzioni
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 17-19)"
---

# Dimostrazione della gerarchia degli infiniti per funzioni (con de l'Hôpital)

Completa [[109_Gerarchia_degli_Infiniti_per_Funzioni]], dove l'enunciato era dato con "dimostrazione con il teorema di de l'Hôpital" ([[152_Teorema_di_de_l_Hopital]]).

> [!info] Notazione
> Nel quaderno gli esponenti sono indicati con lettere diverse rispetto a [[109_Gerarchia_degli_Infiniti_per_Funzioni]] ($x^\alpha=o(a^x)$ e $(\log_ax)^\alpha=o(x^\gamma)$ invece di $x^\beta=o(a^x)$ e $(\log_ax)^\alpha=o(x^\beta)$). Gli enunciati sono gli stessi.

## Passo 1: $x/e^{\beta x}\to0$
$$\lim_{x\to+\infty}\frac{x}{e^{\beta x}}=0\qquad\forall\beta>0$$
vedi [[154_Esempi_di_Applicazione_de_l_Hopital]] (de l'Hôpital una volta).

## Passo 2: potenza contro esponenziale
$$\lim_{x\to+\infty}\frac{x^\alpha}{a^x}=0\qquad\forall\alpha>0,\ \forall a>1$$
$$\lim_{x\to+\infty}\frac{x^\alpha}{a^x}=\lim_{x\to+\infty}\left(\frac{x}{a^{x/\alpha}}\right)^\alpha=\lim_{x\to+\infty}\left(\frac{x}{e^{\frac{\log a}{\alpha}\,x}}\right)^\alpha$$
Poiché $\displaystyle\lim_{x\to+\infty}\frac{x}{e^{\frac{\log a}\alpha x}}=0$ per il passo 1 ($\beta=\frac{\log a}{\alpha}>0$), per algebra dei limiti (continuità di $t\mapsto t^\alpha$ per $\alpha>0$)
$$\lim_{x\to+\infty}\frac{x^\alpha}{a^x}=\left(\lim_{x\to+\infty}\frac{x}{e^{\frac{\log a}\alpha x}}\right)^\alpha=0^\alpha=0$$
Quindi $x^\alpha=o(a^x)$ per $x\to\infty$, $\forall\alpha>0$, $\forall a>1$.

## Passo 3: logaritmo contro potenza
$$\lim_{x\to+\infty}\frac{\log_ax}{x^\beta}=0\qquad\forall a>1,\ \forall\beta>0$$
$$\lim_{x\to+\infty}\frac{\log_ax}{x^\beta}\overset{H}{=}\lim_{x\to+\infty}\frac{\log_ae\cdot\frac1x}{\beta x^{\beta-1}}=\lim_{x\to+\infty}\frac{\log_ae}{\beta}\cdot\frac1{x^\beta}=0$$
(ultimo passaggio per algebra dei limiti).

## Passo 4: potenza del logaritmo contro potenza
$$\lim_{x\to+\infty}\frac{(\log_ax)^\alpha}{x^\gamma}=0\qquad\forall a>1,\ \forall\alpha,\gamma>0$$
$$\lim_{x\to+\infty}\frac{(\log_ax)^\alpha}{x^\gamma}=\lim_{x\to+\infty}\left(\frac{\log_ax}{x^{\gamma/\alpha}}\right)^\alpha=\left(\lim_{x\to+\infty}\frac{\log_ax}{x^{\gamma/\alpha}}\right)^\alpha=0^\alpha=0$$
dall'esempio precedente con $\beta=\frac\gamma\alpha>0$, grazie anche alla continuità di $t\mapsto t^\alpha$ per $\alpha>0$.

Quindi $(\log_ax)^\alpha=o(x^\gamma)$ per $x\to\infty$, $\forall\alpha,\gamma>0$, $\forall a>1$. $\square$

## Note collegate
- [[109_Gerarchia_degli_Infiniti_per_Funzioni]]
- [[36_Gerarchia_degli_Infiniti]] (versione per successioni)
- [[152_Teorema_di_de_l_Hopital]]
- [[154_Esempi_di_Applicazione_de_l_Hopital]]
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/gerarchia-infiniti-dimostrazione
