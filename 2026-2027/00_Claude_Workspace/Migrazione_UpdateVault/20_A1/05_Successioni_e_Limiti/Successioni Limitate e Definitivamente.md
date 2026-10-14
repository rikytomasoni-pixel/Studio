---
created: 2026-09-30
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/successioni_e_limiti
aliases: []
origine: UpdateVault
---
[[00_A1_Successioni_e_Limiti|⬅️ Torna a Successioni e Limiti]]

# Successioni Limitate e Definitivamente

> [!warning] Def. Successione
> Una **successione** (di numeri reali) è una funzione
> $$f: A\subseteq\mathbb{N}\subseteq\mathbb{R}\to\mathbb{R}$$
> con $A=\{n\in\mathbb{N}: n\geq n_0\}$ per qualche $n_0\in\mathbb{N}$.

**Esempi.**
$$f(n) = \dfrac{1}{n}, \quad n\geq 1$$
$$g(n) = \log(n-7), \quad n\geq 8$$

> [!note] Nota di trascrizione
> Nella pagina originale erano presenti altri due esempi, risultati illeggibili nella scansione fornita.

**Osservazione.** A livello di notazione scriveremo $a_n, b_n,\dots$ invece di $f(n), g(n), h(n)\dots$

**Osservazione.** Il grafico di una successione è una sequenza di punti
$$\mathcal{G}(a_n) = \{(n,a_n)\in\mathbb{R}^2 : n\in\mathcal{D}(a_n),\ n\in\mathbb{N}\}$$

![[grafico-successione-punti.png]]
**Esempio.** $a_n = \dfrac{1}{n}$


![[grafico-successione-2-su-n-piu-1.png]]
## Limitatezza

> [!warning] Definizione
> Una successione si dice:
> - **limitata dall'alto** (superiormente) se $\exists\, M\in\mathbb{R}$ tale che
> $$a_n \leq M \qquad \forall\, n\in\mathbb{N}$$
> - **limitata dal basso** (inferiormente) se $\exists\, m\in\mathbb{R}$ tale che
> $$a_n \geq m \qquad \forall\, n\in\mathbb{N}$$
> - **limitata** se è limitata sia dall'alto che dal basso, cioè se $\exists\, m,M\in\mathbb{R}$ tali che
> $$m\leq a_n\leq M \qquad \forall\, n\in\mathbb{N}$$

**Osservazione.** Equivalentemente, $a_n$ è limitata se $\exists\, k>0$ tale che
$$|a_n|\leq k \qquad \forall\, n\in\mathbb{N}$$

## Proprietà definitivamente vere

> [!warning] Definizione — Definitivamente
> Diremo che una successione $a_n$ soddisfa una certa proprietà $P$ **definitivamente** (in $n\in\mathbb{N}$) se
> $$\exists\, N\in\mathbb{N} \text{ tale che } P \text{ è soddisfatta da } a_n \ \ \forall\, n\geq N$$

**Esempio.** $a_n = \dfrac{1}{n}$ è definitivamente minore di $\dfrac{1}{10}$.

Infatti $a_n < \dfrac{1}{10}$ se e solo se $\dfrac{1}{n} < \dfrac{1}{10}$ se e solo se $n>10$, cioè se $n\geq N=11$.

---
Precedente: [[Successioni di Numeri Reali]] · Successivo: [[Limite di una Successione]]
