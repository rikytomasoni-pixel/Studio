---
created: 2026-10-07
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Potenze con Base ed Esponente Variabili

## Esponenziali con base ed esponente variabili

**Osservazione.** $a_n = e^{b_n\log a_n}$

Se $\lim_{n\to\infty} a_n = a>0$ e $\lim_{n\to\infty} b_n = b\in\mathbb{R}$, allora
$$\lim_{n\to\infty} b_n\log a_n = b\log a \quad \text{(per algebra dei limiti; vedi [[Algebra dei Limiti]])}$$
$$\lim_{n\to\infty} a_n^{\,b_n} = \lim_{n\to\infty} e^{b_n\log a_n} = e^{b\log a} = a^b$$

## Teorema generale sulle potenze $a_n^{b_n}$

> [!abstract] Teorema
> Se $a_n, b_n$ sono successioni tali che $\lim_{n\to\infty} a_n = a\geq 0$ ($a_n>0$ definitivamente) e $\lim_{n\to\infty} b_n = b$. Allora
> $$\lim_{n\to\infty} a_n^{\,b_n} = a^b$$
> (salvo forme di indeterminazione), dove
> $$a^{+\infty} = +\infty \quad \forall\, a>1 \ \text{(anche } a=+\infty\text{)}$$
> $$a^{-\infty} = 0 \quad \forall\, a>1 \ \text{(anche } a=+\infty\text{)}$$
> $$a^{+\infty} = 0 \quad \forall\, a\in[0,1)$$
> $$a^{-\infty} = +\infty \quad \forall\, a\in[0,1)$$
> $$(+\infty)^b = +\infty \quad \forall\, b>0 \ \text{(anche } b=+\infty\text{)}$$
> $$(+\infty)^b = 0 \quad \forall\, b<0 \ \text{(anche } b=-\infty\text{)}$$

**Osservazione.** $0^0$, $\infty^0$, $1^\infty$ sono esclusi: sono forme di indeterminazione.

**Osservazione.** Non sono forme di indeterminazione:
$$b_n = \dfrac{1}{n}, \quad a_n=1 \ \Rightarrow\ a_n^{\,b_n} = 1^{1/n} = 1 \to 1$$
$$a_n = n, \quad b_n = 0 \ \Rightarrow\ a_n\cdot b_n = n\cdot 0 = 0 \to 0$$

## Applicazione alla gerarchia degli infiniti

**Osservazione.** $\displaystyle\lim_{n\to\infty} n^{1/n} = 1$ $\quad [\infty^0]$

$$n^{1/n} = e^{\frac{1}{n}\log n}, \qquad \dfrac{\log n}{n} \to 0 \quad \text{per gerarchia degli infiniti}$$
$$\Rightarrow \quad \lim_{n\to\infty} n^{1/n} = \lim_{n\to\infty} e^{\frac{\log n}{n}} = e^0 = 1$$

---
Precedente: [[Tecniche per le Forme Infinito meno Infinito]] · Successivo: [[Numero di Nepero]]
