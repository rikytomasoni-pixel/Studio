---
created: 2026-09-30
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/6
  - argomento/funzioni
aliases: []
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Funzioni Trigonometriche Inverse

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

Sono iniettive perché strettamente monotone (cfr. [[2026-09-25 A1 Lezione 5|teorema monotonia/invertibilità]]).

---
Precedente: [[Esempi di Funzioni Inverse]]
