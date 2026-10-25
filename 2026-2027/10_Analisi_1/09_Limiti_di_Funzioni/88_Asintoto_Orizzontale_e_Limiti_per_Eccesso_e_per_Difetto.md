---
tags:
  - AM1
  - limiti-di-funzioni
  - asintoto-orizzontale
  - limite-per-eccesso
  - definizione
data: 2026-10-23
fonte: "AM1 L13 26-27.pdf (pag. 11-13)"
---

# Asintoto orizzontale e limiti per eccesso e per difetto

## Asintoto orizzontale
> [!abstract] Definizione — asintoto orizzontale
> $f$ ha **asintoto orizzontale** $y=\ell$, $\ell\in\mathbb{R}$, per $x\to+\infty$ (rispettivamente $x\to-\infty$) se
> $$\lim_{x\to+\infty}f(x)=\ell\qquad\left(\text{rispettivamente }\lim_{x\to-\infty}f(x)=\ell\right)$$
> (limite finito all'infinito, [[87_Definizioni_Metriche_di_Limite_all_Infinito]]).

> [!example] Esempio
> $e^{-x}$ ha asintoto orizzontale $y=0$ a $+\infty$.

## Limiti per eccesso e per difetto
> [!abstract] Definizione — limite per eccesso / per difetto
> Se $\ell\in\mathbb{R}$, $x_0\in\overline{\mathbb{R}}$, si dice che
> $$\lim_{x\to x_0}f(x)=\ell^+\qquad(\ell^-)$$
> se $\displaystyle\lim_{x\to x_0}f(x)=\ell$ ed inoltre esiste $\mathcal{U}(x_0)$ intorno di $x_0$ tale che
> $$f(x)\geq\ell\quad(f(x)\leq\ell)\qquad\forall x\in\mathcal{U}(x_0)\cap I,\ x\neq x_0$$
> (si parla di limite **per eccesso** (o **per difetto**)).

> [!example] Esempi
> $$\lim_{x\to+\infty}e^{-x}=0^+\qquad\qquad\lim_{x\to-\infty}\frac1x=0^-$$

## Forma metrica per $x\to\pm\infty$
> [!note] Osservazione
> - $\displaystyle\lim_{x\to+\infty}f(x)=\ell^+$, $\ell\in\mathbb{R}$: $\ \forall\varepsilon>0\ \exists M>0$ tale che $\ x>M\ \Rightarrow\ \ell\leq f(x)<\ell+\varepsilon$.
> - $\displaystyle\lim_{x\to+\infty}f(x)=\ell^-$, $\ell\in\mathbb{R}$: $\ \forall\varepsilon>0\ \exists M>0$ tale che $\ x>M\ \Rightarrow\ \ell-\varepsilon<f(x)\leq\ell$.
> - Similmente per $\displaystyle\lim_{x\to-\infty}f(x)=\ell^+$ e $\displaystyle\lim_{x\to-\infty}f(x)=\ell^-$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** pag. 12 (per $\ell^+$) e pag. 13 (per $\ell^-$), in alto. **Cosa cercare:** grafico di una funzione che oscilla attorno a $y=\ell$ (rossa) con le linee $y=\ell\pm\varepsilon$ in azzurro; oltre la soglia $M$ (in verde sull'asse $x$) il grafico sta tutto sopra $\ell$ (per $\ell^+$) o tutto sotto $\ell$ (per $\ell^-$).

## Note collegate
- [[87_Definizioni_Metriche_di_Limite_all_Infinito]]
- [[86_Definizione_Topologica_di_Limite]]
- [[89_Asintoto_Obliquo]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/asintoto-orizzontale
