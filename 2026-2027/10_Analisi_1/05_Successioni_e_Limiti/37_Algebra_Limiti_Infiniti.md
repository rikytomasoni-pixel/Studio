---
tags:
  - AM1
  - successioni
  - limiti
  - forme-indeterminate
  - algebra-dei-limiti
data: 2026-10-07
fonte: Lezione 8
---

# Algebra dei limiti con $\pm\infty$ e forme di indeterminazione

## Limiti di successioni razionali (potenze di $n$ e funzioni limitate)

**Esempio.**
$$a_n = \dfrac{3n^5 - 4n^3 + \log n - 8\arctan(n^2+1) - 3}{2n^{16/3} + 147\log n^{52} - \sin n}$$
$$= \dfrac{n^5\left(3 - \dfrac{4}{n^2} + \dfrac{\log n}{n^5} - 8\,\dfrac{\arctan(n^2+1)}{n^5} - \dfrac{3}{n^5}\right)}{n^{16/3}\left(2 + 147\cdot 52\,\dfrac{\log n}{n^{16/3}} - \dfrac{\sin n}{n^{16/3}}\right)}$$
dove i termini $\dfrac{4}{n^2}$, $\dfrac{\log n}{n^5}$, $\dfrac{\arctan(n^2+1)}{n^5}$, $\dfrac{3}{n^5}$, $\dfrac{\log n}{n^{16/3}}$, $\dfrac{\sin n}{n^{16/3}}$ tendono tutti a $0$. Quindi
$$a_n = \dfrac{1}{n^{1/3}}\cdot\dfrac{3+\cdots}{2+\cdots} \ \longrightarrow\ 0\cdot\dfrac{3+0}{2+0} = 0$$
$$\Rightarrow\quad \lim_{n\to\infty} a_n = 0$$

**Osservazione.** $a_n = \dfrac{P(n)}{Q(n)}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate in $n$ (o di funzioni "trascurabili" rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ (positiva) è più piccola della potenza massima di $n$ in $Q$ (positiva). Ragionando come sopra,
$$\lim_{n\to\infty} \dfrac{P(n)}{Q(n)} = 0$$

**Esempio.**
$$a_n = \dfrac{2n^5 - 47n^4 + \log\log n + \cos n}{5n^5 + \arctan\sqrt{n} + (\log n)^{42} - 1}$$
$$= \dfrac{n^5\left(2 - \dfrac{47}{n} + \dfrac{\log\log n}{n^5} + \dfrac{\cos n}{n^5}\right)}{n^5\left(5 + \dfrac{\arctan\sqrt{n}}{n^5} + \dfrac{(\log n)^{42}}{n^5} - \dfrac{1}{n^5}\right)}$$
dove $\dfrac{(\log n)^{42}}{n^5} = \left(\dfrac{\log n}{n^{5/42}}\right)^{42}\to 0$ e gli altri termini tendono a $0$. Quindi
$$a_n = 1\cdot\dfrac{2+\cdots}{5+\cdots} \ \longrightarrow\ \dfrac{2+0}{5+0} = \dfrac{2}{5}
\quad\Rightarrow\quad \lim_{n\to\infty} a_n = \dfrac{2}{5}$$

**Osservazione.** $a_n = \dfrac{P(n)}{Q(n)}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate in $n$ (oppure funzioni "trascurabili" rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ è uguale alla potenza massima di $n$ in $Q$ (entrambe positive). Allora
$$\lim_{n\to\infty} \dfrac{P(n)}{Q(n)} = l\in\mathbb{R}\setminus\{0\}$$
dove $l$ è il quoziente del coefficiente della potenza massima di $n$ in $P$ e del coefficiente della potenza massima di $n$ in $Q$.

## Aritmetizzazione parziale di $\overline{\mathbb{R}}$

> [!abstract] Teorema (aritmetizzazione parziale di $\infty$)
> Siano $a_n, b_n$ successioni.
>
> **1)** Se $\lim_{n\to\infty} a_n = a \in\mathbb{R}$ e $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} (a_n+b_n) = \pm\infty \qquad (a\pm\infty = \pm\infty \quad \forall\, a\in\mathbb{R})$$
>
> **2)** Se $\lim_{n\to\infty} a_n = \pm\infty$ e $\lim_{n\to\infty} b_n = \pm\infty$ (concordi in segno), allora
> $$\lim_{n\to\infty} (a_n+b_n) = \pm\infty \quad \text{(stesso segno)}$$
> $$(+\infty)+(+\infty)=+\infty \qquad (-\infty)+(-\infty)=-\infty$$
>
> **3)** Se $\lim_{n\to\infty} a_n = a \in\overline{\mathbb{R}}\setminus\{0\}$ e $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} a_nb_n = \pm\infty$$
> con l'usuale regola del prodotto dei segni:
> - $+\infty$ se $a>0$ e $\lim b_n=+\infty$, oppure $a<0$ e $\lim b_n=-\infty$
> - $-\infty$ altrimenti
>
> $$\pm\infty\cdot a = \begin{cases}+\infty\\-\infty\end{cases} \text{ con regola dei segni} \quad \forall\, a\in\overline{\mathbb{R}}\setminus\{0\}$$
>
> **4)** Se $\lim_{n\to\infty} a_n = a \in\overline{\mathbb{R}}\setminus\{0\}$ e $\lim_{n\to\infty} b_n = 0^\pm$ ($b_n\neq 0$ definitivamente), allora
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = \pm\infty$$
> con l'usuale regola del prodotto dei segni:
> - $+\infty$ se $a>0$ e $\lim b_n=0^+$, oppure $a<0$ e $\lim b_n=0^-$
> - $-\infty$ altrimenti
>
> $$\dfrac{a}{0^\pm} = \begin{cases}+\infty\\-\infty\end{cases} \text{ con regola dei segni} \quad \forall\, a\in\overline{\mathbb{R}}\setminus\{0\}$$
>
> **5)** Se $\lim_{n\to\infty} a_n = a \in\mathbb{R}$ e $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 0 \qquad \left(\dfrac{a}{\pm\infty} = 0 \quad \forall\, a\in\mathbb{R}\right)$$

