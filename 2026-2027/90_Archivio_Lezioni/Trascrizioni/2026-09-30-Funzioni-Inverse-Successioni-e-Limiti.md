---
created: 2026-09-30
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
aliases: []
---
[[00_A1_Indice|⬅️ Torna all'Indice A1]]

# Funzioni Inverse, Successioni e Limite di Successione

Si completa il discorso sulla [[2026-09-25-Proprieta-delle-Funzioni-Composizione-e-Inversa|funzione inversa]] (calcolo, grafico, funzioni trigonometriche inverse) e si introduce la nozione di **limite di una successione**, con l'unicità del limite e il teorema sulle successioni monotone.

## 1. Funzioni inverse

Se $f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$ è **iniettiva**, allora esiste $f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$ con
$$f^{-1}(y)=x\iff y=f(x),\qquad x\in\mathcal{D}(f),\ y\in\operatorname{Im}f.$$

**Osservazione.** Calcolare la regola analitica di $f^{-1}(y)$ per ogni $y\in\operatorname{Im}f$ significa **risolvere l'equazione** $f(x)=y$ in $x\in\mathcal{D}(f)$, $\forall y\in\operatorname{Im}f$.

**Esempio.** $f(x)=e^{x^3+2}$, $\operatorname{Im}f=(0,\infty)$. Per $y>0$:
$$e^{x^3+2}=y\ \Rightarrow\ x^3+2=\log y\ \Rightarrow\ x^3=\log y-2\ \Rightarrow\ x=\sqrt[3]{\log y-2}=f^{-1}(y).$$

### Grafico dell'inversa
Il grafico $\mathcal{G}(f^{-1})$ si ottiene da $\mathcal{G}(f)$ per **simmetria rispetto alla bisettrice $y=x$**.

![[grafico-inversa-simmetria-bisettrice.png]]

Infatti:
$$(a,b)\in\mathcal{G}(f)\iff b=f(a)\iff f^{-1}(b)=a\iff(b,a)\in\mathcal{G}(f^{-1}).$$

### Esempio: potenze $x^n$
$f:\mathbb{R}\to\mathbb{R}$, $f(x)=x^n$, $n\in\mathbb{N}$, $n\ge1$.

- Se $n$ è **pari**, $f$ non è né iniettiva né suriettiva.
- Se $n$ è **dispari**, $f$ è biettiva.

> **Figura (disegno senza immagine disponibile):**
>
> A sinistra ($n$ dispari): curva $f$ crescente su tutto $\mathbb{R}$ con punto di flesso nell'origine, ramo $x\ge0$ evidenziato in rosso ($g$). A destra ($n$ pari): parabola-like $f$ simmetrica rispetto all'asse $y$, con il solo ramo $x\ge0$ in rosso ($g$).

Si considera la restrizione $g(x)=x^n$, $g:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$: è **iniettiva** (strettamente crescente), $\operatorname{Im}g=[0,\infty)$. La sua inversa è
$$g^{-1}:[0,\infty)\to\mathbb{R},\qquad g^{-1}(y)=\sqrt[n]{y}=x,\qquad \operatorname{Im}g^{-1}=\mathcal{D}(g)=[0,\infty),$$
ed è l'unica soluzione di $x^n=y$ con $x\ge0$.

> **Figura (disegno senza immagine disponibile):**
>
> Curva rossa $g^{-1}$ che parte dall'origine, concava, crescente e con tangente verticale nell'origine.

## 2. Funzioni trigonometriche inverse

### Arcotangente
$f(x)=\tan x$, $\mathcal{D}(f)=\{x\in\mathbb{R}:x\neq\frac\pi2+k\pi,\ k\in\mathbb{Z}\}$, $\operatorname{Im}f=\mathbb{R}$. È suriettiva ma **non iniettiva**.

![[grafico-tangente-con-restrizione.png]]

$x=\arctan y$, $y\in\mathbb{R}$, è l'**unica** soluzione di $\tan x=y$ con $x\in(-\frac\pi2,\frac\pi2)$. Tutte le soluzioni sono date da
$$\arctan y+k\pi,\qquad k\in\mathbb{Z}.$$
Quindi $h(y)=\arctan y$, $h:\mathbb{R}\to\mathbb{R}$, è l'inversa della **restrizione** di $\tan$ a $(-\frac\pi2,\frac\pi2)$, con $\mathcal{D}(h)=\mathbb{R}$, $\operatorname{Im}h=(-\frac\pi2,\frac\pi2)$.

![[grafico-arcotangente.png]]

### Arcoseno
$f(x)=\sin x$, $f:\mathbb{R}\to\mathbb{R}$, $\operatorname{Im}f=[-1,1]$: né iniettiva né suriettiva.

![[grafico-seno-con-restrizione.png]]

Per ogni $y\in[-1,1]$, $x=\arcsin y$ è l'**unica** soluzione di $\sin x=y$ con $x\in[-\frac\pi2,\frac\pi2]$. Tutte le soluzioni sono, $\forall k\in\mathbb{Z}$,
$$\arcsin y+2k\pi\qquad\text{e}\qquad(\pi-\arcsin y)+2k\pi.$$
*(Per $y=\pm1$ le due famiglie coincidono.)* Inversa della restrizione di $\sin$ a $[-\frac\pi2,\frac\pi2]$:
$$h(y)=\arcsin y,\quad h:[-1,1]\to\mathbb{R},\quad \operatorname{Im}h=\left[-\tfrac\pi2,\tfrac\pi2\right].$$

![[grafico-arcoseno.png]]

### Arcocoseno
$f(x)=\cos x$, $f:\mathbb{R}\to\mathbb{R}$, $\operatorname{Im}f=[-1,1]$: né iniettiva né suriettiva.

![[grafico-coseno-con-restrizione.png]]

Per ogni $y\in[-1,1]$, $x=\arccos y$ è l'**unica** soluzione di $\cos x=y$ con $x\in[0,\pi]$. Tutte le soluzioni sono, $\forall k\in\mathbb{Z}$,
$$\arccos y+2k\pi\qquad\text{e}\qquad-\arccos y+2k\pi.$$
*(Per $y=\pm1$ le due famiglie coincidono.)*
$$h(y)=\arccos y,\quad h:[-1,1]\to\mathbb{R},\quad\operatorname{Im}h=[0,\pi].$$

![[grafico-arcocoseno.png]]

### Restrizioni invertibili (riepilogo)

| Funzione | Restrizione | Monotonia | Inversa |
|---|---|---|---|
| $\tan x$ | $(-\frac\pi2,\frac\pi2)$ | strett. crescente | $\arctan$ |
| $\sin x$ | $[-\frac\pi2,\frac\pi2]$ | strett. crescente | $\arcsin$ |
| $\cos x$ | $[0,\pi]$ | strett. decrescente | $\arccos$ |

Sono iniettive perché strettamente monotone (cfr. [[2026-09-25-Proprieta-delle-Funzioni-Composizione-e-Inversa|teorema monotonia/invertibilità]]).

## 3. Successioni di numeri reali

**Definizione.** Una **successione** (di numeri reali) è una funzione
$$f:\{n\in\mathbb{N}:n\ge n_0\}\subseteq\mathbb{N}\ (\subseteq\mathbb{R})\to\mathbb{R}\quad\text{per qualche } n_0\in\mathbb{N}.$$

Esempi: $f(n)=\frac1n$ ($n\ge1$); $g(n)=\log(n-7)$ ($n\ge8$); $h(n)=n^2$ ($n\ge0$); $v(n)=\frac1{n^2-49}$ ($n\ge8$).

A livello di notazione si scrive $a_n,b_n,c_n,\dots$ invece di $f(n),g(n),h(n),\dots$.

**Grafico.** Il grafico di una successione è una **sequenza di punti** $(n,a_n)\in\mathbb{R}^2$:
$$\mathcal{G}(\{a_n\})=\{(n,a_n)\in\mathbb{R}^2:\ n\ge n_0,\ n\in\mathbb{N}\}.$$

![[grafico-successione-punti.png]]

**Esempio.** $a_n=\dfrac2{n+1}$: i valori $2,\,1,\,\tfrac23,\dots$ si avvicinano a $0$.

![[grafico-successione-2-su-n-piu-1.png]]

### Successioni limitate
Una successione si dice:
- **limitata dall'alto** se $\exists M\in\mathbb{R}$: $a_n\le M\ \ \forall n\in\mathbb{N}$;
- **limitata dal basso** se $\exists m\in\mathbb{R}$: $a_n\ge m\ \ \forall n\in\mathbb{N}$;
- **limitata** se lo è da entrambe: $m\le a_n\le M\ \forall n$. Equivalentemente, $\exists K>0$ tale che $|a_n|\le K\ \forall n\in\mathbb{N}$.

### «Definitivamente»
**Definizione.** Una successione soddisfa una proprietà $P$ **definitivamente** (in $n\in\mathbb{N}$) se $\exists N\in\mathbb{N}$ tale che $P$ è soddisfatta da $a_n$ per ogni $n\ge N$.

**Esempio.** $a_n=\frac1n$ è definitivamente minore di $\frac1\pi$: infatti $\frac1n<\frac1\pi\iff n>\pi\iff n\ge N=4$.

## 4. Limite di una successione

**Definizione (convergenza).** Una successione $a_n$ **converge** a $\ell\in\mathbb{R}$ e si scrive $\displaystyle\lim_{n\to\infty}a_n=\ell$ se
$$\forall\varepsilon>0\ \ \exists N\in\mathbb{N}\ \text{ tale che }\ \forall n\ge N:\quad|a_n-\ell|<\varepsilon\quad(\iff\ell-\varepsilon<a_n<\ell+\varepsilon).$$

![[definizione-limite-successione-striscia-epsilon.png]]

**Osservazione.**
$$\lim_{n\to\infty}a_n=\ell\iff\lim_{n\to\infty}|a_n-\ell|=0\iff\lim_{n\to\infty}(a_n-\ell)=0.$$

Non tutte le successioni ammettono limite in $\mathbb{R}$: $\lim n$ e $\lim(-1)^n$ **non esistono in $\mathbb{R}$**.

### Unicità del limite

> **Teorema (unicità del limite).** Data una successione $a_n$, se esiste $\displaystyle\lim_{n\to\infty}a_n=\ell\in\mathbb{R}$, allora esso è **unico**.

**Dimostrazione (per assurdo).** Supponiamo esistano $\ell_1\neq\ell_2$ in $\mathbb{R}$ tali che $\lim a_n=\ell_1$ e $\lim a_n=\ell_2$; per comodità $\ell_1>\ell_2$.

![[unicita-limite-intorni-disgiunti.png]]

Si sceglie
$$\varepsilon=\frac13|\ell_1-\ell_2|=\frac{\ell_1-\ell_2}3>0.$$
Allora $\ell_1-\varepsilon>\ell_2+\varepsilon$: infatti ciò equivale a $\ell_1-\ell_2>2\varepsilon=2\,\frac{\ell_1-\ell_2}3$, cioè $\frac13(\ell_1-\ell_2)>0$, vero. Quindi
$$(\ell_1-\varepsilon,\ell_1+\varepsilon)\cap(\ell_2-\varepsilon,\ell_2+\varepsilon)=\varnothing.$$
Per definizione di limite esistono $N_1,N_2$ tali che $a_n\in(\ell_1-\varepsilon,\ell_1+\varepsilon)$ per $n\ge N_1$ e $a_n\in(\ell_2-\varepsilon,\ell_2+\varepsilon)$ per $n\ge N_2$. Allora per ogni $n\ge N=\max\{N_1,N_2\}$ dovrebbe essere $a_n$ nell'intersezione, che è vuota. **Assurdo.** $\square$

### Esempio: $\lim\frac1n=0$
Fissato $\varepsilon>0$ si risolve $|a_n-0|<\varepsilon$, cioè $-\varepsilon<\frac1n<\varepsilon$. La disuguaglianza $\frac1n>-\varepsilon$ vale $\forall n\in\mathbb{N}$ (poiché $\frac1n>0>-\varepsilon$), mentre $\frac1n<\varepsilon\iff n>\frac1\varepsilon$. Quindi $\lim_{n\to\infty}\frac1n=0$ per definizione.

## 5. Limiti infiniti e regolarità

**Definizione (divergenza a $+\infty$).** $\displaystyle\lim_{n\to\infty}a_n=+\infty$ se $\forall M>0\ \exists N\in\mathbb{N}$ tale che $\forall n\ge N$: $a_n>M$.

![[divergenza-a-piu-infinito.png]]

**Definizione (divergenza a $-\infty$).** $\displaystyle\lim_{n\to\infty}a_n=-\infty$ se $\forall M>0\ \exists N\in\mathbb{N}$ tale che $\forall n\ge N$: $a_n<-M$.

![[divergenza-a-meno-infinito.png]]

**Esempio.** $a_n=\log\frac1n$: $\forall M>0$ si risolve $\log\frac1n<-M\iff\frac1n<e^{-M}\iff n>e^M$. Quindi $\lim\log\frac1n=-\infty$.

**Definizioni.**
- Se $\lim a_n=\ell\in\mathbb{R}$, $a_n$ **converge** a $\ell$.
- Se $\lim a_n=\pm\infty$, $a_n$ **diverge** a $\pm\infty$.
- In entrambi i casi $a_n$ è **regolare**.
- Se $a_n$ non converge né diverge ($\nexists\lim a_n$ in $\overline{\mathbb{R}}$), è **irregolare** (o **oscillante**, o **indeterminata**).
- $\overline{\mathbb{R}}=\mathbb{R}\cup\{+\infty\}\cup\{-\infty\}$ è l'insieme dei **reali estesi**.

**Esempi.**
- $a_n=(-1)^n$: irregolare **limitata**.
- $a_n=(-2)^n$: irregolare **illimitata**.
- $a_n=\begin{cases}2^n&n\text{ pari}\\1&n\text{ dispari}\end{cases}$: irregolare, illimitata dall'alto.

> **Teorema (unicità del limite in $\overline{\mathbb{R}}$).** Se esiste $\lim a_n=\ell\in\overline{\mathbb{R}}$, allora tale limite è unico. *(Senza dimostrazione.)*

**Definizione.** Se $\lim a_n=0$, $a_n$ è una successione **infinitesima**; se $\lim a_n=\pm\infty$, è una successione **infinita**.

### Convergenza per eccesso e per difetto
**Definizione.** $a_n$ converge a $\ell\in\mathbb{R}$ **per eccesso** (**per difetto**) se $\lim a_n=\ell$ e inoltre $a_n\ge\ell$ ($a_n\le\ell$) definitivamente. Si scrive
$$\lim_{n\to\infty}a_n=\ell^+\qquad(\lim a_n=\ell^-).$$

Formalmente:
- $\lim a_n=\ell^+$: $\forall\varepsilon>0\ \exists N:\ \forall n\ge N\ \ \ell\le a_n<\ell+\varepsilon$;
- $\lim a_n=\ell^-$: $\forall\varepsilon>0\ \exists N:\ \forall n\ge N\ \ \ell-\varepsilon<a_n\le\ell$.

![[convergenza-per-eccesso.png]]

**Esempi.**
- $\lim 2^{1/n}=1^+$
- $\lim\dfrac n{n+1}=1^-$
- $\lim\dfrac{(-1)^n}n=0$: né per eccesso né per difetto.

## 6. Successioni monotone

**Definizione.** Una successione $a_n$ è:

| Tipo | Condizione ($\forall n$) | Equivalente |
|---|---|---|
| **crescente** | $a_n\le a_{n+1}$ | $m\le n\Rightarrow a_m\le a_n$ |
| **decrescente** | $a_n\ge a_{n+1}$ | $m\le n\Rightarrow a_m\ge a_n$ |
| **strettamente crescente** | $a_n<a_{n+1}$ | $m<n\Rightarrow a_m<a_n$ |
| **strettamente decrescente** | $a_n>a_{n+1}$ | $m<n\Rightarrow a_m>a_n$ |

Esempi: $a_n=2^n$ cresce; $a_n=\frac1{2^n}$ decresce.

> **Teorema (limite di successioni monotone e limitate).** Sia $a_n$ una successione **monotona e limitata**. Allora $\exists\lim a_n=\ell\in\mathbb{R}$. Inoltre:
> - se $a_n$ è **crescente**: $\lim a_n=\ell^-$ con $\ell=\sup_n a_n\in\mathbb{R}$;
> - se $a_n$ è **decrescente**: $\lim a_n=\ell^+$ con $\ell=\inf_n a_n\in\mathbb{R}$.

**Osservazione.** Se $a_n$ è crescente, basta chiedere che sia limitata dall'alto (dal basso lo è automaticamente: $a_n\ge a_0$). Se è decrescente, basta chiedere che sia limitata dal basso.

**Dimostrazione** (solo il caso crescente e limitata; il decrescente è analogo). Sia $\ell=\sup_{n}a_n$. Esso esiste grazie all'**assioma dell'estremo superiore** che $\mathbb{R}$ soddisfa (e $\mathbb{Q}$ no, cfr. [[2026-09-16-Campi-Ordinati-Estremo-Superiore-e-Potenze|completezza]]); poiché $a_n$ è limitata dall'alto, $\ell\in\mathbb{R}$. Per definizione di estremo superiore:

1. $a_n\le\ell$ $\forall n$ ($\ell$ è maggiorante);
2. $\forall\varepsilon>0\ \exists n_0$ tale che $\ell-\varepsilon<a_{n_0}\le\ell$ ($\ell-\varepsilon$ non è maggiorante);
3. poiché $a_n$ è crescente, $\forall n\ge n_0$: $a_n\ge a_{n_0}$.

Dunque $\forall\varepsilon>0\ \exists n_0$ tale che $\forall n\ge n_0$:
$$\ell-\varepsilon<a_{n_0}\le a_n\le\ell,$$
cioè, per definizione, $\lim a_n=\ell^-$ con $\ell=\sup a_n$. $\square$

![[successione-crescente-limitata-sup.png]]

**Osservazione.** Questo teorema si appoggia sull'assioma dell'estremo superiore, che $\mathbb{R}$ soddisfa e $\mathbb{Q}$ no.

> **Teorema (limite delle successioni monotone, caso generale).** Sia $a_n$ una successione monotona. Allora ammette limite: $\exists\lim a_n=\ell\in\overline{\mathbb{R}}$.
> - Se $a_n$ cresce: $\lim a_n=\ell^-$ con $\ell=\sup_n a_n\in\mathbb{R}\cup\{+\infty\}$.
> - Se $a_n$ decresce: $\lim a_n=\ell^+$ con $\ell=\inf_n a_n\in\mathbb{R}\cup\{-\infty\}$.

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ **regolare**.
