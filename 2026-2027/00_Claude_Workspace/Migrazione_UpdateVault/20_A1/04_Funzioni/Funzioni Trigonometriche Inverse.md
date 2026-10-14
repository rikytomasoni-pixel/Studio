---
created: 2026-09-30
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/funzioni
aliases: []
origine: UpdateVault
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Funzioni Trigonometriche Inverse

## Esempio — tangente

$f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$, $f(x)=\operatorname{tg}x$

$$\mathcal{D}(f) = \left\{x\in\mathbb{R} : x\neq \dfrac{\pi}{2}+k\pi,\ k\in\mathbb{Z}\right\}, \qquad \operatorname{Im}f=\mathbb{R}$$

$f$ non è iniettiva su tutto $\mathcal{D}(f)$.![[grafico-tangente-con-restrizione.png]]

$x = \arctan y$, $y\in\mathbb{R}$, è l'unica soluzione di $\operatorname{tg}x=y$ tale che $x\in\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$.

Tutte le soluzioni sono date da $\arctan y + k\pi$, $k\in\mathbb{Z}$.

$h(y)=\arctan y$, $h:\mathbb{R}\to\mathbb{R}$, è l'inversa della restrizione di $f(x)=\operatorname{tg}x$ all'intervallo $\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$:
$$\mathcal{D}(h) = \mathbb{R}, \qquad \operatorname{Im}h = \left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$$



![[grafico-arcotangente.png]]
## Esempio — seno

$f:\mathbb{R}\to\mathbb{R}$, $f(x)=\sin x$, $\operatorname{Im}f=[-1,1]$

$f$ non è iniettiva, né suriettiva.
![[grafico-seno-con-restrizione.png]]

$\forall\, y\in\operatorname{Im}f=[-1,1]$, $x=\arcsin y$ è l'unica soluzione di $\sin x=y$ tale che $x\in\left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right]$.

Tutte le soluzioni sono date, per ogni $k\in\mathbb{Z}$, da
$$\arcsin y + 2k\pi \qquad \text{oppure} \qquad \pi-\arcsin y+2k\pi$$
(per $y=\pm 1$ le due famiglie coincidono).

$h(y)=\arcsin y$, $h:[-1,1]\subseteq\mathbb{R}\to\mathbb{R}$:
$$\operatorname{Im}h = \left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right], \qquad \mathcal{D}(h)=[-1,1]$$
![[grafico-arcoseno.png]]
## Esempio — coseno

$f:\mathbb{R}\to\mathbb{R}$, $f(x)=\cos x$, $\operatorname{Im}f=[-1,1]$

$f$ non è iniettiva, né suriettiva.
![[grafico-coseno-con-restrizione.png]]

$\forall\, y\in\operatorname{Im}f=[-1,1]$, $x=\arccos y$ è l'unica soluzione di $\cos x=y$ tale che $x\in[0,\pi]$.

Tutte le soluzioni sono date, per ogni $k\in\mathbb{Z}$, da
$$\arccos y + 2k\pi \qquad \text{oppure} \qquad -\arccos y+2k\pi$$
(per $y=\pm 1$ le due famiglie coincidono).

$h(y)=\arccos y$, $h:[-1,1]\subseteq\mathbb{R}\to\mathbb{R}$:
$$\operatorname{Im}h = [0,\pi], \qquad \mathcal{D}(h)=[-1,1]$$
![[grafico-arcocoseno.png]]
## Osservazione riassuntiva

- La restrizione di $f(x)=\operatorname{tg}x$ a $\left(-\dfrac{\pi}{2},\dfrac{\pi}{2}\right)$ è strettamente crescente, quindi iniettiva.
- La restrizione di $f(x)=\sin x$ a $\left[-\dfrac{\pi}{2},\dfrac{\pi}{2}\right]$ è strettamente crescente, quindi iniettiva.
- La restrizione di $f(x)=\cos x$ a $[0,\pi]$ è strettamente decrescente, quindi iniettiva.

---
Precedente: [[Esempi di Funzioni Inverse]]
