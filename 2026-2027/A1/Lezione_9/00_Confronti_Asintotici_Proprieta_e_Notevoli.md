---
tags:
  - AM1
  - successioni
  - o-piccolo
  - asintotico
  - confronti-asintotici
data: 2026-10-09
fonte: Lezione 9
immagini_mancanti: false
---

# Proprietà degli infinitesimi equivalenti e o-piccolo

Richiamo: date $a_n, b_n$ successioni ($b_n\neq 0$ definitivamente in $n\in\mathbb{N}$):
$$\lim_{n\to\infty}\dfrac{a_n}{b_n}=0 \ \Rightarrow\ a_n=o(b_n) \ \text{ per } n\to\infty \qquad \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \ \Rightarrow\ a_n\sim b_n$$
(vedi [[04_o_piccolo_e_Asintotico]])

## Caratterizzazione dell'equivalenza asintotica

> [!abstract] Proposizione
> $$a_n\sim b_n \quad\Longleftrightarrow\quad a_n=b_n+o(b_n)$$

**dim:**
$$a_n\sim b_n \iff \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \iff \lim_{n\to\infty}\left(\dfrac{a_n}{b_n}-1\right)=0 \iff \lim_{n\to\infty}\dfrac{a_n-b_n}{b_n}=0 \iff a_n-b_n=o(b_n) \iff a_n=(a_n-b_n)+b_n=b_n+o(b_n)$$

**Oss:** $b_n=o(1)$ per definizione, infatti $\lim_{n\to\infty}\dfrac{b_n}{1}=0$, cioè $\lim_{n\to\infty} b_n=0$, cioè $b_n$ è infinitesima.

## Proprietà di $\sim$

> [!note] Osservazione
> - $a_n\sim a_n$ (ovvio)
> - $a_n\sim b_n$ e $b_n\sim c_n \ \Rightarrow\ a_n\sim c_n$. Infatti $\dfrac{a_n}{c_n}=\dfrac{a_n}{b_n}\cdot\dfrac{b_n}{c_n}\to 1\cdot 1=1$
> - $a_n\sim b_n \ \Rightarrow\ b_n\sim a_n$. Infatti $\dfrac{b_n}{a_n}=\left(\dfrac{a_n}{b_n}\right)^{-1}\to 1^{-1}=1$
>
> $\sim$ è una relazione di equivalenza fra successioni (definitivamente $\neq 0$).

## Esempi per $n\to\infty$

*(Es: foglio "Asintotici notevoli" su WeBeep)*

$$\sin\dfrac1n\sim\dfrac1n, \qquad \sin\dfrac1n=\dfrac1n+o\!\left(\dfrac1n\right)$$
$$e^{1/n}-1\sim\dfrac1n, \qquad e^{1/n}-1=\dfrac1n+o\!\left(\dfrac1n\right)\ \Rightarrow\ e^{1/n}=1+\dfrac1n+o\!\left(\dfrac1n\right)$$
$$\log\left(1+\dfrac1n\right)\sim\dfrac1n, \qquad \log\left(1+\dfrac1n\right)=\dfrac1n+o\!\left(\dfrac1n\right)$$
$$1-\cos\dfrac1n\sim\dfrac{1}{2n^2}, \qquad 1-\cos\dfrac1n=\dfrac{1}{2n^2}+o\!\left(\dfrac1{n^2}\right)\ \Rightarrow\ \cos\dfrac1n=1-\dfrac{1}{2n^2}+o\!\left(\dfrac1{n^2}\right)$$
$$\left(1+\dfrac1n\right)^\alpha-1\sim\dfrac\alpha n\ \ (\alpha\neq0), \qquad \left(1+\dfrac1n\right)^\alpha-1=\dfrac\alpha n+o\!\left(\dfrac1n\right)\ \Rightarrow\ \left(1+\dfrac1n\right)^\alpha=1+\dfrac\alpha n+o\!\left(\dfrac1n\right)$$
$$\arctan\dfrac1n\sim\dfrac1n, \qquad \arctan\dfrac1n=\dfrac1n+o\!\left(\dfrac1n\right)$$

## Compatibilità di $\sim$ con prodotto, quoziente, potenza e limite

