---
tags:
  - AM1
  - funzioni
  - funzione-inversa
  - esempi
data: 2026-09-30
fonte: Lezione 6
---

# Funzioni inverse — richiami ed esempi

> [!info] Richiamo
> Se $f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$ è iniettiva, allora
> $$\exists\, f^{-1}: \operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R} \quad \text{con} \quad f^{-1}(y)=x \ \Longleftrightarrow\ y=f(x)$$
> $$x\in\mathcal{D}(f),\ y\in\operatorname{Im}f$$

**Osservazione.** Calcolare la regola analitica di calcolo di $f^{-1}(y)$, $\forall\, y\in\operatorname{Im}f$, vuol dire risolvere l'equazione
$$f(x)=y \qquad \forall\, x\in\mathcal{D}(f),\ y\in\operatorname{Im}f$$

**Esempio.** $f(x) = e^{x^3+2}$, $\operatorname{Im}f = (0,\infty)$

$$f(x)=y \quad \forall\, y>0$$
$$e^{x^3+2} = y$$
$$x^3+2 = \log y$$
$$x^3 = \log y - 2$$
$$x = \sqrt[3]{\log y - 2} = f^{-1}(y)$$

**Osservazione.** Il grafico di $f^{-1}$, $\mathcal{G}(f^{-1})$, si ottiene dal grafico di $f$, $\mathcal{G}(f)$, per simmetria rispetto alla retta $y=x$.

![[GraficoFunzioniInverse.png]]

Infatti
$$(a,b) \in \mathcal{G}(f) \ \Longleftrightarrow\ b=f(a),\ a\in\mathcal{D}(f),\ b\in\operatorname{Im}f$$
$$\Rightarrow \quad f^{-1}(b)=a,\ b\in\mathcal{D}(f^{-1}),\ a\in\operatorname{Im}f^{-1}$$
$$\Rightarrow \quad (b,a)\in\mathcal{G}(f^{-1})$$

cioè $(a,b)\in\mathcal{G}(f) \ \Longleftrightarrow\ (b,a)\in\mathcal{G}(f^{-1})$.

## Esempio — potenza $n$-esima

$f(x)=x^n$, $x\in\mathbb{R}$, $n\in\mathbb{N}$, $n\geq 1$, $f:\mathbb{R}\to\mathbb{R}$.

Se $n$ è pari, $f$ non è iniettiva né suriettiva.

Si consideri $g(x)=x^n$ ($n$ pari), $g:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$. $g$ è iniettiva (strettamente crescente), $\operatorname{Im}g = [0,\infty)$.

La sua inversa è $g^{-1}:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$, con $\operatorname{Im}g^{-1} = \mathcal{D}(g) = [0,\infty)$:
$$g^{-1}(y) = \sqrt[n]{y}$$
$x=\sqrt[n]{y}$ è l'unica soluzione di $x^n=g(x)=y$ con $x\geq 0$.

## Esempio — tangente

$f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$, $f(x)=\operatorname{tg}x$

$$\mathcal{D}(f) = \left\{x\in\mathbb{R} : x\neq \dfrac{\pi}{2}+k\pi,\ k\in\mathbb{Z}\right\}, \qquad \operatorname{Im}f=\mathbb{R}$$

$f$ non è iniettiva su tutto $\mathcal{D}(f)$.![[GraficoTgx.png]]

$x = \arctan y$, $y\in\mathbb{R}$, è l'unica soluzione di $\operatorname{tg}x=y$ tale che $x\in\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$.

Tutte le soluzioni sono date da $\arctan y + k\pi$, $k\in\mathbb{Z}$.

$h(y)=\arctan y$, $h:\mathbb{R}\to\mathbb{R}$, è l'inversa della restrizione di $f(x)=\operatorname{tg}x$ all'intervallo $\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$:
$$\mathcal{D}(h) = \mathbb{R}, \qquad \operatorname{Im}h = \left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$$



![[GraficoArctanx.png]]
## Esempio — seno

$f:\mathbb{R}\to\mathbb{R}$, $f(x)=\sin x$, $\operatorname{Im}f=[-1,1]$

$f$ non è iniettiva, né suriettiva.
![[GraficoSinx.png]]

$\forall\, y\in\operatorname{Im}f=[-1,1]$, $x=\arcsin y$ è l'unica soluzione di $\sin x=y$ tale che $x\in\left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right]$.

Tutte le soluzioni sono date, per ogni $k\in\mathbb{Z}$, da
$$\arcsin y + 2k\pi \qquad \text{oppure} \qquad \pi-\arcsin y+2k\pi$$
(per $y=\pm 1$ le due famiglie coincidono).

$h(y)=\arcsin y$, $h:[-1,1]\subseteq\mathbb{R}\to\mathbb{R}$:
$$\operatorname{Im}h = \left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right], \qquad \mathcal{D}(h)=[-1,1]$$
![[GraficoArcsinx.png]]
## Esempio — coseno

$f:\mathbb{R}\to\mathbb{R}$, $f(x)=\cos x$, $\operatorname{Im}f=[-1,1]$

$f$ non è iniettiva, né suriettiva.
![[GraficoCosx.png]]

$\forall\, y\in\operatorname{Im}f=[-1,1]$, $x=\arccos y$ è l'unica soluzione di $\cos x=y$ tale che $x\in[0,\pi]$.

Tutte le soluzioni sono date, per ogni $k\in\mathbb{Z}$, da
$$\arccos y + 2k\pi \qquad \text{oppure} \qquad -\arccos y+2k\pi$$
(per $y=\pm 1$ le due famiglie coincidono).

$h(y)=\arccos y$, $h:[-1,1]\subseteq\mathbb{R}\to\mathbb{R}$:
$$\operatorname{Im}h = [0,\pi], \qquad \mathcal{D}(h)=[-1,1]$$
![[GraficoArccosx.png]]
## Osservazione riassuntiva

- La restrizione di $f(x)=\operatorname{tg}x$ a $\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$ è strettamente crescente, quindi iniettiva.
- La restrizione di $f(x)=\sin x$ a $\left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right]$ è strettamente crescente, quindi iniettiva.
- La restrizione di $f(x)=\cos x$ a $[0,\pi]$ è strettamente decrescente, quindi iniettiva.

### Note collegate
- [[00_MOC_A1]]
- [[26_Iniettivita_Suriettivita_Inversa]] — definizioni di iniettività, suriettività e funzione inversa
- [[27_Teorema_Monotone_Invertibili]] — le funzioni strettamente monotone sono invertibili
- [[23_Monotonia]]
- [[24_Funzioni_Periodiche]] — periodicità di $\sin$, $\cos$, $\operatorname{tg}$
- [[12_Logaritmi]] — esempio con $\log$