---
tags:
  - AM1
  - limiti-di-funzioni
  - gerarchia-degli-infiniti
  - teorema
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 15-18)"
---

# Gerarchia degli infiniti (per funzioni)

> [!abstract] Teorema (gerarchia degli infiniti)
> Siano $a>1$, $\alpha,\beta>0$. Allora
> $$\lim_{x\to+\infty}\frac{(\log_ax)^\alpha}{x^\beta}=0\qquad\text{cioè}\qquad(\log_ax)^\alpha=o(x^\beta)\ \ \text{per }x\to+\infty$$
> $$\lim_{x\to+\infty}\frac{x^\beta}{a^x}=0\qquad\text{cioè}\qquad x^\beta=o(a^x)\ \ \text{per }x\to+\infty$$

*(dimostrazione con il teorema di de l'Hôpital)*

> [!note] Osservazione — composizione con una funzione infinita
> Da quanto scritto sopra e dal [[104_Cambio_di_Variabile_nei_Limiti|teorema sul cambio di variabile nei limiti]] segue che se $f(x)$ è una funzione tale che $\displaystyle\lim_{x\to x_0}f(x)=+\infty$, $x_0\in\overline{\mathbb{R}}$, allora
> $$\lim_{x\to x_0}\frac{(\log_af(x))^\alpha}{(f(x))^\beta}\overset{t=f(x)}{=}\lim_{t\to+\infty}\frac{(\log_at)^\alpha}{t^\beta}=0\qquad\lim_{x\to x_0}\frac{(f(x))^\beta}{a^{f(x)}}\overset{t=f(x)}{=}\lim_{t\to+\infty}\frac{t^\beta}{a^t}=0$$
> Similmente, se $x_n$ è una successione divergente a $+\infty$:
> $$\lim_{n\to\infty}\frac{(\log_ax_n)^\alpha}{(x_n)^\beta}=0\qquad\lim_{n\to\infty}\frac{(x_n)^\beta}{a^{x_n}}=0$$
> (per $x_n=n$ ritroviamo la gerarchia degli infiniti vista per le successioni: [[36_Gerarchia_degli_Infiniti]]).

> [!example] Esempio
> $$\lim_{t\to0^+}t^\beta\,|\log_at|^\alpha=0\qquad\forall a>1,\ \forall\alpha,\beta>0\qquad[0\cdot\infty]$$
> Per cambio di variabile e gerarchia degli infiniti, infatti, posto $x=\frac1t$ (con $\displaystyle\lim_{t\to0^+}\frac1t=+\infty$, $\,x=x(t)$):
> $$\lim_{t\to0^+}t^\beta|\log_at|^\alpha=\lim_{x\to+\infty}\frac1{x^\beta}\Big|\log_a\frac1x\Big|^\alpha=\lim_{x\to+\infty}\frac{(\log_ax)^\alpha}{x^\beta}=0$$

## Note collegate
- [[36_Gerarchia_degli_Infiniti]] (versione per successioni)
- [[104_Cambio_di_Variabile_nei_Limiti]]
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/gerarchia-infiniti