> [!abstract] Proposizione
> 1. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora $a_n b_n \sim a_n' b_n'$
> 2. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$
> 3. Se $a_n\sim a_n'$, $\alpha\in\mathbb{R}$, allora $a_n^{\,\alpha}\sim (a_n')^{\,\alpha}$ (assumendo che l'operazione abbia senso…)
> 4. Se $a_n\sim a_n'$ allora le due successioni hanno lo stesso carattere, cioè: o convergono entrambe allo stesso limite $l\in\mathbb{R}$, o divergono entrambe a $+\infty$, o entrambe a $-\infty$, o sono entrambe indeterminate

> [!danger] Attenzione
> In generale, se $a_n\sim a_n'$ e $b_n\sim b_n'$, **non è detto** che
> $$a_n\pm b_n\sim a_n'\pm b_n' \qquad a_n^{\,b_n}\sim(a_n')^{\,b_n'} \qquad e^{a_n}\sim e^{a_n'} \qquad \log(a_n)\sim\log(a_n')$$

> [!danger] Attenzione
> In generale
> $$a_n\sim b_n \ \not\Rightarrow\ a_n-b_n\to 0 \qquad\qquad a_n-b_n\to 0 \ \not\Rightarrow\ a_n\sim b_n$$

**dim (della proposizione):** $a_n\sim a_n'$, $b_n\sim b_n'$

1. $$\dfrac{a_n'b_n'}{a_nb_n}=\left(\dfrac{a_n'}{a_n}\right)\cdot\left(\dfrac{b_n'}{b_n}\right)\to 1\cdot1=1$$

2. $$\dfrac{\dfrac{a_n}{b_n}}{\dfrac{a_n'}{b_n'}}=\dfrac{a_n}{b_n}\cdot\dfrac{b_n'}{a_n'}=\left(\dfrac{a_n}{a_n'}\right)\cdot\left(\dfrac{b_n}{b_n'}\right)^{-1}\to 1\cdot1^{-1}=1$$

3. $$\dfrac{a_n^{\,\alpha}}{(a_n')^{\alpha}}=\left(\dfrac{a_n}{a_n'}\right)^{\alpha}\to 1^\alpha=1$$

4. $a_n, a_n'$ hanno lo stesso comportamento al limite.
   Se $\exists\,\lim_{n\to\infty}a_n'=l\in\overline{\mathbb{R}}$, allora $a_n=\dfrac{a_n}{a_n'}\cdot a_n'\to 1\cdot l=l\in\overline{\mathbb{R}}$.
   Se invece $a_n$ non ammette limite in $\overline{\mathbb{R}}$ e per assurdo $\exists\,\lim_{n\to\infty}a_n'=l\in\overline{\mathbb{R}}$, allora $a_n=\dfrac{a_n}{a_n'}\cdot a_n'\to 1\cdot l=l\in\overline{\mathbb{R}}$, cioè $\exists\,\lim_{n\to\infty}a_n=l\in\overline{\mathbb{R}}$, assurdo. Quindi $\nexists\,\lim_{n\to\infty}a_n'$ in $\overline{\mathbb{R}}$. $\square$

## Esempio

$$a_n=\dfrac{3n^7+5n^{42/95}+\log n-\cos n+5}{2n^6-18n^3+\arctan n+(\log n)^2-2}$$

$$N=3n^7+o(n^7)\sim 3n^7, \qquad D=2n^6+o(n^6)\sim 2n^6$$
$$a_n=\dfrac{3n^7+o(n^7)}{2n^6+o(n^6)}\sim\dfrac{3n^7}{2n^6}=\dfrac32\,n\to+\infty \quad\Rightarrow\quad \lim_{n\to\infty}a_n=+\infty$$

## Asintotici notevoli

*(Es: foglio asintotici su WeBeep)*

Se $\varepsilon_n\to0$ ($\varepsilon_n\neq0$ definitivamente), allora per $n\to\infty$:

$$\sin\varepsilon_n\sim\varepsilon_n, \qquad \sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$$
$$1-\cos\varepsilon_n\sim\dfrac{\varepsilon_n^2}{2}, \qquad 1-\cos\varepsilon_n=\dfrac{\varepsilon_n^2}{2}+o(\varepsilon_n^2), \qquad \cos\varepsilon_n=1-\dfrac{\varepsilon_n^2}{2}+o(\varepsilon_n^2)$$
$$e^{\varepsilon_n}-1\sim\varepsilon_n, \qquad e^{\varepsilon_n}-1=\varepsilon_n+o(\varepsilon_n), \qquad e^{\varepsilon_n}=1+\varepsilon_n+o(\varepsilon_n)$$
$$\log(1+\varepsilon_n)\sim\varepsilon_n, \qquad \log(1+\varepsilon_n)=\varepsilon_n+o(\varepsilon_n)$$
$$(1+\varepsilon_n)^\alpha-1\sim\alpha\,\varepsilon_n \ \ (\alpha\neq0), \qquad (1+\varepsilon_n)^\alpha-1=\alpha\,\varepsilon_n+o(\varepsilon_n), \qquad (1+\varepsilon_n)^\alpha=1+\alpha\,\varepsilon_n+o(\varepsilon_n)$$
$$\arctan\varepsilon_n\sim\varepsilon_n, \qquad \arctan\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$$

