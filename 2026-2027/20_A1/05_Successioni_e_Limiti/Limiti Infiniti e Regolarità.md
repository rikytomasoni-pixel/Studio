---
created: 2026-09-30
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/successioni_e_limiti
aliases: []
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Limiti Infiniti e Regolarità

**Definizione (divergenza a $+\infty$).** $\displaystyle\lim_{n\to\infty}a_n=+\infty$ se $\forall M>0\ \exists N\in\mathbb{N}$ tale che $\forall n\ge N$: $a_n>M$.

![[divergenza-a-piu-infinito.png]]

**Definizione (divergenza a $-\infty$).** $\displaystyle\lim_{n\to\infty}a_n=-\infty$ se $\forall M>0\ \exists N\in\mathbb{N}$ tale che $\forall n\ge N$: $a_n<-M$.

![[divergenza-a-meno-infinito.png]]

**Esempio.** $a_n=\log\frac1n$: $\forall M>0$ si risolve $\log\frac1n<-M\iff\frac1n<e^{-M}\iff n>e^M$. Quindi $\lim\log\frac1n=-\infty$.

**Definizioni.**
- Se $\lim a_n=\ell\in\mathbb{R}$, $a_n$ **converge** a $\ell$.
- Se $\lim a_n=\pm\infty$, $a_n$ **diverge** a $\pm\infty$.
- In entrambi i casi $a_n$ è **regolare**.
- Se $a_n$ non converge né diverge ($\nexists\lim a_n$ in $\overline{\mathbb{R}}$), è **irregolare** (o **oscillante**, o **indeterminata**).
- $\overline{\mathbb{R}}=\mathbb{R}\cup\{+\infty\}\cup\{-\infty\}$ è l'insieme dei **reali estesi**.

**Esempi.**
- $a_n=(-1)^n$: irregolare **limitata**.
- $a_n=(-2)^n$: irregolare **illimitata**.
- $a_n=\begin{cases}2^n&n\text{ pari}\\1&n\text{ dispari}\end{cases}$: irregolare, illimitata dall'alto.

> **Teorema (unicità del limite in $\overline{\mathbb{R}}$).** Se esiste $\lim a_n=\ell\in\overline{\mathbb{R}}$, allora tale limite è unico. *(Senza dimostrazione.)*

**Definizione.** Se $\lim a_n=0$, $a_n$ è una successione **infinitesima**; se $\lim a_n=\pm\infty$, è una successione **infinita**.

### Convergenza per eccesso e per difetto
**Definizione.** $a_n$ converge a $\ell\in\mathbb{R}$ **per eccesso** (**per difetto**) se $\lim a_n=\ell$ e inoltre $a_n\ge\ell$ ($a_n\le\ell$) definitivamente. Si scrive
$$\lim_{n\to\infty}a_n=\ell^+\qquad(\lim a_n=\ell^-).$$

Formalmente:
- $\lim a_n=\ell^+$: $\forall\varepsilon>0\ \exists N:\ \forall n\ge N\ \ \ell\le a_n<\ell+\varepsilon$;
- $\lim a_n=\ell^-$: $\forall\varepsilon>0\ \exists N:\ \forall n\ge N\ \ \ell-\varepsilon<a_n\le\ell$.

![[convergenza-per-eccesso.png]]

**Esempi.**
- $\lim 2^{1/n}=1^+$
- $\lim\dfrac n{n+1}=1^-$
- $\lim\dfrac{(-1)^n}n=0$: né per eccesso né per difetto.

---
Precedente: [[Limite di una Successione]] · Successivo: [[Successioni Monotone]]
