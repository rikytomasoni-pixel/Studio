---
tags:
  - AM1
  - successioni
  - monotonia
  - derivate
  - leibniz
  - esempio
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 9-12)"
---

# Monotonia di una successione tramite una funzione derivabile

> [!note] Osservazione — monotonia delle successioni
> Per dimostrare che una successione $a_n$ sia monotona, bisogna mostrare che per ogni $n\in\mathbb{N}$
> - $a_n\le a_{n+1}$ (crescente)
> - $a_n\ge a_{n+1}$ (decrescente)
>
> Tuttavia, se si riesce a definire una funzione $f:[0,\infty)\to\mathbb{R}$ monotona crescente/decrescente tale che $f(n)=a_n$ per ogni $n\in\mathbb{N}$ ($f$ **interpola** i valori della successione $a_n$), allora si può dedurre che la successione $a_n$ ha la stessa monotonia della funzione $f$.

Infatti, se $f$ cresce/decresce, essendo $n<n+1$,
$$a_n=f(n)\le f(n+1)=a_{n+1}\quad(\text{crescente})\qquad a_n=f(n)\ge f(n+1)=a_{n+1}\quad(\text{decrescente})$$

Per dimostrare che $f$ sia crescente/decrescente è sufficiente che $f$ sia derivabile e $f'(x)\ge0\ /\ f'(x)\le0$ per ogni $x\in[0,\infty)$, grazie al [[140_Test_di_Monotonia|test di monotonia]].

![[corrispondenzaFunzioneSuccessione.png]]

> [!warning] Condizione solo sufficiente
> Questa è una condizione **sufficiente**: può accadere che $a_n$ sia monotona e che una funzione $f$ che ne interpola i valori non lo sia.

![[esempioPag10L19.png]]

## Esempio: $a_n=\dfrac{\log n}{n}$, $n\ge1$

Sia $f:(0,\infty)\to\mathbb{R}$, $f(x)=\dfrac{\log x}{x}$. Allora
$$f'(x)=\frac{1-\log x}{x^2}\qquad\forall x>0$$
$$f'(x)\ge0\iff1-\log x\ge0\iff0<x\le e$$
Quindi $f$ **cresce** in $(0,e]$ e **decresce** in $[e,\infty)$.
![[MassimoLogxsuX.png]]

![[LogXsuX.png]]

$a_n$ è decrescente per $n\ge3$ (forse anche per $n\ge2$, forse no…) $\Rightarrow$ $a_n$ è **definitivamente decrescente**.

> [!note] Osservazione (non presente negli appunti)
> Il dubbio del quaderno si risolve a mano: $a_2=\frac{\log2}{2}\approx0{,}347<a_3=\frac{\log3}{3}\approx0{,}366$, quindi $a_n$ **non** è decrescente da $n\ge2$; lo è da $n\ge3$ (il massimo di $f$ è in $x=e\approx2{,}718$, tra $2$ e $3$).

## Applicazione: serie $\sum_{n=1}^\infty(-1)^n\dfrac{\log n}{n}$

- $\displaystyle\sum_{n=1}^\infty\frac{\log n}{n}=+\infty$ per confronto con $\displaystyle\sum_{n=1}^\infty\frac1n$ (serie armonica): quindi la serie **non converge assolutamente**.
- La serie **converge per Leibniz** ([[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]) perché $a_n=\dfrac{\log n}{n}\ge0$ per ogni $n\ge1$, $\displaystyle\lim_{n\to\infty}a_n=0$ per la [[36_Gerarchia_degli_Infiniti|gerarchia degli infiniti]] e $a_n$ è definitivamente decrescente per quanto visto sopra.

Lo stesso esempio è già trattato in [[79_Esempio_Serie_Alternata_log_n_su_n]] (L12).

> [!tip] Tecnica
> Da utilizzare per lo studio della monotonia di $a_n$ quando si vuole usare il criterio di Leibniz per studiare il carattere di
> $$\sum_{n=0}^\infty(-1)^na_n\qquad\text{con }a_n\ge0,\ \lim_{n\to\infty}a_n=0$$

## Note collegate
- [[31_Successioni_Monotone]]
- [[140_Test_di_Monotonia]]
- [[79_Esempio_Serie_Alternata_log_n_su_n]]
- [[76_Serie_a_Segno_Alterno_e_Criterio_di_Leibniz]]
- [[78_Osservazioni_sul_Criterio_di_Leibniz]]
- [[36_Gerarchia_degli_Infiniti]]
- [[00_MOC_Analisi_1]]

#AM1/successioni/monotonia-tramite-derivate
