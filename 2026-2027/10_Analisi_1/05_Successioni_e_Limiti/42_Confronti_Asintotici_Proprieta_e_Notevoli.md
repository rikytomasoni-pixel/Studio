---
tags:
  - AM1
  - successioni
  - o-piccolo
  - asintotico
  - confronti-asintotici
data: 2026-10-09
fonte: Lezione 9
---

# Asintotici e $o$-piccolo: proprietà e asintotici notevoli

> [!warning] Definizione
> Date $a_n, b_n$ successioni ($b_n\neq 0$ definitivamente in $n\in\mathbb{N}$):
> - se $\displaystyle\lim_{n\to\infty}\dfrac{a_n}{b_n}=0$ scriviamo $a_n=o(b_n)$
> - se $\displaystyle\lim_{n\to\infty}\dfrac{a_n}{b_n}=1$ scriviamo $a_n\sim b_n$
>
> (vedi [[41_o_piccolo_e_Asintotico]])

## Caratterizzazione dell'equivalenza asintotica

**Osservazione.** $a_n\sim b_n \iff a_n=b_n+o(b_n)$

Infatti:
$$a_n\sim b_n \iff \lim_{n\to\infty}\dfrac{a_n}{b_n}=1 \iff \lim_{n\to\infty}\left(\dfrac{a_n}{b_n}-1\right)=0 \iff \lim_{n\to\infty}\dfrac{a_n-b_n}{b_n}=0$$
$$\iff a_n-b_n=o(b_n) \iff a_n=(a_n-b_n)+b_n=b_n+o(b_n)$$

**Osservazione.** $b_n=o(1)$ per definizione, infatti
$$\lim_{n\to\infty}\dfrac{b_n}{1}=0$$
cioè $\displaystyle\lim_{n\to\infty} b_n=0$, cioè $b_n$ è infinitesima.

## Proprietà di $\sim$

**Osservazioni.**
- $a_n\sim a_n$ (ovvio)
- $a_n\sim b_n$ e $b_n\sim c_n$ $\Rightarrow$ $a_n\sim c_n$. Infatti
$$\dfrac{a_n}{c_n}=\dfrac{a_n}{b_n}\cdot\dfrac{b_n}{c_n}\to 1\cdot 1=1$$
- $a_n\sim b_n$ $\Rightarrow$ $b_n\sim a_n$. Infatti
$$\dfrac{b_n}{a_n}=\left(\dfrac{a_n}{b_n}\right)^{-1}\to 1^{-1}=1$$

$\sim$ è una **relazione di equivalenza** fra successioni (definitivamente $\neq 0$).

## Asintotici notevoli

*(Vedi il "foglio asintotici notevoli" su WeBeep.)*

**Esempio.** Per $n\to\infty$:

$$\sin\dfrac1n\sim\dfrac1n \qquad\qquad \sin\dfrac1n=\dfrac1n+o\!\left(\dfrac1n\right)$$
$$e^{\frac1n}-1\sim\dfrac1n \qquad\qquad e^{\frac1n}-1=\dfrac1n+o\!\left(\dfrac1n\right) \ \Rightarrow\ e^{\frac1n}=1+\dfrac1n+o\!\left(\dfrac1n\right)$$
$$\log\left(1+\dfrac1n\right)\sim\dfrac1n \qquad\qquad \log\left(1+\dfrac1n\right)=\dfrac1n+o\!\left(\dfrac1n\right)$$
$$1-\cos\dfrac1n\sim\dfrac{1}{2n^2} \qquad\qquad 1-\cos\dfrac1n=\dfrac{1}{2n^2}+o\!\left(\dfrac1{n^2}\right) \ \Rightarrow\ \cos\dfrac1n=1-\dfrac{1}{2n^2}+o\!\left(\dfrac1{n^2}\right)$$
$$\left(1+\dfrac1n\right)^\alpha-1\sim\dfrac{\alpha}{n}\ \ (\alpha\neq 0) \qquad \left(1+\dfrac1n\right)^\alpha-1=\dfrac{\alpha}{n}+o\!\left(\dfrac1n\right) \ \Rightarrow\ \left(1+\dfrac1n\right)^\alpha=1+\dfrac{\alpha}{n}+o\!\left(\dfrac1n\right)$$
$$\arctan\dfrac1n\sim\dfrac1n \qquad\qquad \arctan\dfrac1n=\dfrac1n+o\!\left(\dfrac1n\right)$$
$$\ldots$$

## Proprietà di compatibilità di $\sim$

