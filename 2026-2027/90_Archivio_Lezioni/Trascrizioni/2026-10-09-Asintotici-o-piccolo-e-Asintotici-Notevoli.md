---
created: 2026-10-09
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
aliases: []
---
[[00_A1_Indice|⬅️ Torna all'Indice A1]]

# Asintotici, o-piccolo e Asintotici Notevoli

Formalizzazione di **asintotico** ($\sim$) e **o-piccolo** ($o$) per successioni, con le regole di calcolo e la tabella degli **asintotici notevoli**, applicati al calcolo di limiti. Continua il discorso sui [[2026-10-07-Aritmetizzazione-dell-Infinito-Numero-di-Nepero-e-Stime-Asintotiche|confronti e stime asintotiche]].

## 1. Definizioni

Date $a_n,b_n$ successioni ($b_n\neq0$ definitivamente in $n\in\mathbb{N}$):

- se $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=0$ scriviamo $a_n=o(b_n)$ ("**$a_n$ è o-piccolo di $b_n$**");
- se $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=1$ scriviamo $a_n\sim b_n$ ("**$a_n$ è asintotico a $b_n$**").

### Caratterizzazione
$$a_n\sim b_n\iff a_n=b_n+o(b_n).$$

Infatti
$$a_n\sim b_n\iff\lim\frac{a_n}{b_n}=1\iff\lim\left(\frac{a_n}{b_n}-1\right)=0\iff\lim\frac{a_n-b_n}{b_n}=0\iff a_n-b_n=o(b_n)\iff a_n=b_n+o(b_n).$$

**Osservazione.** $b_n=o(1)$ per definizione: $\lim\frac{b_n}1=0$, cioè $\lim b_n=0$, cioè $b_n$ è **infinitesima**.

## 2. $\sim$ è una relazione di equivalenza

Sulle successioni (definitivamente $\neq0$):
- **riflessiva**: $a_n\sim a_n$ (ovvio);
- **transitiva**: $a_n\sim b_n$ e $b_n\sim c_n\Rightarrow a_n\sim c_n$. Infatti $\dfrac{a_n}{c_n}=\dfrac{a_n}{b_n}\cdot\dfrac{b_n}{c_n}\to1\cdot1=1$;
- **simmetrica**: $a_n\sim b_n\Rightarrow b_n\sim a_n$. Infatti $\dfrac{b_n}{a_n}=\left(\dfrac{a_n}{b_n}\right)^{-1}\to1^{-1}=1$.

## 3. Asintotici notevoli

Se $\varepsilon_n\to0$ ($\varepsilon_n\neq0$ definitivamente), per $n\to\infty$ valgono:

| Asintotico | Sviluppo con o-piccolo |
|---|---|
| $\sin\varepsilon_n\sim\varepsilon_n$ | $\sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$ |
| $1-\cos\varepsilon_n\sim\dfrac{\varepsilon_n^2}2$ | $\cos\varepsilon_n=1-\dfrac{\varepsilon_n^2}2+o(\varepsilon_n^2)$ |
| $e^{\varepsilon_n}-1\sim\varepsilon_n$ | $e^{\varepsilon_n}=1+\varepsilon_n+o(\varepsilon_n)$ |
| $\log(1+\varepsilon_n)\sim\varepsilon_n$ | $\log(1+\varepsilon_n)=\varepsilon_n+o(\varepsilon_n)$ |
| $(1+\varepsilon_n)^\alpha-1\sim\alpha\varepsilon_n\ \ (\alpha\neq0)$ | $(1+\varepsilon_n)^\alpha=1+\alpha\varepsilon_n+o(\varepsilon_n)$ |
| $\arctan\varepsilon_n\sim\varepsilon_n$ | $\arctan\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$ |

Casi particolari con $\varepsilon_n=\frac1n$:
$$\sin\frac1n\sim\frac1n,\quad e^{1/n}-1\sim\frac1n,\quad\log\left(1+\frac1n\right)\sim\frac1n,\quad1-\cos\frac1n\sim\frac1{2n^2},\quad\left(1+\frac1n\right)^\alpha-1\sim\frac\alpha n,\quad\arctan\frac1n\sim\frac1n.$$
*(Il foglio degli asintotici notevoli è disponibile su WeBeep.)*

> **Figura (disegno senza immagine disponibile):**
>
> Grafico di una successione infinitesima $\varepsilon_n$: punti rossi $\varepsilon_0,\varepsilon_1,\varepsilon_2,\varepsilon_3,\dots,\varepsilon_n$ che oscillano sopra e sotto l'asse orizzontale, con ampiezza decrescente verso $0$ al crescere di $n$; sull'asse sono segnati $0,1,2,3,\dots,n$.

## 4. Proprietà del calcolo asintotico

> **Proposizione.** Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora:
> 1. $a_nb_n\sim a_n'b_n'$;
> 2. $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$;
> 3. $a_n^\alpha\sim(a_n')^\alpha$ per $\alpha\in\mathbb{R}$ (assumendo che l'operazione abbia senso);
> 4. se $a_n\sim a_n'$ allora le due successioni hanno **lo stesso carattere**: o convergono entrambe allo stesso limite $\ell\in\mathbb{R}$, o divergono entrambe a $+\infty$, o entrambe a $-\infty$, o sono entrambe indeterminate.

**Dimostrazione.**
1. $\dfrac{a_n'b_n'}{a_nb_n}=\dfrac{a_n'}{a_n}\cdot\dfrac{b_n'}{b_n}\to1\cdot1=1$.
2. $\dfrac{a_n/b_n}{a_n'/b_n'}=\dfrac{a_n}{a_n'}\cdot\left(\dfrac{b_n}{b_n'}\right)^{-1}\to1\cdot1^{-1}=1$.
3. $\dfrac{a_n^\alpha}{(a_n')^\alpha}=\left(\dfrac{a_n}{a_n'}\right)^\alpha\to1^\alpha=1$.
4. Se $\exists\lim a_n'=\ell\in\overline{\mathbb{R}}$, allora $a_n=\dfrac{a_n}{a_n'}\cdot a_n'\to1\cdot\ell=\ell$. Se invece $a_n'$ non ammette limite in $\overline{\mathbb{R}}$ e per assurdo $\exists\lim a_n=\ell\in\overline{\mathbb{R}}$, allora $a_n'=\dfrac{a_n'}{a_n}\cdot a_n\to1\cdot\ell=\ell$: **assurdo**. $\square$

