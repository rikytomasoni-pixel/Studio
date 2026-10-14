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

# Numeri Complessi e Forma Algebrica

## Perché non bastano i numeri reali

$$x^2+1=0$$
non ha soluzioni in $\mathbb{R}$, né in nessun campo ordinato $X$. Infatti, in un campo ordinato $X$ vale
$$x^2\geq 0 \ \ \forall\, x\in X \qquad \text{e} \qquad 1>0$$
$$\Rightarrow \quad x^2+1 \geq 1 > 0 \qquad \forall\, x\in X$$
$$\Rightarrow \quad x^2+1 \neq 0 \qquad \forall\, x\in X$$

**Domanda.** È possibile costruire un campo che estenda $\mathbb{R}$ (che sarà non ordinato) in cui $x^2+1=0$ ammetta soluzione?

> *(Sì, e faremo di meglio...)*

## Unità immaginaria e definizione di $\mathbb{C}$

Introduciamo l'**unità immaginaria**, che indichiamo con $i$, definita dalla proprietà
$$i^2 = -1 \qquad \left(i^2+1=0\right)$$

> [!warning] Definizione — Numeri complessi
> Definiamo $\mathbb{C}$ come segue:
> $$\mathbb{C} = \left\{ z=a+ib \ :\ a,b\in\mathbb{R},\ i^2+1=0 \right\}$$
> $z=a+ib$ si dice **forma algebrica** del numero complesso $z\in\mathbb{C}$.

> [!warning] Definizione — Parte reale e parte immaginaria
> Dato $z=a+ib\in\mathbb{C}$, $a,b\in\mathbb{R}$:
> $$a = \operatorname{Re} z \quad \text{parte reale di } z, \qquad b = \operatorname{Im} z \quad \text{parte immaginaria di } z$$

**Osservazione.** $\operatorname{Re} z, \operatorname{Im} z \in \mathbb{R}$.

**Esempio.** $z = 4-7i \ \Rightarrow\ \operatorname{Re} z = 4,\ \ \operatorname{Im} z = -7$.

## Somma e prodotto

$\forall\, z=a+ib\in\mathbb{C}$, $\forall\, w=x+iy\in\mathbb{C}$ (con $a,b,x,y\in\mathbb{R}$):
$$z+w = (a+x)+i(b+y)$$
$$z\cdot w = (ax-by)+i(bx+ay)$$

**Osservazione.** Le operazioni in $\mathbb{C}$, $+$ e $\cdot$, sono definite formalmente come somme e prodotti di polinomi a coefficienti reali (di grado al più $1$) in $i$, con in più la regola aggiuntiva $i^2=-1$.

## $\mathbb{C}$ è un campo

> [!abstract] Teorema
> $\mathbb{C}$ con $+,\cdot$ è un campo.
> - L'elemento neutro di $+$ è $0 = 0+i0$
> - L'elemento neutro di $\cdot$ è $1 = 1+i0$
> - Se $z=a+ib\in\mathbb{C}$ allora $-z = -a-ib$
> - Se $z\in\mathbb{C}$, $z\neq 0$ (cioè $a^2+b^2\neq 0$) allora
> $$z^{-1} = \dfrac{a}{a^2+b^2} - i\,\dfrac{b}{a^2+b^2}$$

**Verifica.**
$$z\cdot z^{-1} = (a+ib)\left(\dfrac{a}{a^2+b^2} - i\dfrac{b}{a^2+b^2}\right) = \dfrac{a^2}{a^2+b^2} + \dfrac{iba}{a^2+b^2} - \dfrac{iab}{a^2+b^2} + \dfrac{b^2}{a^2+b^2} = \dfrac{a^2+b^2}{a^2+b^2} = 1+i0 = 1$$

> *(Osservazione: $z\neq 0$ se $a^2+b^2\neq 0$)*

**Esempio.** $z = 3-4i$:
$$-z = -3+4i, \qquad \dfrac{1}{z} = \dfrac{3}{25}+\dfrac{4}{25}i$$

**Osservazione.** $\mathbb{R}\subset \mathbb{C}$:
$$x\in\mathbb{R} \quad \longleftrightarrow \quad z = x+i0 \in \mathbb{C}$$

---
Successivo: [[Piano di Argand-Gauss]]
