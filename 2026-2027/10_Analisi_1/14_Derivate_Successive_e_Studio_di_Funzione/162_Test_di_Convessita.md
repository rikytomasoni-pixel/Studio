---
tags:
  - AM1
  - derivate-successive
  - convessita
  - derivata-seconda
  - teorema
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 9-10)"
---

# Test di convessità

> [!abstract] Teorema (test di convessità)
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo.
> 1. Se $f$ è **derivabile** in $I$, allora $f$ è convessa (concava) in $I$ se e solo se $f'$ è **monotona crescente** (decrescente) in $I$.
> 2. Se $f$ è **derivabile 2 volte** in $I$, allora $f$ è convessa (concava) in $I$ se e solo se
> $$f''(x)\ge0\quad\forall x\in I\qquad\big(f''(x)\le0\quad\forall x\in I\big)$$

> [!note] Osservazione
> (2) segue immediatamente da (1) e dal [[140_Test_di_Monotonia|test di monotonia]] applicato a $f'$.

## Esempio: $f(x)=\log_a x$, $a>0$, $a\ne1$, $x>0$

$$f'(x)=\frac{1}{x\log a}\quad(x>0)\qquad f''(x)=-\frac{1}{x^2\log a}\quad(x>0)$$

- Se $a>1$ allora $\log a>0$, quindi $f'(x)>0$ e $f''(x)<0$ per ogni $x\in(0,\infty)$ $\Rightarrow$ $\log_a x$ è **crescente e concava**.
- Se $0<a<1$ allora $\log a<0$, quindi $f'(x)<0$ e $f''(x)>0$ per ogni $x\in(0,\infty)$ $\Rightarrow$ $\log_a x$ è **decrescente e convessa**.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Pag. 10:** due grafici di $\log_a x$ nello stesso piano, entrambi passanti per il punto $(1,0)$: in rosso il caso $a>1$ (crescente, concavo), in blu il caso $0<a<1$ (decrescente, convesso, con asintoto verticale sull'asse $y$).

## Note collegate
- [[161_Convessita_e_Rette_Tangenti]]
- [[163_Punti_di_Flesso]]
- [[165_Flessi_e_Derivata_Seconda]]
- [[140_Test_di_Monotonia]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[157_Studio_del_Grafico_di_una_Funzione]]
- [[12_Logaritmi]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/convessita
