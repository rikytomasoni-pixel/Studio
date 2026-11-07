---
tags:
  - AM1
  - serie
  - esempi
  - serie-irregolare
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 12-13)"
---

# Esempi elementari di serie

## Serie di termini nulli
$a_n=0\ \ \forall n\in\mathbb{N}$:
$$S_N=\sum_{n=0}^Na_n=0\ \ \forall N\in\mathbb{N}\ \Rightarrow\ \sum_{n=0}^\infty0=\lim_{N\to\infty}S_N=0\quad\text{converge}$$

## Serie di termini tutti uguali a 1
$a_n=1\ \ \forall n\in\mathbb{N}$:
$$S_N=\sum_{n=0}^Na_n=N+1\ \ \forall N\in\mathbb{N}\ \Rightarrow\ \sum_{n=0}^\infty1=\lim_{N\to\infty}S_N=+\infty\quad\text{diverge}$$

## Serie di termini alterni
$a_n=(-1)^n$:
$$S_N=\sum_{n=0}^Na_n=\sum_{n=0}^N(-1)^n=\begin{cases}1&N\text{ pari}\\0&N\text{ dispari}\end{cases}$$
$$\sum_{n=0}^\infty(-1)^n\ \text{ è indeterminata:}\quad\nexists\lim_{N\to\infty}S_N$$

## Note collegate
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[48_Studio_del_Carattere_di_una_Serie]]
- [[50_Serie_Geometrica]] (generalizza questi esempi)
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[00_MOC_Analisi_1]]

#AM1/serie/esempi-elementari