## Forme di indeterminazione

**Osservazione.** $\infty-\infty$, $\infty\cdot 0$, $\dfrac{\infty}{\infty}$, $\dfrac{0}{0}$ sono **forme di indeterminazione** (nulla si può dire in generale).

**Esempi di forma indeterminata $[0\cdot\infty]$.**
$$a_n = \dfrac{1}{n},\ b_n=\sqrt{7}\,n \ \Rightarrow\ a_nb_n = \sqrt{7} \to \sqrt{7}$$
$$a_n = \dfrac{1}{n^2},\ b_n=\sqrt{7}\,n \ \Rightarrow\ a_nb_n = \dfrac{\sqrt{7}}{n} \to 0$$
$$a_n = \dfrac{1}{\sqrt{n}},\ b_n=\sqrt{7}\,n \ \Rightarrow\ a_nb_n = \sqrt{7}\sqrt{n} \to +\infty$$
$$a_n = \dfrac{(-1)^n}{n},\ b_n=\sqrt{7}\,n \ \Rightarrow\ a_nb_n = (-1)^n\sqrt{7} \text{ non ha limite}$$

**Esempio.**
$$\lim_{n\to\infty} \dfrac{18n^3 - n^{3/2} + \sin n + \log\log n}{-2n^2 + n^{3/4} - (\log n)^{18} + 7}$$
$$a_n = \dfrac{n^3\left(18 - n^{-3/2} + \dfrac{\sin n}{n^3} + \dfrac{\log\log n}{n^3}\right)}{n^2\left(-2 + n^{-5/4} - \dfrac{(\log n)^{18}}{n^2} + \dfrac{7}{n^2}\right)}$$
dove $n^{-3/2}$, $\dfrac{\sin n}{n^3}$, $\dfrac{\log\log n}{n^3}$, $n^{-5/4}$, $\dfrac{7}{n^2}$ e $\dfrac{(\log n)^{18}}{n^2} = \left(\dfrac{\log n}{n^{1/9}}\right)^{18}$ tendono tutti a $0$. Quindi
$$a_n = n\cdot\dfrac{18+\cdots}{-2+\cdots} \ \longrightarrow\ +\infty\cdot(-9) = -\infty
\quad\Rightarrow\quad \lim_{n\to\infty} a_n = -\infty$$

