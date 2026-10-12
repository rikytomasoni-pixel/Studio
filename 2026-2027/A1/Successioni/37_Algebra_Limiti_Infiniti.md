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

> [!abstract] Teorema — Aritmetizzazione parziale di $\overline{\mathbb{R}}$
> Siano $a_n, b_n$ successioni.
>
> **1)** Se $\lim_{n\to\infty} a_n = l \in\mathbb{R}$, $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} (a_n+b_n) = \pm\infty \qquad (l+(\pm\infty) = \pm\infty, \ \forall\, l\in\mathbb{R})$$
>
> **2)** Se $\lim_{n\to\infty} a_n = +\infty$, $\lim_{n\to\infty} b_n = +\infty$ (concordi in segno), allora
> $$\lim_{n\to\infty} (a_n+b_n) = +\infty$$
> (stesso segno: $(+\infty)+(+\infty)=+\infty$, $(-\infty)+(-\infty)=-\infty$)
>
> **3)** Se $\lim_{n\to\infty} a_n = l \in\mathbb{R}\setminus\{0\}$, $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} a_n b_n = \pm\infty$$
> con l'usuale regola del prodotto dei segni:
> $$l>0,\ \lim b_n=+\infty \ \Rightarrow\ \lim a_n b_n = +\infty$$
> $$l>0,\ \lim b_n=-\infty \ \Rightarrow\ \lim a_n b_n = -\infty \quad \text{(altrimenti con regola dei segni per } l<0\text{)}$$
>
> **4)** Se $\lim_{n\to\infty} a_n = a\in\mathbb{R}\setminus\{0\}$ e $\lim_{n\to\infty} b_n = 0^{\pm}$ ($b_n\neq 0$ definitivamente), allora
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = \pm\infty$$
> con l'usuale regola del prodotto dei segni: $a>0$ e $\lim b_n=0^+$ $\Rightarrow$ $\lim \dfrac{a_n}{b_n}=+\infty$; $a<0$ e $\lim b_n=0^+$ $\Rightarrow$ $\lim \dfrac{a_n}{b_n}=-\infty$ (altrimenti con regola dei segni).
>
> **5)** Se $\lim_{n\to\infty} a_n = a\in\mathbb{R}$, $\lim_{n\to\infty} b_n = \pm\infty$, allora
> $$\lim_{n\to\infty} \dfrac{a_n}{b_n} = 0 \qquad \forall\, a\in\mathbb{R}$$

**Osservazione.** $0\cdot\infty$, $\infty-\infty$, $\dfrac{\infty}{\infty}$, $\dfrac{0}{0}$ sono **forme di indeterminazione**: nulla si può dire in generale.

**Esempi di forme indeterminate.**
$$a_n = n, \quad b_n = \dfrac{1}{n} \ \Rightarrow\ a_n\cdot b_n = 1 \to 1 \qquad [0\cdot\infty]$$
$$a_n = n, \quad b_n = n^2 \ \Rightarrow\ a_n - b_n = n-n^2 \to -\infty \qquad [\infty-\infty]$$
$$a_n = n, \quad b_n = n^2+n \ \Rightarrow\ a_n - b_n = -n^2 \to -\infty \qquad [\infty-\infty]$$
$$a_n = n+(-1)^n, \quad b_n = n \ \Rightarrow\ a_n - b_n = (-1)^n \text{ non ha limite} \qquad [\infty-\infty]$$

## Esempi con limiti di successioni razionali (rapporto di polinomi/potenze e funzioni limitate)

**Esempio.**
$$a_n = \dfrac{n+\sin n + \log\log n}{2n+\cdots}$$
$$\lim_{n\to\infty} a_n = 0$$

**Osservazione.** $a_n = \dfrac{P}{Q}$, dove $P, Q$ sono somme di potenze di $n$ e di funzioni limitate in $n$ (o "trascurabili" rispetto a potenze di $n$): se la potenza massima di $n$ in $P$ (positiva) è più piccola della potenza massima di $n$ in $Q$ (positiva), allora, ragionando come sopra,
$$\lim_{n\to\infty} a_n = 0$$

**Esempio.**
$$a_n = \dfrac{5n+\cdots}{n+\cdots} \quad\Rightarrow\quad \lim_{n\to\infty} a_n = \dfrac{5+0}{1+0} = 5$$

**Osservazione.** $a_n=\dfrac{P}{Q}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate (o trascurabili rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ è uguale alla potenza massima di $n$ in $Q$ (entrambe positive). Allora
$$\lim_{n\to\infty} a_n = l$$
dove $l$ è il quoziente del coefficiente della potenza massima di $n$ in $P$ e del coefficiente della potenza massima di $n$ in $Q$.

**Esempio.**
$$a_n = \dfrac{\sin n + \log\log n + \cdots}{\log n + \cdots}$$
$$\lim_{n\to\infty} a_n = -\infty$$

**Osservazione.** $a_n=\dfrac{P}{Q}$, dove $P,Q$ sono somme di potenze di $n$ e di funzioni limitate di $n$ (o trascurabili rispetto a potenze di $n$), dove la potenza massima di $n$ in $P$ (positiva) è maggiore della potenza massima di $n$ in $Q$ (positiva). Allora
$$a_n \to \pm\infty, \quad \text{segno deciso dal prodotto dei segni dei coefficienti delle potenze massime di } n \text{ in } P, Q$$

**Esempio.** $a_n = \dfrac{n!}{n^n} \to 0$ per gerarchia degli infiniti (vedi [[36_Gerarchia_degli_Infiniti]]).

## Razionalizzazione (tecnica per $\infty-\infty$)

**Esempio.** $a_n = \sqrt{n} - \sqrt{n-1}$

$$a_n = \dfrac{(\sqrt{n}-\sqrt{n-1})(\sqrt{n}+\sqrt{n-1})}{\sqrt{n}+\sqrt{n-1}} = \dfrac{n-(n-1)}{\sqrt{n}+\sqrt{n-1}} = \dfrac{1}{\sqrt{n}+\sqrt{n-1}} \to 0$$

**Esempio.** $a_n = \sqrt{n^2+n}-n-\dfrac{1}{2}$

Usando $(a^7-b^7)=(a-b)(a^6+a^5b+a^4b^2+a^3b^3+a^2b^4+ab^5+b^6)$ (razionalizzazione con potenze superiori), oppure tecniche analoghe con radici, si ottiene
$$\lim_{n\to\infty} a_n = 0$$

## Esponenziali con base ed esponente variabili

**Osservazione.** $a_n = e^{b_n\log a_n}$

Se $\lim_{n\to\infty} a_n = a>0$ e $\lim_{n\to\infty} b_n = b\in\mathbb{R}$, allora
$$\lim_{n\to\infty} b_n\log a_n = b\log a \quad \text{(per algebra dei limiti; vedi [[34_Algebra_dei_Limiti]])}$$
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

### Note collegate
- [[00_MOC_A1]]
- [[34_Algebra_dei_Limiti]] — algebra dei limiti per successioni convergenti
- [[36_Gerarchia_degli_Infiniti]]
- [[38_Numero_di_Nepero]] — applicazione delle forme $1^\infty$
- [[12_Logaritmi]]