> [!warning] Attenzione: cosa NON vale
> In generale, $a_n\sim a_n'$ e $b_n\sim b_n'$ **non** implicano
> - $a_n\pm b_n\sim a_n'\pm b_n'$ (somme e sottrazioni),
> - $a_n^{b_n}\sim(a_n')^{b_n'}$,
> - $e^{a_n}\sim e^{a_n'}$,
> - $\log(a_n)\sim\log(a_n')$.
>
> Inoltre, in generale:
> - $a_n\sim b_n\not\Rightarrow a_n-b_n\to0$;
> - $a_n-b_n\to0\not\Rightarrow a_n\sim b_n$.

## 5. Esempi

### Esempio 1: rapporto di «polinomi generalizzati»
$$a_n=\frac{3n^7+5n^{42/95}+\log n-\cos n+5}{2n^6-18n^3+\arctan n+(\log n)^2-2}.$$
Numeratore $N=3n^7+o(n^7)\sim3n^7$ e denominatore $D=2n^6+o(n^6)\sim2n^6$. Quindi
$$a_n=\frac{3n^7+o(n^7)}{2n^6+o(n^6)}\sim\frac{3n^7}{2n^6}=\frac32n\to+\infty\ \Rightarrow\ \lim a_n=+\infty.$$

### Esempio 2
$$a_n=\frac{\sin\frac1{n^2}}{e^{7/n}-1}\cdot n.$$
- $\varepsilon_n=\frac1{n^2}\to0$: $\sin\frac1{n^2}\sim\frac1{n^2}$;
- $\varepsilon_n=\frac7n\to0$: $e^{7/n}-1\sim\frac7n$.

$$a_n\sim\frac{\frac1{n^2}}{\frac7n}\cdot n=\frac17\ \Rightarrow\ \lim a_n=\frac17.$$

### Esempio 3
$$a_n=\frac{\sqrt[3]{1+n}-n^{1/3}}{1-e^{2/n}}\cdot\arctan\frac1{n^2}\cdot n^{5/3}.$$
- $\arctan\frac1{n^2}\sim\frac1{n^2}$ (con $\varepsilon_n=\frac1{n^2}\to0$);
- $1-e^{2/n}\sim-\frac2n$, perché $-(e^{\varepsilon_n}-1)\sim-\varepsilon_n$ con $\varepsilon_n=\frac2n\to0$;
- $\sqrt[3]{1+n}-n^{1/3}\sim\,?$

> [!warning] Errori da evitare
> - $\sqrt[3]{1+n}=(1+n)^{1/3}\neq1+\frac n3+o(n)$, perché $\varepsilon_n=n\not\to0$.
> - $\sqrt[3]{1+n}\sim n^{1/3}$ è vero, **ma** $\sqrt[3]{1+n}-n^{1/3}\not\sim n^{1/3}-n^{1/3}=0$: **non si usa $\sim$ nelle somme e sottrazioni**.

Si raccoglie $n$ in modo da avere $(1+\varepsilon_n)^\alpha$ con $\varepsilon_n=\frac1n$ e $\alpha=\frac13$:
$$\sqrt[3]{1+n}=n^{1/3}\left(1+\frac1n\right)^{1/3}=n^{1/3}\left(1+\frac1{3n}+o\!\left(\frac1n\right)\right)=n^{1/3}+\frac1{3n^{2/3}}+o\!\left(\frac1{n^{2/3}}\right).$$
Infatti $\dfrac{n^{1/3}\,o(1/n)}{1/n^{2/3}}=\dfrac{o(1/n)}{1/n}\to0$. Quindi
$$\sqrt[3]{1+n}-n^{1/3}=\frac1{3n^{2/3}}+o\!\left(\frac1{n^{2/3}}\right)\sim\frac1{3n^{2/3}}.$$
Mettendo tutto insieme:
$$a_n\sim\frac{\frac1{3n^{2/3}}}{-\frac2n}\cdot\frac1{n^2}\cdot n^{5/3}=-\frac16.$$

### Esempio 4
$$a_n=(n^3+n^2)^{1/3}-(n^3-n)^{1/3}.$$
Si potrebbe usare $a^3-b^3=(a-b)(a^2+ab+b^2)$; qui si usa invece lo sviluppo:
$$(n^3+n^2)^{1/3}=n\left(1+\frac1n\right)^{1/3}=n\left(1+\frac1{3n}+o\!\left(\frac1n\right)\right),$$
$$(n^3-n)^{1/3}=n\left(1-\frac1{n^2}\right)^{1/3}=n\left(1-\frac1{3n^2}+o\!\left(\frac1{n^2}\right)\right).$$
Quindi
$$a_n=n+\frac13+n\,o\!\left(\frac1n\right)-n+\frac1{3n}+n\,o\!\left(\frac1{n^2}\right)=\frac13+\frac1{3n}+o(1)=\frac13+o(1)\to\frac13.$$
(Infatti $\dfrac{n\,o(1/n)}{1}=\dfrac{o(1/n)}{1/n}\to0$ e $\dfrac{n\,o(1/n^2)}{1/n}=\dfrac{o(1/n^2)}{1/n^2}\to0$.)

## 6. Regole del calcolo con o-piccolo

- $a_n\cdot o(b_n)=o(a_nb_n)$. Infatti $\dfrac{a_n\,o(b_n)}{a_nb_n}=\dfrac{o(b_n)}{b_n}\to0$.
- $o(a_n)=a_n\cdot o(1)$.
- $c\cdot o(a_n)=o(a_n)$ per ogni costante $c\neq0$: $\dfrac{c\,o(a_n)}{a_n}\to c\cdot0=0$.
- $\pm\,o(a_n)=o(a_n)$.
- $o\!\left(\frac1n\right)+o\!\left(\frac1{n^2}\right)=o\!\left(\frac1n\right)$ e $o(n)+o(n^2)=o(n^2)$ (vince l'ordine «più grande»).
- Se $a_n\sim b_n$ allora $o(a_n)=o(b_n)$. Infatti $\dfrac{o(a_n)}{b_n}=\dfrac{o(a_n)}{a_n}\cdot\dfrac{a_n}{b_n}\to0\cdot1=0$. Ad esempio $o\!\left(\sin\frac1n\right)=o\!\left(\frac1n\right)$.

### Esempio da completare (forma $\frac00$)
$$a_n=\frac{\sin\frac1n-\frac1n}{\frac1{n^3}}.$$
Poiché $\sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$ con $\varepsilon_n=\frac1n$:
$$\sin\frac1n-\frac1n=\frac1n+o\!\left(\frac1n\right)-\frac1n=o\!\left(\frac1n\right)\ \Rightarrow\ a_n=\frac{o(1/n)}{1/n^3}=n^3\,o\!\left(\frac1n\right)=o(n^2).$$
Con questo livello di approssimazione **non si riesce a concludere** quanto vale $\lim a_n$: la stima $o(n^2)$ è troppo debole. *(L'esempio nel quaderno termina con «$\lim a_n=\,?$»: servirebbe uno sviluppo di $\sin\varepsilon_n$ a un ordine successivo.)*
