---
tags:
  - AM1
  - successioni
  - definizioni
  - limitatezza
data: 2026-09-30
fonte: Lezione 6
---

# Successioni di numeri reali — definizioni di base

> [!warning] Def. Successione
> Una **successione** (di numeri reali) è una funzione
> $$f: A\subseteq\mathbb{N}\subseteq\mathbb{R}\to\mathbb{R}$$
> con $A=\{n\in\mathbb{N}: n\geq n_0\}$ per qualche $n_0\in\mathbb{N}$.

**Esempi.**
$$f(n) = \dfrac{1}{n}, \quad n\geq 1$$
$$g(n) = \log(n-7), \quad n\geq 8$$
$$h(n) = n^2, \quad n\geq 0$$
$$v(n) = \dfrac{1}{n^2-49}, \quad n\geq 8$$

**Osservazione.** A livello di notazione scriveremo $a_n, b_n,\dots$ invece di $f(n), g(n), h(n)\dots$

**Osservazione.** Il grafico di una successione è una sequenza di punti
$$\mathcal{G}(a_n) = \{(n,a_n)\in\mathbb{R}^2 : n\in\mathcal{D}(a_n),\ n\in\mathbb{N}\}$$

![[SuccessionePuntiIsolati.png]]
**Esempio.** $a_n = \dfrac{2}{n+1}$ (i primi valori sono $2,\ 1,\ \tfrac23,\dots$)


![[Successione1suN.png]]
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

**Esempio.** $a_n = \dfrac{1}{n}$ è definitivamente minore di $\dfrac{1}{\pi}$.

Infatti $\dfrac{1}{n} < \dfrac{1}{\pi}$ se e solo se $n>\pi$, cioè se e solo se $n\geq N=4$.

### Note collegate
- [[00_MOC_A1]]
- [[02_Funzioni_Generalità]] — definizione generale di successione e primi esempi
- [[02_Limiti_di_Successioni]] — convergenza e divergenza
- [[03_Successioni_Monotone]]
- [[01_Insiemi_Limitati_Max_Min]] — limitatezza di un insieme