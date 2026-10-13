---
tags:
  - AM1
  - funzioni
  - monotonia
  - rapporto-incrementale
data: 2026-09-25
fonte: Lezione 5
---

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

![[monotoniaGrafici.png]]

Nell'ordine (come nel PDF): il primo grafico è **crescente (non strettamente)**, il secondo **strettamente crescente**, il terzo **decrescente (non strettamente)**, il quarto **strettamente decrescente**.

**Esempio.** $f(x)=\dfrac{1}{x}$, $x\in(-\infty,0)\cup(0,\infty)$

![[grafico 1suX.png]]

$f$ **non** è monotona in $(-\infty,0)\cup(0,\infty)$; $f$ è **strettamente decrescente** in $(-\infty,0)$ e in $(0,\infty)$.

## Caratterizzazione tramite rapporto incrementale

**Osservazione.** $f$ crescente preserva le disuguaglianze; $f$ decrescente le inverte.

$$f \text{ crescente} \quad\Longleftrightarrow\quad \dfrac{f(x_2)-f(x_1)}{x_2-x_1}\geq 0 \qquad \forall\, x_1,x_2\in\mathcal{D}(f),\ x_1\neq x_2$$

Questo rapporto è il coefficiente angolare della retta secante per $(x_1,f(x_1))$ e $(x_2,f(x_2))$:
$$m = \dfrac{f(x_2)-f(x_1)}{x_2-x_1} \geq 0$$

$$f \text{ decrescente} \quad\Longleftrightarrow\quad \dfrac{f(x_2)-f(x_1)}{x_2-x_1}\leq 0 \qquad \forall\, x_1,x_2\in\mathcal{D}(f),\ x_2\neq x_1$$
![[RapportoIncrementale.png]]
*(simile a quanto visto sopra; strettamente toglie l'uguale...)*

### Note collegate
- [[00_MOC_A1]]
- [[07_Teorema_Monotone_Invertibili]] — le funzioni strettamente monotone sono invertibili
- [[06_Iniettivita_Suriettivita_Inversa]]
- [[02_Funzioni_Generalità]]
- [[05_Radici_e_Potenze]] — $t\mapsto t^n$ strettamente crescente
- [[00_Logaritmi]] — $a^x$ strettamente monotona