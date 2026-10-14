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

# Coniugato e Modulo

> [!warning] Definizione — Complesso coniugato
> Dato $z=x+iy\in\mathbb{C}$, chiamiamo
> $$\overline{z} = x-iy$$
> **complesso coniugato** di $z\in\mathbb{C}$.

> [!warning] Definizione — Modulo
> Indichiamo con
> $$|z| = \sqrt{x^2+y^2}$$
> il **modulo** di $z\in\mathbb{C}$.

**Osservazioni.**
- $|z|=0$ se e solo se $z=0$
- $|z|\geq 0 \ \ \forall\, z\in\mathbb{C}$

![[coniugato-e-modulo.png]]

- $\overline{z}$ è il simmetrico di $z$ rispetto all'asse reale
- $|z|$ è la distanza di $z\in\mathbb{C}$ da $0$ nel piano complesso (teorema di Pitagora), per ogni $z\in\mathbb{C}$
- Più in generale, $|z-w|$ è la distanza di $z\in\mathbb{C}$ da $w\in\mathbb{C}$ nel piano complesso: se $z=x+iy$, $w=a+ib$,
$$|z-w| = \sqrt{(x-a)^2+(y-b)^2}$$
- $z=\overline{z}$ se e solo se $z\in\mathbb{R}$ (cioè $\operatorname{Im} z = 0$)

## Luoghi geometrici notevoli

- $\operatorname{Re} z = \text{costante}$ → retta **verticale**
- $\operatorname{Im} z = \text{costante}$ → retta **orizzontale**
- $|z| = \text{costante} = \rho \geq 0$ → circonferenza centrata in $O$, di raggio $\rho$
![[luoghi-notevoli-piano-complesso.png]]

## Proprietà algebriche

$$z\cdot \overline{z} = (x+iy)(x-iy) = x^2+y^2 = |z|^2 \qquad \forall\, z\in\mathbb{C}$$
$$|z| = |\overline{z}| \qquad \forall\, z\in\mathbb{C}$$
$$z^{-1} = \dfrac{1}{z} = \dfrac{\overline{z}}{\overline{z}\, z} = \dfrac{\overline{z}}{|z|^2} = \dfrac{x-iy}{x^2+y^2} \qquad \forall\, z\in\mathbb{C}\setminus\{0\},\ \ z=x+iy$$
$$\overline{(w\cdot z)} = \overline{w}\cdot \overline{z} \qquad \forall\, z,w\in\mathbb{C}$$
$$\overline{(w+z)} = \overline{w}+\overline{z} \qquad \forall\, z,w\in\mathbb{C}$$
$$\dfrac{z}{w} = \dfrac{z}{w}\cdot\dfrac{\overline{w}}{\overline{w}} = \dfrac{z\cdot \overline{w}}{|w|^2} \qquad \forall\, z\in\mathbb{C},\ \forall\, w\in\mathbb{C}\setminus\{0\}$$

**Esempio.** $z=3-2i$, $w=1+7i$:
$$\dfrac{z}{w} = \dfrac{z\cdot \overline{w}}{|w|^2} = \dfrac{(3-2i)(1-7i)}{1+49} = \dfrac{-11-23i}{50} = -\dfrac{11}{50} - \dfrac{23}{50}i$$

---
Precedente: [[Piano di Argand-Gauss]] · Successivo: [[Equazioni in C]]