> [!note] Osservazione
> $\varepsilon_n\to0$ non richiede che $\varepsilon_n$ sia monotona o positiva. Nel quaderno è disegnata la successione $\varepsilon_0,\varepsilon_1,\varepsilon_2,\varepsilon_3,\dots,\varepsilon_n$ con i punti sopra e sotto l'asse che si avvicinano a $0$ al crescere di $n$.

## Esempio

$$a_n=\dfrac{\sin\dfrac1{n^2}}{e^{7/n}-1}\cdot n$$

- $\varepsilon_n=\dfrac1{n^2}\to0$, $\sin\varepsilon_n\sim\varepsilon_n$: quindi $\sin\dfrac1{n^2}\sim\dfrac1{n^2}$
- $\varepsilon_n=\dfrac7n\to0$, $e^{\varepsilon_n}-1\sim\varepsilon_n$: quindi $e^{7/n}-1\sim\dfrac7n$

$$a_n\sim\dfrac{\dfrac1{n^2}}{\dfrac7n}\cdot n=\dfrac17 \quad\Rightarrow\quad \lim_{n\to\infty}a_n=\dfrac17$$

## Esempio (con radice cubica)

$$a_n=\dfrac{\sqrt[3]{1+n}-n^{1/3}}{1-e^{2/n}}\cdot\arctan\dfrac1{n^2}\cdot n^{5/3}$$

- $\arctan\dfrac1{n^2}\sim\dfrac1{n^2}$ (con $\varepsilon_n=\dfrac1{n^2}\to0$)
- $1-e^{2/n}\sim-\dfrac2n$, infatti $-(e^{\varepsilon_n}-1)\sim-\varepsilon_n$ con $\varepsilon_n=\dfrac2n\to0$
- $\sqrt[3]{1+n}-n^{1/3}\sim\ ?$

Si ha $(1+\varepsilon_n)^\alpha-1\sim\alpha\varepsilon_n$, $(1+\varepsilon_n)^\alpha=1+\alpha\varepsilon_n+o(\varepsilon_n)$ per $\varepsilon_n\to0$.

> [!danger] Attenzione — non si può fare così
> - $\sqrt[3]{1+n}=(1+n)^{1/3}\neq 1+\dfrac n3+o(n)$, perché $\varepsilon_n=n\not\to0$.
> - $\sqrt[3]{1+n}\sim n^{1/3}$ è vero, ma **non** ne segue $\sqrt[3]{1+n}-n^{1/3}\sim n^{1/3}-n^{1/3}=0$: non si può usare $\sim$ in somme e sottrazioni.

Procedimento corretto: $\sqrt[3]{1+n}=n^{1/3}\left(1+\dfrac1n\right)^{1/3}$, con $\varepsilon_n=\dfrac1n$ e $\alpha=\dfrac13$ nello sviluppo $(1+\varepsilon_n)^\alpha$:
$$\sqrt[3]{1+n}=n^{1/3}\left(1+\dfrac1{3n}+o\!\left(\dfrac1n\right)\right)=n^{1/3}+\dfrac1{3n^{2/3}}+n^{1/3}\cdot o\!\left(\dfrac1n\right)$$
dove $n^{1/3}\cdot o\!\left(\dfrac1n\right)=o\!\left(\dfrac1{n^{2/3}}\right)$. Infatti $\dfrac{n^{1/3}\cdot o\!\left(\frac1n\right)}{\frac1{n^{2/3}}}=\dfrac{o\!\left(\frac1n\right)}{\frac1n}\to0$. Quindi
$$\sqrt[3]{1+n}-n^{1/3}=\dfrac1{3n^{2/3}}+o\!\left(\dfrac1{n^{2/3}}\right)\sim\dfrac1{3n^{2/3}}$$
e
$$a_n\sim\dfrac{\dfrac1{3n^{2/3}}}{-\dfrac2n}\cdot\dfrac1{n^2}\cdot n^{5/3}=-\dfrac16 \quad\Rightarrow\quad \lim_{n\to\infty}a_n=-\dfrac16$$

## Esempio (sviluppo con radice cubica, differenza)

$$a_n=\left(n^3+n^2\right)^{1/3}-\left(n^3-n\right)^{1/3}$$

Il quaderno parte dall'identità $a^3-b^3=(a-b)(a^2+ab+b^2)$ con $a=\sqrt[3]{n^3+n^2}$, $b=\sqrt[3]{n^3-n}$, quindi $a-b=\dfrac{a^3-b^3}{a^2+ab+b^2}$, ma poi prosegue con gli sviluppi, che qui sono riportati. Con $(1+\varepsilon_n)^\alpha=1+\alpha\varepsilon_n+o(\varepsilon_n)$:

