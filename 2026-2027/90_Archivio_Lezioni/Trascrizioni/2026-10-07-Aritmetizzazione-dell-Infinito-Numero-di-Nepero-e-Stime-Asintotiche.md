---
created: 2026-10-07
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
aliases: []
---
[[00_A1_Indice|⬅️ Torna all'Indice A1]]

# Aritmetizzazione dell'Infinito, Numero di Nepero e Stime Asintotiche

Strumenti operativi per il calcolo di limiti di successioni: rapporto di «polinomi generalizzati», **aritmetizzazione parziale di $\infty$**, **forme di indeterminazione**, potenze $a_n^{b_n}$, **numero di Nepero** $e$, **criterio del rapporto**, e infine il confronto tra infiniti/infinitesimi con la notazione di **o-piccolo** e **asintotico**. Si appoggia ai [[2026-10-02-Teoremi-sui-Limiti-di-Successioni|teoremi sui limiti]].

## 1. Rapporti di somme di potenze

**Esempio 1.**
$$a_n=\frac{3n^5-4n^3+\log n-8\arctan(n^2+1)-3}{2n^{16/3}+147\log n^{52}-\sin n}$$
Si raccoglie la potenza dominante a numeratore e a denominatore:
$$a_n=\frac{n^5\left(3-\frac4{n^2}+\frac{\log n}{n^5}-8\frac{\arctan(n^2+1)}{n^5}-\frac3{n^5}\right)}{n^{16/3}\left(2+147\cdot52\frac{\log n}{n^{16/3}}-\frac{\sin n}{n^{16/3}}\right)}=\frac1{n^{1/3}}\cdot\frac{3+\dots}{2+\dots}$$
dove tutti i termini «$\dots$» tendono a $0$ (per la [[2026-10-02-Teoremi-sui-Limiti-di-Successioni|gerarchia degli infiniti]] e perché $\arctan$ e $\sin$ sono limitate). Quindi
$$a_n\to0\cdot\frac{3+0}{2+0}=0\ \Rightarrow\ \lim a_n=0.$$

**Osservazione generale.** Sia $a_n=\dfrac{P(n)}{Q(n)}$ con $P,Q$ somme di potenze di $n$ e di funzioni limitate in $n$ (oppure «trascurabili» rispetto a potenze di $n$). Siano $p$ e $q$ le massime potenze (positive) di $n$ in $P$ e $Q$, con coefficienti $c_P$ e $c_Q$. Allora:

| Caso | $\displaystyle\lim\frac{P(n)}{Q(n)}$ |
|---|---|
| $p<q$ | $0$ |
| $p=q$ | $\ell=\dfrac{c_P}{c_Q}\in\mathbb{R}\setminus\{0\}$ |
| $p>q$ | $\pm\infty$ (segno dato dal prodotto dei segni di $c_P$ e $c_Q$) |

**Esempio 2** ($p=q$).
$$a_n=\frac{2n^5-47n^4+\log\log n+\cos n}{5n^5+\arctan\sqrt n+(\log n)^{42}-1}=1\cdot\frac{2+\dots}{5+\dots}\to\frac25.$$
Qui si usa $\dfrac{(\log n)^{42}}{n^5}=\left(\dfrac{\log n}{n^{5/42}}\right)^{42}\to0$.

**Esempio 3** ($p>q$).
$$\lim\frac{18n^3-n^{3/2}+\sin n+\log\log n}{-2n^2+n^{3/4}-(\log n)^{18}+7}=\lim n\cdot\frac{18+\dots}{-2+\dots}=+\infty\cdot(-9)=-\infty.$$

**Esempio 4** (gerarchia).
$$\lim\frac{7\cdot2^n+\log\log n-\arctan n+n^7}{14\,n!-n^{42}+\sin n}=\lim\frac{2^n}{n!}\cdot\frac{7+\dots}{14+\dots}=0\cdot\frac7{14}=0.$$

## 2. Aritmetizzazione parziale di $\infty$

> **Teorema.** Siano $a_n,b_n$ successioni.
> 1. Se $\lim a_n=a\in\mathbb{R}$ e $\lim b_n=\pm\infty$ $\Rightarrow$ $\lim(a_n+b_n)=\pm\infty$ (ovvero $a\pm\infty=\pm\infty$, $\forall a\in\mathbb{R}$).
> 2. Se $\lim a_n=\pm\infty$ e $\lim b_n=\pm\infty$ **concordi in segno** $\Rightarrow$ $\lim(a_n+b_n)=\pm\infty$ (stesso segno): $+\infty+\infty=+\infty$, $-\infty-\infty=-\infty$.
> 3. Se $\lim a_n=a\in\overline{\mathbb{R}}\setminus\{0\}$ e $\lim b_n=\pm\infty$ $\Rightarrow$ $\lim a_nb_n=\pm\infty$ con la **regola dei segni**: $+$ se $a>0$ e $\lim b_n=+\infty$, o $a<0$ e $\lim b_n=-\infty$; $-$ altrimenti. Cioè $\pm\infty\cdot a=\pm\infty$ con regola dei segni $\forall a\in\overline{\mathbb{R}}\setminus\{0\}$.
> 4. Se $\lim a_n=a\in\overline{\mathbb{R}}\setminus\{0\}$ e $\lim b_n=0^\pm$ ($b_n\neq0$ definitivamente) $\Rightarrow$ $\lim\dfrac{a_n}{b_n}=\pm\infty$ con la regola dei segni: $\dfrac a{0^\pm}=\pm\infty$.
> 5. Se $\lim a_n=a\in\mathbb{R}$ e $\lim b_n=\pm\infty$ $\Rightarrow$ $\lim\dfrac{a_n}{b_n}=0$ (ovvero $\dfrac a{\pm\infty}=0$ $\forall a\in\mathbb{R}$).

### Forme di indeterminazione
$$\infty-\infty,\qquad\infty\cdot0,\qquad\frac\infty\infty,\qquad\frac00$$
sono **forme di indeterminazione**: nulla si può dire in generale.

**Esempi per $[0\cdot\infty]$** (tutti con $b_n=\sqrt7\,n\to\infty$):

| $a_n$ | $a_nb_n$ | Limite |
|---|---|---|
| $\dfrac1n$ | $\sqrt7$ | $\sqrt7$ |
| $\dfrac1{n^2}$ | $\dfrac{\sqrt7}n$ | $0$ |
| $\dfrac1{\sqrt n}$ | $\sqrt7\sqrt n$ | $+\infty$ |
| $\dfrac{(-1)^n}n$ | $(-1)^n\sqrt7$ | non esiste |

## 3. Tecniche per forme indeterminate $\infty-\infty$

**Razionalizzazione.** $a_n=\sqrt{n^2+n}-\sqrt{n^2-n}$. Posti $a=\sqrt{n^2+n}$, $b=\sqrt{n^2-n}$, si usa $a-b=\dfrac{a^2-b^2}{a+b}$:
$$a_n=\frac{(n^2+n)-(n^2-n)}{\sqrt{n^2+n}+\sqrt{n^2-n}}=\frac{2n}{n\left(\sqrt{1+\frac1n}+\sqrt{1-\frac1n}\right)}\to\frac2{1+1}=1.$$

**Radice $m$-esima.** Per $\sqrt[7]{n^2+n}-\sqrt[7]{n^2-n}$ si usa la formula
$$a^m-b^m=(a-b)\sum_{k=0}^{m-1}a^{m-1-k}b^k.$$
(per $m=7$: $a^7-b^7=(a-b)(a^6+a^5b+a^4b^2+a^3b^3+a^2b^4+ab^5+b^6)$.) Lo stesso metodo si può applicare, ad esempio, a $a_n=(n^2+n)^{1/\sqrt2}-(n^2-n)^{1/\sqrt2}$, il cui limite viene lasciato come esercizio.

## 4. Potenze $a_n^{b_n}$

Per $a_n>0$: $a_n^{b_n}=e^{\log a_n^{b_n}}=e^{b_n\log a_n}$. Se $\lim a_n=a>0$ e $\lim b_n=b\in\mathbb{R}$ allora $\lim b_n\log a_n=b\log a\in\mathbb{R}$, quindi
$$\lim a_n^{b_n}=e^{b\log a}=e^{\log a^b}=a^b.$$

> **Teorema.** Siano $a_n,b_n$ con $\lim a_n=a\in\overline{\mathbb{R}}$, $a\ge0$ (con $a_n>0$ definitivamente), e $\lim b_n=b\in\overline{\mathbb{R}}$. Allora $\lim a_n^{b_n}=a^b$ (salvo forme indeterminate), dove:
> - $a^{+\infty}=+\infty$ e $a^{-\infty}=0$ $\forall a>1$ (anche $a=+\infty$);
> - $a^{+\infty}=0$ e $a^{-\infty}=+\infty$ $\forall a\in[0,1)$;
> - $(+\infty)^b=+\infty$ $\forall b>0$ (anche $b=+\infty$) e $(+\infty)^b=0$ $\forall b<0$ (anche $b=-\infty$).

**Osservazione.** $\infty^0$, $0^0$, $1^{\pm\infty}$ sono **esclusi**: sono forme di indeterminazione. Invece $a_n\equiv1$, $b_n=n$ dà $1^n\to1$ e $a_n\equiv0$, $b_n=n$ dà $0^n\to0$: questi **non** sono forme di indeterminazione.

**Esempio.** $\displaystyle\lim n^{1/n}=1$ (forma $\infty^0$). Si scrive $n^{1/n}=e^{\frac1n\log n}$ e $\frac1n\log n\to0$ per la gerarchia degli infiniti, quindi $n^{1/n}\to e^0=1$.

## 5. Numero di Nepero

> **Teorema.** La successione $a_n=\left(1+\dfrac1n\right)^n$, $n\ge1$, è **monotona crescente e limitata**. In particolare ammette limite in $\mathbb{R}$. *(Senza dimostrazione completa.)*

**Definizione.**
$$e=\lim_{n\to\infty}\left(1+\frac1n\right)^n=2{,}71828\dots$$

**Osservazioni.**
- $e=\sup_{n\ge1}\left(1+\frac1n\right)^n$ e $e>\left(1+\frac1n\right)^n\ \forall n\ge1$.
- *Idea della dimostrazione:* sfrutta la **disuguaglianza di Bernoulli** (cfr. [[2026-09-14-Insiemi-Numerici-Logica-e-Metodi-di-Dimostrazione|Bernoulli]]): si mostra $\dfrac{a_n}{a_{n-1}}\ge1$ $\forall n\ge2$, quindi $a_n\ge a_{n-1}$ e $a_n$ è crescente. Un'altra applicazione della disuguaglianza di Bernoulli mostra che $a_n$ è limitata.
- Vedremo che $e=\displaystyle\sum_{n=0}^\infty\frac1{n!}$.

> **Teorema.** Sia $c_n$ una successione con $\lim c_n=\pm\infty$. Allora
> $$\lim_{n\to\infty}\left(1+\frac1{c_n}\right)^{c_n}=e.$$

> **Corollario.** $\forall a\in\mathbb{R}$: $\displaystyle\lim_{n\to\infty}\left(1+\frac an\right)^n=e^a$.

**Dimostrazione.** Se $a\neq0$, per $n$ grande $1+\frac an>0$ e
$$\left(1+\frac an\right)^n=\left[\left(1+\frac an\right)^{n/a}\right]^a=\left[\left(1+\frac1{c_n}\right)^{c_n}\right]^a,\qquad c_n=\frac na\to\pm\infty,$$
che tende a $e^a$. Se $a=0$: $\left(1+\frac0n\right)^n=1\to1=e^0$. $\square$

## 6. Criterio del rapporto per successioni

> **Teorema (criterio del rapporto).** Sia $a_n>0$ definitivamente e supponiamo esista $\ell=\displaystyle\lim_{n\to\infty}\frac{a_{n+1}}{a_n}\in\overline{\mathbb{R}}$. Allora:
> - se $\ell>1$: $\lim a_n=+\infty$;
> - se $0\le\ell<1$: $\lim a_n=0$.

**Osservazione.** Se $\ell=1$ non si può concludere nulla su $\lim a_n$. *(Senza dimostrazione: è contenuta nella dimostrazione del criterio del rapporto per serie, che vedremo.)*

**Esempio 1.** $\lim\dfrac{a^n}{n!}=0$ per $a\ge0$ (ovvio se $a\in[0,1]$). Qui $a_n=\frac{a^n}{n!}$ e
$$\frac{a_{n+1}}{a_n}=\frac{a^{n+1}}{(n+1)!}\cdot\frac{n!}{a^n}=\frac a{n+1}\to0\in[0,1)\ \Rightarrow\ \lim\frac{a^n}{n!}=0.$$

**Esempio 2.** $\lim\dfrac{n^n}{n!}=+\infty$. Con $a_n=\frac{n^n}{n!}$:
$$\frac{a_{n+1}}{a_n}=\frac{(n+1)^{n+1}}{(n+1)!}\cdot\frac{n!}{n^n}=\left(\frac{n+1}n\right)^n=\left(1+\frac1n\right)^n\to e\in(1,\infty],$$
quindi $\lim\dfrac{n^n}{n!}=+\infty$, e di conseguenza $\lim\dfrac{n!}{n^n}=\lim\left(\dfrac{n^n}{n!}\right)^{-1}=0$.

### Gerarchia degli infiniti (riquadro riassuntivo)
$$(\log_an)^\beta\ \ll\ n^\alpha\ \ll\ a^n\ \ll\ n!\ \ll\ n^n\qquad\forall\beta>0,\ \forall\alpha>0,\ \forall a>1.$$

## 7. Confronti e stime asintotiche

### Ordini di infinito
**Definizione.** Siano $a_n,b_n$ **infinite** ($\lim a_n=\pm\infty$, $\lim b_n=\pm\infty$, non necessariamente con lo stesso segno). Se
$$\lim_{n\to\infty}\frac{a_n}{b_n}=\begin{cases}0&a_n\text{ è infinito di ordine inferiore rispetto a }b_n\\ \ell\in\mathbb{R}\setminus\{0\}&a_n,b_n\text{ sono infiniti dello stesso ordine}\\ \pm\infty&b_n\text{ è infinito di ordine inferiore rispetto a }a_n\\ \nexists&a_n,b_n\text{ non confrontabili}\end{cases}$$

**Esempi.**
- $(\log_an)^\beta$ è infinito di ordine inferiore rispetto a $n^\alpha,a^n,n!,n^n$ ($\forall a>1,\alpha>0,\beta>0$).
- $n!$ è infinito di ordine superiore rispetto a $n^\alpha,a^n,(\log_an)^\beta$.
- $\log n$ e $\log n^2$ sono infiniti dello stesso ordine: $\dfrac{\log n}{\log n^2}=\dfrac{\log n}{2\log n}=\dfrac12\to\dfrac12$.
- $(2+\sin n)\,n$ e $n$ sono **non confrontabili**.

### Ordini di infinitesimo
**Definizione.** Siano $a_n,b_n$ **infinitesime** ($\lim a_n=\lim b_n=0$, con $b_n\neq0$ definitivamente). Se
$$\lim_{n\to\infty}\frac{a_n}{b_n}=\begin{cases}0&a_n\text{ è infinitesimo di ordine superiore rispetto a }b_n\\ \ell\in\mathbb{R}\setminus\{0\}&\text{infinitesimi dello stesso ordine}\\ \pm\infty&b_n\text{ è infinitesimo di ordine superiore rispetto a }a_n\\ \nexists&\text{non confrontabili}\end{cases}$$

**Esempio.** $\dfrac1{n^n}$ è infinitesimo di ordine superiore rispetto a $\dfrac1{n^\alpha},\dfrac1{(\log_an)^\beta},\dfrac1{a^n},\dfrac1{n!}$ ($\forall\alpha>0,\beta>0,a>1$).

### o-piccolo e asintotico
**Definizione.** Date due successioni qualsiasi $a_n,b_n$ (con $b_n\neq0$ definitivamente):
- $a_n$ è **o-piccolo** di $b_n$, in simboli $a_n=o(b_n)$ per $n\to\infty$, se $\displaystyle\lim\frac{a_n}{b_n}=0$;
- $a_n$ è **asintotico** a $b_n$, in simboli $a_n\sim b_n$ per $n\to\infty$, se $\displaystyle\lim\frac{a_n}{b_n}=1$.

**Osservazioni.**
- Se $\lim\frac{a_n}{b_n}=\pm\infty$ allora $\lim\frac{b_n}{a_n}=0$, quindi $b_n=o(a_n)$.
- Se $\lim\frac{a_n}{b_n}=\ell\in\mathbb{R}\setminus\{0\}$ allora $\lim\frac{a_n}{\ell\,b_n}=1$, quindi $a_n\sim\ell\,b_n$.
- Gerarchia degli infiniti con o-piccolo ($\forall\alpha>0,\beta>0,a>1$):
$$(\log_an)^\beta=o(n^\alpha),\quad n^\alpha=o(a^n),\quad a^n=o(n!),\quad n!=o(n^n).$$

**Esempio.**
$$a_n=7n^{47}+\log n+\log\log n+(\log n)^{18}+\sin n+n^{18}-\arctan n^2=7n^{47}+o(n^{47})\ \sim\ 7n^{47}.$$