**Osservazione.** $a_n = \dfrac{P(n)}{Q(n)}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate in $n$ (o di funzioni "trascurabili" rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ (positiva) è maggiore della potenza massima di $n$ in $Q$ (positiva). Allora
$$\lim_{n\to\infty} \dfrac{P(n)}{Q(n)} = \pm\infty$$
Il segno $\pm$ è deciso dal prodotto dei segni dei coefficienti delle potenze massime di $n$ in $P,Q$.

**Esempio.**
$$a_n = \dfrac{7\cdot 2^n + \log\log n - \arctan n + n^7}{14\,n! - n^{42} + \sin n}
= \dfrac{2^n}{n!}\cdot\dfrac{7+\cdots}{14+\cdots} \ \longrightarrow\ 0\cdot\dfrac{7}{14} = 0$$
per gerarchia degli infiniti (vedi [[36_Gerarchia_degli_Infiniti]]).

## Razionalizzazione (tecnica per $\infty-\infty$)

**Esempio.** $a_n = \sqrt{n^2+n} - \sqrt{n^2-n}$

Posto $a=\sqrt{n^2+n}$, $b=\sqrt{n^2-n}$, si usa $a-b = \dfrac{(a-b)(a+b)}{a+b} = \dfrac{a^2-b^2}{a+b}$:
$$a_n = \dfrac{\left(\sqrt{n^2+n}-\sqrt{n^2-n}\right)\left(\sqrt{n^2+n}+\sqrt{n^2-n}\right)}{\sqrt{n^2+n}+\sqrt{n^2-n}}
= \dfrac{n^2+n-(n^2-n)}{n\sqrt{1+\frac{1}{n}}+n\sqrt{1-\frac{1}{n}}}$$
$$= \dfrac{2n}{n\left(\sqrt{1+\frac{1}{n}}+\sqrt{1-\frac{1}{n}}\right)} \ \longrightarrow\ \dfrac{2}{1+1} = 1$$

**Esempio.** $a_n = \sqrt[7]{n^2+n} - \sqrt[7]{n^2-n}$

Posto $a=\sqrt[7]{n^2+n}$, $b=\sqrt[7]{n^2-n}$, si usa
$$a^7-b^7 = (a-b)\left(a^6+a^5b+a^4b^2+a^3b^3+a^2b^4+ab^5+b^6\right)$$
e in generale
$$a^m-b^m = (a-b)\left(\sum_{k=0}^{m-1} a^{m-1-k}\,b^k\right)$$

**Esempio.** $a_n = (n^2+n)^{\frac{1}{\sqrt{2}}} - (n^2-n)^{\frac{1}{\sqrt{2}}}$. Quanto vale $\displaystyle\lim_{n\to\infty} a_n$ ?

## Esponenziali con base ed esponente variabili

**Osservazione.** $a_n^{\,b_n} = e^{\log a_n^{\,b_n}} = e^{b_n\log a_n}$

Se $\lim_{n\to\infty} a_n = a>0$ e $\lim_{n\to\infty} b_n = b\in\mathbb{R}$, allora
$$\lim_{n\to\infty} b_n\log a_n = b\log a \in\mathbb{R}$$
$$\Rightarrow\quad \lim_{n\to\infty} a_n^{\,b_n} = \lim_{n\to\infty} e^{b_n\log a_n} = e^{b\log a} = e^{\log a^b} = a^b$$

> [!abstract] Teorema
> Se $a_n, b_n$ sono successioni tali che $\lim_{n\to\infty} a_n = a\in\overline{\mathbb{R}}$, $a\geq 0$ (con $a_n>0$ definitivamente) e $\lim_{n\to\infty} b_n = b\in\overline{\mathbb{R}}$. Allora
> $$\lim_{n\to\infty} a_n^{\,b_n} = a^b$$
> (salvo forme di indeterminazione), dove
> $$a^{+\infty} = +\infty \quad \forall\, a>1 \ \text{(anche } a=+\infty\text{)}$$
> $$a^{-\infty} = 0 \quad \forall\, a>1 \ \text{(anche } a=+\infty\text{)}$$
> $$a^{+\infty} = 0 \quad \forall\, a\in[0,1)$$
> $$a^{-\infty} = +\infty \quad \forall\, a\in[0,1)$$
> $$(+\infty)^b = +\infty \quad \forall\, b>0 \ \text{(anche } b=+\infty\text{)}$$
> $$(+\infty)^b = 0 \quad \forall\, b<0 \ \text{(anche } b=-\infty\text{)}$$

**Osservazione.** $\infty^0$, $0^0$, $1^{\pm\infty}$ sono esclusi: sono forme di indeterminazione.

**Osservazione.**
$$a_n\equiv 1,\ b_n=n \ \Rightarrow\ a_n^{\,b_n} = 1^n = 1 \to 1$$
$$a_n\equiv 0,\ b_n=n \ \Rightarrow\ a_n\cdot b_n = 0 \to 0$$
non sono forme di indeterminazione.

### Note collegate
- [[00_MOC_Analisi_1]]
- [[34_Algebra_dei_Limiti]] — algebra dei limiti per successioni convergenti
- [[36_Gerarchia_degli_Infiniti]]
- [[38_Numero_di_Nepero]] — applicazione delle forme $1^\infty$
- [[12_Logaritmi]]

#AM1/successioni-e-limiti/algebra-limiti-infiniti