$$\left(n^3+n^2\right)^{1/3}=n\left(1+\dfrac1n\right)^{1/3}=n\left(1+\dfrac1{3n}+o\!\left(\dfrac1n\right)\right)\ \sim n$$
$$\left(n^3-n\right)^{1/3}=n\left(1-\dfrac1{n^2}\right)^{1/3}=n\left(1-\dfrac1{3n^2}+o\!\left(\dfrac1{n^2}\right)\right)\ \sim n$$

$$\begin{aligned}a_n&=n\left(1+\dfrac1{3n}+o\!\left(\dfrac1n\right)\right)-n\left(1-\dfrac1{3n^2}+o\!\left(\dfrac1{n^2}\right)\right)\\&=\cancel{n}+\dfrac13+n\,o\!\left(\dfrac1n\right)-\cancel{n}+\dfrac1{3n}+n\,o\!\left(\dfrac1{n^2}\right)\\&=\dfrac13+\dfrac1{3n}+n\,o\!\left(\dfrac1n\right)+n\,o\!\left(\dfrac1{n^2}\right)\end{aligned}$$

dove $n\,o\!\left(\dfrac1n\right)=o(1)$ e $n\,o\!\left(\dfrac1{n^2}\right)=o\!\left(\dfrac1n\right)$, quindi la somma dei due è $o(1)$. Infatti $\dfrac{n\cdot o\left(\frac1n\right)}{1}=\dfrac{o\left(\frac1n\right)}{\frac1n}\to0$ e $\dfrac{n\cdot o\left(\frac1{n^2}\right)}{\frac1n}=\dfrac{o\left(\frac1{n^2}\right)}{\frac1{n^2}}\to0$.

$$a_n=\dfrac13+\dfrac1{3n}+o(1)=\dfrac13+o(1)\ \longrightarrow\ \dfrac13$$

## Proprietà di o-piccolo

> [!note] Osservazioni
> - $a_n\cdot o(b_n)=o(a_nb_n)$. Infatti $\dfrac{a_n\cdot o(b_n)}{a_nb_n}=\dfrac{o(b_n)}{b_n}\to0$ per definizione
> - $o(a_n)=a_n\cdot o(1)$
> - $c\cdot o(a_n)=o(a_n)\quad\forall\,c\neq0$. Infatti $\dfrac{c\cdot o(a_n)}{a_n}\to c\cdot0=0$
> - $\pm\,o(a_n)=o(a_n)$
> - $o\!\left(\dfrac1n\right)+o\!\left(\dfrac1{n^2}\right)=o\!\left(\dfrac1n\right)$
> - $o(n)+o(n^2)=o(n^2)$
> - se $a_n\sim b_n\ \Rightarrow\ o(a_n)=o(b_n)$. Infatti $\dfrac{o(a_n)}{b_n}=\dfrac{o(a_n)}{a_n}\cdot\dfrac{a_n}{b_n}\to0\cdot1=0$. Ad esempio $o\!\left(\sin\dfrac1n\right)=o\!\left(\dfrac1n\right)$

## Esempio

$$a_n=\dfrac{\sin\dfrac1n-\dfrac1n}{\dfrac1{n^3}}\qquad\left[\tfrac00\right]\ \text{forma indeterminata}$$

Con $\varepsilon_n=\dfrac1n\to0$: $\sin\varepsilon_n\sim\varepsilon_n$, $\sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$. Quindi
$$\sin\dfrac1n-\dfrac1n=\dfrac1n+o\!\left(\dfrac1n\right)-\dfrac1n=o\!\left(\dfrac1n\right)$$
$$\Rightarrow\quad a_n=\dfrac{o\!\left(\dfrac1n\right)}{\dfrac1{n^3}}=n^3\,o\!\left(\dfrac1n\right)=o(n^2)$$

$\lim_{n\to\infty}a_n=\ ?$ Nel quaderno l'esempio si ferma qui, con il limite lasciato come domanda aperta ($o(n^2)$ da solo non basta per concludere).

> [!warning] Aggiunte presenti nella versione precedente ma non nel PDF manoscritto
> Affermazioni corrette ma che non compaiono nelle pagine della Lezione 9. Se non le hai prese da un'altra fonte, puoi cancellarle.
> - $a_n\sim b_n\ \Rightarrow\ a_n, b_n$ hanno lo stesso segno definitivamente
> - $o(a_n)\cdot o(b_n)=o(a_nb_n)$ e $o\big(o(a_n)\big)=o(a_n)$
> - $a_n-b_n=o(a_n)\iff a_n\sim b_n$

### Note collegate
- [[00_MOC_A1]]
- [[04_o_piccolo_e_Asintotico]] — definizioni di o-piccolo e asintotico, gerarchia in termini di o-piccolo
- [[03_Confronti_Asintotici]] — ordine di infinito
- [[04_Gerarchia_degli_Infiniti]]
- [[00_Algebra_Limiti_Infiniti]]
- [[02_Criterio_del_Rapporto]]
- [[02_Algebra_dei_Limiti]]