> [!abstract] Proposizione
> 1. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ $\Rightarrow$ $a_nb_n\sim a_n'b_n'$
> 2. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ $\Rightarrow$ $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$
> 3. Se $a_n\sim a_n'$, $\alpha\in\mathbb{R}$ $\Rightarrow$ $a_n^{\,\alpha}\sim(a_n')^{\,\alpha}$ (assumendo che l'operazione abbia senso)
> 4. Se $a_n\sim a_n'$ allora le due successioni hanno lo stesso carattere, cioè o convergono entrambe allo stesso limite $l\in\mathbb{R}$, o divergono entrambe a $+\infty$, o entrambe a $-\infty$, o sono entrambe indeterminate (non ammettono limite).

**Osservazione.** In generale, $a_n\sim a_n'$ e $b_n\sim b_n'$ **non implicano**
$$a_n\pm b_n\sim a_n'\pm b_n', \qquad a_n^{\,b_n}\sim(a_n')^{\,b_n'}, \qquad e^{a_n}\sim e^{a_n'}, \qquad \log(a_n)\sim\log(a_n')$$

**Osservazione.** In generale:
$$a_n\sim b_n \ \not\Rightarrow\ a_n-b_n\to 0 \qquad\qquad a_n-b_n\to 0 \ \not\Rightarrow\ a_n\sim b_n$$

**dim (della proposizione).** Siano $a_n\sim a_n'$, $b_n\sim b_n'$.

1. $\dfrac{a_n'b_n'}{a_nb_n}=\left(\dfrac{a_n'}{a_n}\right)\cdot\left(\dfrac{b_n'}{b_n}\right)\to 1\cdot 1=1$, quindi $a_nb_n\sim a_n'b_n'$.

2. $\dfrac{\;\dfrac{a_n}{b_n}\;}{\dfrac{a_n'}{b_n'}}=\dfrac{a_n}{b_n}\cdot\dfrac{b_n'}{a_n'}=\left(\dfrac{a_n}{a_n'}\right)\cdot\left(\dfrac{b_n}{b_n'}\right)^{-1}\to 1\cdot 1^{-1}=1$, quindi $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$.

3. $\dfrac{a_n^{\,\alpha}}{(a_n')^{\alpha}}=\left(\dfrac{a_n}{a_n'}\right)^{\alpha}\to 1^\alpha=1$, quindi $a_n^{\,\alpha}\sim(a_n')^{\alpha}$.

4. Se $\exists\,\displaystyle\lim_{n\to\infty}a_n'=l\in\overline{\mathbb{R}}$, allora
$$a_n=\dfrac{a_n}{a_n'}\cdot a_n'\to 1\cdot l=l\in\overline{\mathbb{R}}$$
Se invece $a_n'$ non ammette limite in $\overline{\mathbb{R}}$, per assurdo supponiamo $\exists\,\displaystyle\lim_{n\to\infty}a_n=l\in\overline{\mathbb{R}}$; allora
$$a_n'=\dfrac{a_n'}{a_n}\cdot a_n\to 1\cdot l=l\in\overline{\mathbb{R}}$$
cioè $\exists\,\displaystyle\lim_{n\to\infty}a_n'=l\in\overline{\mathbb{R}}$, assurdo. Quindi $\nexists\,\displaystyle\lim_{n\to\infty}a_n$ in $\overline{\mathbb{R}}$. $\blacksquare$

**Esempio.**
$$a_n=\dfrac{3n^7+5n^{42/95}-\log n-\cos n+5}{2n^6-18n^3+\arctan n+(\log n)^2-2}$$
Numeratore: $N=3n^7+o(n^7)\sim 3n^7$. Denominatore: $D=2n^6+o(n^6)\sim 2n^6$. Quindi
$$a_n=\dfrac{3n^7+o(n^7)}{2n^6+o(n^6)}\sim\dfrac{3n^7}{2n^6}=\dfrac32\,n\to+\infty \quad\Rightarrow\quad \lim_{n\to\infty}a_n=+\infty$$

## Asintotici notevoli con $\varepsilon_n\to 0$

**Esempio.** *(foglio asintotici su WeBeep)* Se $\varepsilon_n\to0$ ($\varepsilon_n\neq 0$ definitivamente) allora, per $n\to\infty$:

$$\sin\varepsilon_n\sim\varepsilon_n \qquad \sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$$
$$1-\cos\varepsilon_n\sim\dfrac{\varepsilon_n^2}{2} \qquad 1-\cos\varepsilon_n=\dfrac{\varepsilon_n^2}{2}+o(\varepsilon_n^2) \ \Rightarrow\ \cos\varepsilon_n=1-\dfrac{\varepsilon_n^2}{2}+o(\varepsilon_n^2)$$
$$e^{\varepsilon_n}-1\sim\varepsilon_n \qquad e^{\varepsilon_n}-1=\varepsilon_n+o(\varepsilon_n) \ \Rightarrow\ e^{\varepsilon_n}=1+\varepsilon_n+o(\varepsilon_n)$$
$$\log(1+\varepsilon_n)\sim\varepsilon_n \qquad \log(1+\varepsilon_n)=\varepsilon_n+o(\varepsilon_n)$$
$$(1+\varepsilon_n)^\alpha-1\sim\alpha\varepsilon_n\ \ (\alpha\neq 0) \qquad (1+\varepsilon_n)^\alpha-1=\alpha\varepsilon_n+o(\varepsilon_n) \ \Rightarrow\ (1+\varepsilon_n)^\alpha=1+\alpha\varepsilon_n+o(\varepsilon_n)$$
$$\ldots$$

## Esempi di calcolo di limiti

**Esempio.** $a_n=\dfrac{\sin\frac{1}{n^2}}{e^{7/n}-1}\cdot n$

- $\varepsilon_n=\dfrac1{n^2}\to0$, $\ \sin\varepsilon_n\sim\varepsilon_n$, quindi $\sin\dfrac1{n^2}\sim\dfrac1{n^2}$
- $\varepsilon_n=\dfrac7n\to0$, $\ e^{\varepsilon_n}-1\sim\varepsilon_n$, quindi $e^{7/n}-1\sim\dfrac7n$

$$a_n\sim\dfrac{\frac1{n^2}}{\frac7n}\cdot n=\dfrac17 \quad\Rightarrow\quad \lim_{n\to\infty}a_n=\dfrac17$$

**Osservazione.** Una successione $\varepsilon_n\to0$ è una successione di punti $\varepsilon_0,\varepsilon_1,\varepsilon_2,\varepsilon_3,\ldots,\varepsilon_n,\ldots$ che si avvicinano all'asse delle $n$ (anche oscillando sopra e sotto l'asse).

**DISEGNO NON RAPPRESENTABILE** — Grafico di una successione $\varepsilon_n$ (in rosso) con punti $\varepsilon_0,\varepsilon_1,\varepsilon_2,\varepsilon_3,\ldots,\varepsilon_n$ sopra e sotto l'asse delle $n$ che tendono a $0$ (pagina 10 del PDF della Lezione 9).

**Esempio.**
$$a_n=\dfrac{\sqrt[3]{1+n}-n^{1/3}}{1-e^{2/n}}\cdot\arctan\dfrac1{n^2}\cdot n^{5/3}$$

- $\arctan\dfrac1{n^2}\sim\dfrac1{n^2}$, perché $\arctan\varepsilon_n\sim\varepsilon_n$ con $\varepsilon_n=\dfrac1{n^2}\to0$
- $1-e^{2/n}\sim-\dfrac2n$, perché $-(e^{\varepsilon_n}-1)\sim-\varepsilon_n$ con $\varepsilon_n=\dfrac2n\to0$
- $\sqrt[3]{1+n}-n^{1/3}\sim\ ?$

> [!danger] Attenzione — cosa NON si può fare
> - $\sqrt[3]{1+n}=(1+n)^{1/3}\neq 1+\dfrac n3+o(n)$, perché $\varepsilon_n=n\not\to0$
> - $\sqrt[3]{1+n}\sim n^{1/3}$ è vero, **ma non** si può concludere $\sqrt[3]{1+n}-n^{1/3}\sim n^{1/3}-n^{1/3}=0$: non si usa $\sim$ in somme e sottrazioni.

Si procede così:
$$\sqrt[3]{1+n}=n^{1/3}\left(1+\dfrac1n\right)^{1/3}\qquad\text{con } (1+\varepsilon_n)^\alpha,\ \varepsilon_n=\dfrac1n,\ \alpha=\dfrac13$$
$$=n^{1/3}\left(1+\dfrac{1}{3n}+o\!\left(\dfrac1n\right)\right)=n^{1/3}+\dfrac{1}{3n^{2/3}}+n^{1/3}\cdot o\!\left(\dfrac1n\right)$$
Infatti $\dfrac{n^{1/3}\cdot o(1/n)}{1/n^{2/3}}=\dfrac{o(1/n)}{1/n}\to0$, quindi $n^{1/3}\cdot o\!\left(\dfrac1n\right)=o\!\left(\dfrac1{n^{2/3}}\right)$. Allora
$$\sqrt[3]{1+n}-n^{1/3}=\cancel{n^{1/3}}+\dfrac{1}{3n^{2/3}}+o\!\left(\dfrac1{n^{2/3}}\right)-\cancel{n^{1/3}}=\dfrac{1}{3n^{2/3}}+o\!\left(\dfrac1{n^{2/3}}\right)\sim\dfrac{1}{3n^{2/3}}$$
$$a_n\sim\dfrac{\frac{1}{3n^{2/3}}}{-\frac2n}\cdot\dfrac1{n^2}\cdot n^{5/3}=-\dfrac16 \quad\Rightarrow\quad \lim_{n\to\infty}a_n=-\dfrac16$$

**Esempio.** $a_n=(n^3+n^2)^{1/3}-(n^3-n)^{1/3}$

Posto $a=\sqrt[3]{n^3+n^2}$, $b=\sqrt[3]{n^3-n}$, vale $a^3-b^3=(a-b)(a^2+ab+b^2)$, cioè $a-b=\dfrac{a^3-b^3}{a^2+ab+b^2}$ (…). Qui però si procede con gli sviluppi di $(1+\varepsilon_n)^\alpha=1+\alpha\varepsilon_n+o(\varepsilon_n)$:

$$(n^3+n^2)^{1/3}=n\left(1+\dfrac1n\right)^{1/3}=n\left(1+\dfrac1{3n}+o\!\left(\dfrac1n\right)\right)\ \sim\ n$$
$$(n^3-n)^{1/3}=n\left(1-\dfrac1{n^2}\right)^{1/3}=n\left(1-\dfrac1{3n^2}+o\!\left(\dfrac1{n^2}\right)\right)\ \sim\ n$$

$$a_n=n\left(1+\dfrac1{3n}+o\!\left(\dfrac1n\right)\right)-n\left(1-\dfrac1{3n^2}+o\!\left(\dfrac1{n^2}\right)\right)$$
$$=\cancel{n}+\dfrac13+n\,o\!\left(\dfrac1n\right)-\cancel{n}+\dfrac1{3n}-n\,o\!\left(\dfrac1{n^2}\right)$$
$$=\dfrac13+\dfrac1{3n}+n\,o\!\left(\dfrac1n\right)+n\,o\!\left(\dfrac1{n^2}\right)$$

Infatti $\dfrac{n\,o(1/n)}{1}=\dfrac{o(1/n)}{1/n}\to0$, quindi $n\,o\!\left(\dfrac1n\right)=o(1)$; analogamente $\dfrac{n\,o(1/n^2)}{1/n}=\dfrac{o(1/n^2)}{1/n^2}\to0$, quindi $n\,o\!\left(\dfrac1{n^2}\right)=o\!\left(\dfrac1n\right)$. Perciò
$$a_n=\dfrac13+\dfrac1{3n}+o(1)=\dfrac13+o(1)\ \longrightarrow\ \dfrac13$$

## Proprietà di $o$-piccolo

**Osservazioni.**
- $a_n\cdot o(b_n)=o(a_nb_n)$. Infatti $\dfrac{a_n\cdot o(b_n)}{a_nb_n}=\dfrac{o(b_n)}{b_n}\to0$ per definizione.
- $o(a_n)=a_n\cdot o(1)$
- $c\cdot o(a_n)=o(a_n)\quad\forall\,c\neq0$. Infatti $\dfrac{c\,o(a_n)}{a_n}\to c\cdot0=0$.
- $\pm\,o(a_n)=o(a_n)$
- $o\!\left(\dfrac1n\right)+o\!\left(\dfrac1{n^2}\right)=o\!\left(\dfrac1n\right)$
- $o(n)+o(n^2)=o(n^2)$
- Se $a_n\sim b_n$ $\Rightarrow$ $o(a_n)=o(b_n)$. Infatti
$$\dfrac{o(a_n)}{b_n}=\dfrac{o(a_n)}{a_n}\cdot\dfrac{a_n}{b_n}\to 0\cdot1=0$$
Ad esempio $o\!\left(\sin\dfrac1n\right)=o\!\left(\dfrac1n\right)$.

**Esempio.** $a_n=\dfrac{\sin\frac1n-\frac1n}{\frac1{n^3}}$ è una forma indeterminata $\left[\dfrac00\right]$.

Con $\varepsilon_n=\dfrac1n\to0$: $\sin\varepsilon_n\sim\varepsilon_n$, $\ \sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$, cioè
$$\sin\dfrac1n-\dfrac1n=\dfrac1n+o\!\left(\dfrac1n\right)-\dfrac1n=o\!\left(\dfrac1n\right)$$
$$\Rightarrow\quad a_n=\dfrac{o\!\left(\frac1n\right)}{\frac1{n^3}}=n^3\,o\!\left(\dfrac1n\right)=o(n^2)$$
$$\lim_{n\to\infty}a_n=\ ?$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[41_o_piccolo_e_Asintotico]] — definizioni di o-piccolo e asintotico, gerarchia in termini di o-piccolo
- [[40_Confronti_Asintotici]] — ordine di infinito
- [[36_Gerarchia_degli_Infiniti]]
- [[37_Algebra_Limiti_Infiniti]]
- [[39_Criterio_del_Rapporto]]
- [[34_Algebra_dei_Limiti]]
- [[43_Asintotici_con_Funzioni_Composte]]

#AM1/successioni-e-limiti/confronti-asintotici-proprieta-e-notevoli
