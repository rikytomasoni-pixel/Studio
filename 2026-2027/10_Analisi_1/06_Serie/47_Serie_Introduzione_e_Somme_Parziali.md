---
tags:
  - AM1
  - serie
  - somme-parziali
  - definizione
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 7-9)"
stato: da_verificare
immagini_mancanti: true
---

# Serie di numeri reali: introduzione e somme parziali

## Motivazioni (esempi introduttivi)
- Un rettangolo di lati $1$ e $2$ suddiviso in rettangoli di area $1,\ \frac12,\ \frac14,\ \frac18,\ \frac1{16},\dots$:
$$2=1+\frac12+\frac14+\frac18+\frac1{16}+\dots+\frac1{2^n}+\dots$$

![[IntroduzioneSerie.png|236]]

- $0,\overline9=1$ in base $10$; $\ 0,\overline7=1$ in base $8$ (vedi [[51_Rappresentazione_Decimale_e_Serie]]).
- $r\in\mathbb{R}\Rightarrow r=\pm a_0,a_1a_2a_3\dots$ con $a_0\in\mathbb{N}$, $a_k\in\{0,1,2,\dots,9\}$ $\forall k\geq1$.
- Achille e la tartaruga (paradosso).

## Successione delle somme parziali

> [!abstract] Definizione
> Data una successione di numeri reali $a_n$, definiamo **successione delle somme parziali** di $a_n$
> $$S_N=\sum_{n=0}^{N}a_n=a_0+a_1+a_2+\dots+a_N\qquad\forall N\in\mathbb{N}$$

## Serie

> [!abstract] Definizione
> Chiamiamo **serie degli $a_n$** la scrittura formale
> $$\sum_{n=0}^{\infty}a_n$$
> che si legge "serie degli $a_n$". Indica formalmente la somma degli infiniti termini $a_n$.

- Diremo che la serie degli $a_n$ **converge** a $S\in\mathbb{R}$ se
$$\exists\lim_{N\to\infty}S_N=S\in\mathbb{R}\qquad\text{dove }S_N=\sum_{n=0}^Na_n$$
Scriveremo in tal caso
$$\sum_{n=0}^{\infty}a_n=S=\left(\lim_{N\to\infty}S_N\right)\in\mathbb{R}$$
$S$ si chiama **somma della serie** degli $a_n$.

- Diremo che la serie degli $a_n$ **diverge a $\pm\infty$** se
$$\exists\lim_{N\to\infty}S_N=\pm\infty$$
In tal caso scriveremo
$$\sum_{n=0}^{\infty}a_n=\pm\infty\ \left(=\lim_{N\to\infty}S_N\right)$$
e diremo che $\pm\infty$ è la somma della serie degli $a_n$.

In entrambi i casi diremo che la serie degli $a_n$ è **regolare** (serie convergente o divergente).

- Se $\nexists\lim_{N\to\infty}S_N$ in $\overline{\mathbb{R}}$ diremo che la serie degli $a_n$ è **irregolare** o **indeterminata**.

> [!note] Osservazione
> La somma della serie è
> $$S=\sum_{n=0}^{\infty}a_n=\lim_{N\to\infty}S_N=\lim_{N\to\infty}\sum_{n=0}^Na_n\in\overline{\mathbb{R}}\qquad\text{se esiste}$$

## Note collegate
- [[48_Studio_del_Carattere_di_una_Serie]]
- [[49_Esempi_Elementari_di_Serie]]
- [[50_Serie_Geometrica]]
- [[51_Rappresentazione_Decimale_e_Serie]]
- [[30_Limiti_di_Successioni]]
- [[29_Successioni_Definizioni_Base]]
- [[00_MOC_Analisi_1]]

#AM1/serie/introduzione-somme-parziali
