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

# Successioni Limitate e Definitivamente

**Definizione.** Una **successione** (di numeri reali) è una funzione
$$f:\{n\in\mathbb{N}:n\ge n_0\}\subseteq\mathbb{N}\ (\subseteq\mathbb{R})\to\mathbb{R}\quad\text{per qualche } n_0\in\mathbb{N}.$$

Esempi: $f(n)=\frac1n$ ($n\ge1$); $g(n)=\log(n-7)$ ($n\ge8$); $h(n)=n^2$ ($n\ge0$); $v(n)=\frac1{n^2-49}$ ($n\ge8$).

A livello di notazione si scrive $a_n,b_n,c_n,\dots$ invece di $f(n),g(n),h(n),\dots$.

**Grafico.** Il grafico di una successione è una **sequenza di punti** $(n,a_n)\in\mathbb{R}^2$:
$$\mathcal{G}(\{a_n\})=\{(n,a_n)\in\mathbb{R}^2:\ n\ge n_0,\ n\in\mathbb{N}\}.$$

![[grafico-successione-punti.png]]

**Esempio.** $a_n=\dfrac2{n+1}$: i valori $2,\,1,\,\tfrac23,\dots$ si avvicinano a $0$.

![[grafico-successione-2-su-n-piu-1.png]]

### Successioni limitate
Una successione si dice:
- **limitata dall'alto** se $\exists M\in\mathbb{R}$: $a_n\le M\ \ \forall n\in\mathbb{N}$;
- **limitata dal basso** se $\exists m\in\mathbb{R}$: $a_n\ge m\ \ \forall n\in\mathbb{N}$;
- **limitata** se lo è da entrambe: $m\le a_n\le M\ \forall n$. Equivalentemente, $\exists K>0$ tale che $|a_n|\le K\ \forall n\in\mathbb{N}$.

### «Definitivamente»
**Definizione.** Una successione soddisfa una proprietà $P$ **definitivamente** (in $n\in\mathbb{N}$) se $\exists N\in\mathbb{N}$ tale che $P$ è soddisfatta da $a_n$ per ogni $n\ge N$.

**Esempio.** $a_n=\frac1n$ è definitivamente minore di $\frac1\pi$: infatti $\frac1n<\frac1\pi\iff n>\pi\iff n\ge N=4$.

---
Precedente: [[Successioni di Numeri Reali]] · Successivo: [[Limite di una Successione]]
