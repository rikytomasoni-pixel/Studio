---
tags:
  - AM1
  - continuita
  - teorema-degli-zeri
  - bisezione
  - teorema
data: 2026-11-04
lezione: 15
fonte: "AM1 L15 26-27.pdf (pag. 21-25)"
---

# Teorema degli zeri

**Proprietà globali di funzioni continue o monotone su intervalli.**

> [!abstract] Teorema (degli zeri)
> Sia $f:[a,b]\to\mathbb{R}$, $a,b\in\mathbb{R}$, $f$ continua in $[a,b]$ e tale che $f(a)\cdot f(b)<0$ (cioè $f(a),f(b)$ discordi in segno). Allora $\exists x_0\in(a,b)$ tale che $f(x_0)=0$.
> Inoltre se $f$ è strettamente monotona esso è unico.

> [!note] Osservazioni
> - Questo teorema fornisce condizioni che garantiscono che l'equazione $f(x)=0$ abbia soluzione.
> - Garantisce che la soluzione $x_0$ è in $(a,b)$.
> - Fornisce un **algoritmo** che produce approssimazioni della soluzione $x_0$: $a_n$ cresce, $b_n$ decresce, $\displaystyle\lim_{n\to\infty}a_n=\lim_{n\to\infty}b_n=x_0$ (**algoritmo di bisezione**), e $\forall n\in\mathbb{N}$
> $$0\le x_0-a_n\le b_n-a_n=\frac{b-a}{2^n}\qquad0\le b_n-x_0\le b_n-a_n=\frac{b-a}{2^n}$$

## Dimostrazione
### Unicità (se $f$ strettamente monotona)
Mostriamo che se $f$ è strettamente monotona allora (se esiste) è unico il punto $x_0\in(a,b)$ tale che $f(x_0)=0$. Infatti se $f$ strettamente crescente
$$f(x)>f(x_0)=0\quad\forall x\in(x_0,b)\qquad f(x)<f(x_0)=0\quad\forall x\in(a,x_0)$$
Invece se $f$ strettamente decrescente le disuguaglianze sono invertite. In ogni caso $f(x)\neq f(x_0)=0$ $\forall x\in(a,b)$ con $x\neq x_0$. Quindi $x_0$ è l'unica soluzione di $f(x)=0$ in $(a,b)$.

### Esistenza (metodo di bisezione)
Mostriamo ora che nelle ipotesi del teorema esiste $x_0\in[a,b]$ tale che $f(x_0)=0$.

Poniamo $a_0=a$, $b_0=b$, $c_0=\dfrac{a_0+b_0}{2}$ punto medio del segmento $[a_0,b_0]$. Se $f(c_0)=0$ allora $x_0=c_0$ e abbiamo finito.

Se $f(c_0)\neq0$ allora o vale $f(c_0)f(a_0)<0$ o vale $f(c_0)f(b_0)<0$ (non entrambe) perché $f(a_0)$ e $f(b_0)$ sono discordi in segno.
- Se $f(a_0)\cdot f(c_0)<0$ poniamo $a_1=a_0$, $b_1=c_0$, $c_1=\frac{a_1+b_1}2$ punto medio di $[a_1,b_1]$.
- Se $f(c_0)\cdot f(b_0)<0$ poniamo $a_1=c_0$, $b_1=b_0$, $c_1=\frac{a_1+b_1}2$.

Ripetiamo il ragionamento con $[a_1,b_1]$, con $[a_2,b_2]$ e così via. L'algoritmo procede e si ferma se troviamo $c_n$ per qualche $n\in\mathbb{N}$ tale che $f(c_n)=0$: in tal caso $x_0=c_n$ e abbiamo concluso. Altrimenti l'algoritmo procede all'infinito e produce due successioni $a_n,b_n$ con le proprietà seguenti:

1. $a_n$ cresce, $b_n$ decresce
2. $a_n,b_n\in[a,b]\quad\forall n\in\mathbb{N}$
3. $0<b_n-a_n=\dfrac{b-a}{2^n}\quad\forall n\in\mathbb{N}$
4. $f(a_n)\cdot f(b_n)<0\quad\forall n\in\mathbb{N}$ e $c_n=\dfrac{a_n+b_n}2$ $\ \forall n\in\mathbb{N}$

Da (1) e (2) $a_n,b_n$ sono successioni monotone e limitate, quindi per il [[31_Successioni_Monotone|teorema di regolarità delle successioni monotone]]
$$\exists\ \bar a=\lim_{n\to\infty}a_n\in\mathbb{R},\qquad\bar b=\lim_{n\to\infty}b_n\in\mathbb{R}$$
Da (2), per [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni|permanenza del segno]], segue che $\bar a,\bar b\in[a,b]$. Da (3), per algebra dei limiti,
$$\bar b-\bar a=\lim_{n\to\infty}(b_n-a_n)=\lim_{n\to\infty}\frac{b-a}{2^n}=0\ \Rightarrow\ \bar b=\bar a$$
Chiamiamo $x_0=\bar b=\bar a\in[a,b]$. Per continuità di $f$
$$\lim_{n\to\infty}f(a_n)=f(x_0)=f(\bar a),\qquad\lim_{n\to\infty}f(b_n)=f(x_0)=f(\bar b)$$
Da (4), per permanenza del segno e algebra dei limiti,
$$0\ge\lim_{n\to\infty}f(b_n)\cdot f(a_n)=\big(f(x_0)\big)^2\ge0\ \Rightarrow\ \big(f(x_0)\big)^2=0\ \Rightarrow\ f(x_0)=0\qquad\square$$

> [!note] Osservazione (non presente negli appunti)
> La dimostrazione produce $x_0\in[a,b]$, mentre l'enunciato afferma $x_0\in(a,b)$: poiché $f(a)f(b)<0$ implica $f(a)\neq0$ e $f(b)\neq0$, lo zero non può essere un estremo, quindi $x_0\in(a,b)$.

## Note collegate
- [[113_Teorema_dei_Valori_Intermedi]] (si dimostra a partire da questo teorema)
- [[112_Teorema_di_Weierstrass]]
- [[116_Continuita_e_Invertibilita]]
- [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni]]
- [[31_Successioni_Monotone]]
- [[00_MOC_Analisi_1]]

#AM1/proprieta-globali/teorema-degli-zeri
