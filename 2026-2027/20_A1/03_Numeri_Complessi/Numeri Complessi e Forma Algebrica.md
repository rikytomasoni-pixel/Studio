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

# Numeri Complessi e Forma Algebrica

L'equazione $x^2+1=0$ non ha soluzioni in $\mathbb{R}$, e in **nessun campo ordinato** $X$. Infatti in un campo ordinato
$$x^2\ge0\ \ \forall x\in X,\qquad 1>0 \;\Rightarrow\; x^2+1\ge1>0\;\Rightarrow\; x^2+1\neq 0\ \ \forall x\in X.$$

**Domanda:** si può costruire un campo che estenda $\mathbb{R}$ (necessariamente non ordinato) in cui $x^2+1=0$ ammetta soluzione? *Sì, e faremo di meglio.*

Si introduce l'**unità immaginaria** $i$, definita dalla proprietà
$$i^2=-1\qquad(i^2+1=0).$$

## 3. Forma algebrica

$$\mathbb{C}=\{z=a+ib:\ a,b\in\mathbb{R},\ i^2+1=0\}$$

$z=a+ib$ si dice **forma algebrica** del numero complesso $z$. Si definiscono:

- $a=\operatorname{Re}z$, **parte reale** di $z$;
- $b=\operatorname{Im}z$, **parte immaginaria** di $z$.

Entrambe sono numeri **reali**. Esempio: $z=4-7i\Rightarrow \operatorname{Re}z=4,\ \operatorname{Im}z=-7$.

### Operazioni
Per $z=a+ib$, $w=x+iy$ ($a,b,x,y\in\mathbb{R}$):
$$z+w=(a+x)+i(b+y)$$
$$z\cdot w=(ax-by)+i(bx+ay)$$

Le operazioni sono definite formalmente come somme e prodotti di **polinomi a coefficienti reali** (di grado al più 1) in $i$, con la regola aggiuntiva $i^2=-1$.

> **Teorema.** $\mathbb{C}$ con $+,\cdot$ è un [[2026-09-16 A1 Lezione 2|campo]].

- Elemento neutro della somma: $0=0+i0$. Elemento neutro del prodotto: $1=1+i0$.
- Opposto: se $z=a+ib$ allora $-z=-a-ib$.
- **Inverso**: se $z\neq0$ (cioè $a^2+b^2\neq0$),
$$z^{-1}=\frac1z=\frac{a}{a^2+b^2}-i\,\frac{b}{a^2+b^2}.$$

Verifica:
$$z\cdot z^{-1}=(a+ib)\left(\frac{a}{a^2+b^2}-i\frac{b}{a^2+b^2}\right)=\frac{a^2+b^2}{a^2+b^2}=1+i0=1.$$

**Esempio.** $z=3-4i\ \Rightarrow\ -z=-3+4i,\ \ \dfrac1z=\dfrac{3}{25}+\dfrac{4}{25}i$.

Si ha $\mathbb{R}\subset\mathbb{C}$ tramite l'identificazione $x\in\mathbb{R}\leftrightarrow z=x+i0\in\mathbb{C}$.

---
Successivo: [[Piano di Argand-Gauss]]
