---
tags:
  - AM1
  - successioni
  - confronti-asintotici
  - ordine-di-infinito
  - ordine-di-infinitesimo
data: 2026-10-07
fonte: Lezione 8
---

# Confronti e stime asintotiche: ordine di infinito

> [!warning] Definizione
> Siano $a_n,b_n$ successioni infinite, cioè
> $$\lim_{n\to\infty}a_n=\pm\infty,\qquad\lim_{n\to\infty}b_n=\pm\infty$$
> (non necessariamente dello stesso segno). Se
> $$\lim_{n\to\infty}\dfrac{a_n}{b_n}=\begin{cases}0 & a_n \text{ è infinito di ordine inferiore rispetto a } b_n\\[2pt] l\in\mathbb{R}\setminus\{0\} & a_n,b_n \text{ sono infiniti dello stesso ordine}\\[2pt] \pm\infty & b_n \text{ è infinito di ordine inferiore rispetto a } a_n\\[2pt] \nexists & a_n,b_n \text{ non confrontabili}\end{cases}$$

**Esempio.** $(\log_a n)^\beta$ è infinito di ordine inferiore rispetto a $n^\alpha,\ a^n,\ n!,\ n^n$, $\quad\forall\,a>1,\ \forall\,\alpha>0,\ \forall\,\beta>0$.

**Esempio.** $n!$ è infinito di ordine superiore rispetto a $n^\alpha,\ a^n,\ (\log_a n)^\beta$, $\quad\forall\,a>1,\ \forall\,\alpha>0,\ \forall\,\beta>0$.

**Esempio.** $\log n$, $\log n^2$ sono infiniti dello stesso ordine. Infatti
$$\dfrac{\log n}{\log n^2}=\dfrac{\log n}{2\log n}=\dfrac12\ \longrightarrow\ \dfrac12$$

**Esempio.** $(2+\sin n)\,n$ e $n$ sono **non confrontabili** (il rapporto $2+\sin n$ non ha limite).

> [!warning] Differenze rispetto alla trascrizione precedente
> - Nel secondo esempio ($n!$) la versione precedente scriveva "$\forall\,q>0$"; il PDF dice $\forall\,a>1$.
> - L'esempio "$n+\sin n$ e $n$" (stesso ordine, con $\lim\frac{n+\sin n}{n}=1$) **non è nel PDF**: è corretto, lo lascio qui come aggiunta, cancellabile. Nel PDF l'esempio di non confrontabilità è $(2+\sin n)n$ vs $n$.
> - Il rapporto per $\log n$, $\log n^2$ nel PDF è $\frac{\log n}{\log n^2}=\frac12$ (la versione precedente lo scriveva capovolto, $=2$, anch'esso corretto).

### Note collegate
- [[00_MOC_A1]]
- [[04_Gerarchia_degli_Infiniti]] — esempi di confronto tra infiniti
- [[04_o_piccolo_e_Asintotico]] — notazioni $o(\cdot)$ e $\sim$
- [[02_Limiti_di_Successioni]]
