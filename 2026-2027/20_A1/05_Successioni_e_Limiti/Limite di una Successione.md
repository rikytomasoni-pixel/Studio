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

# Limite di una Successione

**Definizione (convergenza).** Una successione $a_n$ **converge** a $\ell\in\mathbb{R}$ e si scrive $\displaystyle\lim_{n\to\infty}a_n=\ell$ se
$$\forall\varepsilon>0\ \ \exists N\in\mathbb{N}\ \text{ tale che }\ \forall n\ge N:\quad|a_n-\ell|<\varepsilon\quad(\iff\ell-\varepsilon<a_n<\ell+\varepsilon).$$

![[definizione-limite-successione-striscia-epsilon.png]]

**Osservazione.**
$$\lim_{n\to\infty}a_n=\ell\iff\lim_{n\to\infty}|a_n-\ell|=0\iff\lim_{n\to\infty}(a_n-\ell)=0.$$

Non tutte le successioni ammettono limite in $\mathbb{R}$: $\lim n$ e $\lim(-1)^n$ **non esistono in $\mathbb{R}$**.

### Unicità del limite

> **Teorema (unicità del limite).** Data una successione $a_n$, se esiste $\displaystyle\lim_{n\to\infty}a_n=\ell\in\mathbb{R}$, allora esso è **unico**.

**Dimostrazione (per assurdo).** Supponiamo esistano $\ell_1\neq\ell_2$ in $\mathbb{R}$ tali che $\lim a_n=\ell_1$ e $\lim a_n=\ell_2$; per comodità $\ell_1>\ell_2$.

![[unicita-limite-intorni-disgiunti.png]]

Si sceglie
$$\varepsilon=\frac13|\ell_1-\ell_2|=\frac{\ell_1-\ell_2}3>0.$$
Allora $\ell_1-\varepsilon>\ell_2+\varepsilon$: infatti ciò equivale a $\ell_1-\ell_2>2\varepsilon=2\,\frac{\ell_1-\ell_2}3$, cioè $\frac13(\ell_1-\ell_2)>0$, vero. Quindi
$$(\ell_1-\varepsilon,\ell_1+\varepsilon)\cap(\ell_2-\varepsilon,\ell_2+\varepsilon)=\varnothing.$$
Per definizione di limite esistono $N_1,N_2$ tali che $a_n\in(\ell_1-\varepsilon,\ell_1+\varepsilon)$ per $n\ge N_1$ e $a_n\in(\ell_2-\varepsilon,\ell_2+\varepsilon)$ per $n\ge N_2$. Allora per ogni $n\ge N=\max\{N_1,N_2\}$ dovrebbe essere $a_n$ nell'intersezione, che è vuota. **Assurdo.** $\square$

### Esempio: $\lim\frac1n=0$
Fissato $\varepsilon>0$ si risolve $|a_n-0|<\varepsilon$, cioè $-\varepsilon<\frac1n<\varepsilon$. La disuguaglianza $\frac1n>-\varepsilon$ vale $\forall n\in\mathbb{N}$ (poiché $\frac1n>0>-\varepsilon$), mentre $\frac1n<\varepsilon\iff n>\frac1\varepsilon$. Quindi $\lim_{n\to\infty}\frac1n=0$ per definizione.

---
Precedente: [[Successioni Limitate e Definitivamente]] · Successivo: [[Limiti Infiniti e Regolarità]]
