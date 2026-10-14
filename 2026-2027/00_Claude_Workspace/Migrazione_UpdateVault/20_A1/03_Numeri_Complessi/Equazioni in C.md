---
created: 2026-09-18
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/numeri_complessi
aliases: []
origine: UpdateVault
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Equazioni in C

## Esempio di equazione con parte reale, parte immaginaria e coniugato

**Esempio.** Risolvere in $\mathbb{C}$:
$$z^2+2\operatorname{Re} z - i\operatorname{Im} z + \overline{z} = 0$$

Poniamo $z=x+iy\in\mathbb{C}$, $x,y\in\mathbb{R}$:
$$(x+iy)^2+2x-iy+x-iy = 0$$
$$x^2+2xyi-y^2+2x-iy+x-iy=0$$
$$\left(x^2-y^2+3x\right) + i\left(2xy-2y\right) = 0+i0$$

$$\begin{cases} x^2-y^2+3x=0 & \operatorname{Re}(\cdots)=\operatorname{Re} 0 = 0 \\[4pt] 2xy-2y=0 & \operatorname{Im}(\cdots)=\operatorname{Im} 0 = 0 \end{cases}$$

**Un'equazione in $\mathbb{C}$ in una variabile complessa $z\in\mathbb{C}$ equivale a un sistema di due equazioni nelle variabili reali $(x,y)\in\mathbb{R}^2$.**

Dalla seconda equazione: $2y(x-1)=0 \Rightarrow y=0$ oppure $x=1$.

$$\begin{cases} x=0 \\ y=0 \end{cases} \quad \lor \quad \begin{cases} x=-3 \\ y=0 \end{cases} \quad \lor \quad \begin{cases} y=2 \\ x=1 \end{cases} \quad \lor \quad \begin{cases} y=-2 \\ x=1 \end{cases}$$

$$\Rightarrow \quad z_0=0, \quad z_1=-3, \quad z_2=1+2i, \quad z_3=1-2i$$

**Osservazione.** In questo sistema $x,y\in\mathbb{R}$.

---
Precedente: [[Coniugato e Modulo]] · Successivo: [[Modulo e Argomento]]
