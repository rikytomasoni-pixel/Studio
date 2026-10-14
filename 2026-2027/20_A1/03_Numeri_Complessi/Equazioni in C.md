---
created: 2026-09-18
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/numeri_complessi
aliases: []
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Equazioni in C

Un'equazione in una variabile complessa $z\in\mathbb{C}$ equivale a un **sistema di due equazioni** nelle variabili reali $(x,y)\in\mathbb{R}^2$ (uguagliando parte reale e parte immaginaria).

**Esempio.** $z^2+2\operatorname{Re}z-i\operatorname{Im}z+\bar z=0$, con $z=x+iy$:
$$(x+iy)^2+2x-iy+x-iy=0\ \Rightarrow\ (x^2-y^2+3x)+i(2xy-2y)=0+i0$$
$$\begin{cases}x^2-y^2+3x=0 & (\operatorname{Re})\\ 2xy-2y=0 & (\operatorname{Im})\end{cases}$$
La seconda dà $2y(x-1)=0$: o $y=0$ (e allora $x=0$ oppure $x=-3$), o $x=1$ (e allora $y=\pm2$). Soluzioni:
$$z_0=0,\quad z_1=-3,\quad z_2=1+2i,\quad z_3=1-2i.$$
In questo sistema $x,y\in\mathbb{R}$.

---
Precedente: [[Coniugato e Modulo]] · Successivo: [[Modulo e Argomento]]
