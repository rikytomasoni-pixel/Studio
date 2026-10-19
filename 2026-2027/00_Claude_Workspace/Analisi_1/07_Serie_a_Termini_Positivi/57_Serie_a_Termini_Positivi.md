---
tags:
  - AM1
  - serie
  - serie-a-termini-positivi
  - teorema
  - dimostrazione
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 4-5)"
stato: da_verificare
destinazione: 10_Analisi_1/07_Serie_a_Termini_Positivi (cartella nuova)
---

# Serie a termini (definitivamente) positivi

> [!info] Definizione
> Una serie $\displaystyle\sum_{n=1}^\infty a_n$ si dice **a termini (definitivamente) positivi** se $a_n\geq0$ per ogni $n\in\mathbb{N}$ (definitivamente).

> [!abstract] Teorema
> Se la serie $\displaystyle\sum_{n=1}^\infty a_n$ è a termini (definitivamente) positivi, allora essa **converge** oppure **diverge a $+\infty$** (non può essere indeterminata).

## Dimostrazione
Per ipotesi esiste $n_0\in\mathbb{N}$ tale che $a_n\geq0$ per ogni $n\geq n_0$. Allora per ogni $N\geq n_0$
$$S_N=\sum_{n=1}^N a_n=\sum_{n=1}^{N-1}a_n+\underbrace{a_N}_{\geq0}\geq\sum_{n=1}^{N-1}a_n=S_{N-1}$$
$\Rightarrow S_N$ è **definitivamente crescente** in $N\in\mathbb{N}$.

Quindi, per il teorema di esistenza del limite per successioni (definitivamente) monotone ([[31_Successioni_Monotone]]),
$$\exists\,S=\lim_{N\to\infty}S_N\in\mathbb{R}\cup\{+\infty\}$$
cioè
$$\sum_{n=1}^\infty a_n=\lim_{N\to\infty}S_N=S\in\mathbb{R}\cup\{+\infty\}$$
La serie converge se $S\in\mathbb{R}$, diverge se $S=+\infty$. $\square$

## Note collegate
- [[58_Criterio_del_Confronto_per_Serie]] (si usa questo teorema)
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[48_Studio_del_Carattere_di_una_Serie]]
- [[31_Successioni_Monotone]]
- [[00_MOC_Analisi_1]]

#AM1/serie/termini-positivi
