---
created: 2026-09-25
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
origine: UpdateVault
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Monotonia

> [!info] Definizione — Funzione monotona
> $f:A\subseteq\mathbb{R}\to\mathbb{R}$ si dice monotona:
> - **crescente** se $\forall\, x_1,x_2\in A$: $\ x_1<x_2 \ \Rightarrow\ f(x_1)\leq f(x_2)$
> - **strettamente crescente** se $\forall\, x_1,x_2\in A$: $\ x_1<x_2 \ \Rightarrow\ f(x_1)<f(x_2)$
> - **decrescente** se $\forall\, x_1,x_2\in A$: $\ x_1<x_2 \ \Rightarrow\ f(x_1)\geq f(x_2)$
> - **strettamente decrescente** se $\forall\, x_1,x_2\in A$: $\ x_1<x_2 \ \Rightarrow\ f(x_1)>f(x_2)$
>
> $f$ si dice monotona se soddisfa una di queste 4 proprietà.

**Esempi** (grafici con un salto):

![[esempi-monotonia-quattro-grafici.png]]

**Esempio.** $f(x)=\dfrac{1}{x}$, $x\in(-\infty,0)\cup(0,\infty)$

![[grafico-iperbole-1-su-x.png]]

$f$ **non** è monotona in $(-\infty,0)\cup(0,\infty)$; $f$ è **strettamente decrescente** in $(-\infty,0)$ e in $(0,\infty)$.

## Caratterizzazione tramite rapporto incrementale

**Osservazione.** $f$ crescente preserva le disuguaglianze; $f$ decrescente le inverte.

$$f \text{ crescente} \quad\Longleftrightarrow\quad \dfrac{f(x_2)-f(x_1)}{x_2-x_1}\geq 0 \qquad \forall\, x_1,x_2\in\mathcal{D}(f),\ x_1\neq x_2$$

Questo rapporto è il coefficiente angolare della retta secante per $(x_1,f(x_1))$ e $(x_2,f(x_2))$:
$$m = \dfrac{f(x_2)-f(x_1)}{x_2-x_1} \geq 0$$

$$f \text{ decrescente} \quad\Longleftrightarrow\quad \dfrac{f(x_2)-f(x_1)}{x_2-x_1}\leq 0 \qquad \forall\, x_1,x_2\in\mathcal{D}(f),\ x_2\neq x_1$$
![[retta-secante-funzione-crescente.png]]
*(simile a quanto visto sopra; strettamente toglie l'uguale...)*

---
Precedente: [[Funzioni Pari e Dispari]] · Successivo: [[Funzioni Periodiche]]
