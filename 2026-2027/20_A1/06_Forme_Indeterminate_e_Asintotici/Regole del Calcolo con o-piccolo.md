---
created: 2026-10-09
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Regole del Calcolo con o-piccolo

## Ulteriori proprietà di o-piccolo

> [!abstract] Teorema (Proprietà)
> $$o(a_n)\cdot o(b_n) = o(a_n b_n)$$
> $$o\big(o(a_n)\big) = o(a_n)$$
> $$o\!\left(\dfrac1n\right)+o\!\left(\dfrac{1}{n^2}\right) = o\!\left(\dfrac1n\right)$$
> $$o(n)+o(n^2) = o(n^2)$$

**dim (prima proprietà):** $\dfrac{o(a_n)}{a_n}\to 0$, $\dfrac{o(b_n)}{b_n}\to 0$ per definizione, quindi $\dfrac{o(a_n)\cdot o(b_n)}{a_n\cdot b_n} = \dfrac{o(a_n)}{a_n}\cdot\dfrac{o(b_n)}{b_n}\to 0\cdot 0 = 0$.

**dim (seconda proprietà):** $o(a_n)\to 0\cdot a_n$; applicando di nuovo la definizione di $o$-piccolo a una successione che è già $o(a_n)$ si ottiene ancora $o(a_n)$.

> [!note] Osservazione
> $$a_n-b_n = o(a_n) \quad\Longleftrightarrow\quad a_n\sim b_n$$

<DUBBIO posizione="ultima pagina, dopo le proprietà di o-piccolo">La riga finale ("ad esempio o(√n)=o(n)" o simile) e l'ultimo esempio numerico della lezione, con una forma indeterminata del tipo $\left[\dfrac{0}{0}\right]$ coinvolgente $\varepsilon_n\sim 2n$ e $\sin\varepsilon_n$, sono troppo illeggibili per essere trascritti con sicurezza: mancano dati sufficienti per ricostruire la successione $a_n$ e il valore del limite richiesto ("$\lim_{n\to\infty} a_n = ?$").</DUBBIO>

---
Precedente: [[Esempi di Limiti con gli Asintotici]]
