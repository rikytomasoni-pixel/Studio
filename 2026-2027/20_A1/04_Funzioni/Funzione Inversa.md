---
created: 2026-09-25
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
origine: UpdateVault
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Funzione Inversa

> [!info] Definizione — Funzione inversa
> Data $f:A\to B$ **iniettiva**, la funzione che ad ogni $y\in\operatorname{Im}f$ associa l'unico $x\in A$ tale che $f(x)=y$ si chiama **inversa** di $f$ e si indica con
> $$f^{-1}: \operatorname{Im}f\subseteq B \longrightarrow A$$
> $$x=f^{-1}(y) \quad\Longleftrightarrow\quad f(x)=y, \qquad y\in\operatorname{Im}f \ \Longleftrightarrow\ x\in A$$

![[funzione-inversa-diagramma.png]]

**Osservazioni.**
- $\mathcal{D}(f^{-1}) = \operatorname{Im}f$, $\quad \operatorname{Im}f^{-1} = \mathcal{D}(f)$
- $f^{-1}(f(x)) = x \quad \forall\, x\in\mathcal{D}(f)$
- $f(f^{-1}(y)) = y \quad \forall\, y\in\operatorname{Im}f$

> [!info] Definizione — Invertibilità
> Se $f:A\to B$ è iniettiva, diremo che $f$ è **invertibile** (sulla sua immagine), cioè $\exists\, f^{-1}: \operatorname{Im}f\subseteq B\to A$.

## Esempi

**Esempio.** $f:\mathbb{R}\to\mathbb{R}$, $f(x)=x^2$: né iniettiva, né suriettiva.

**Esempio.** $h:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$, $h(x)=x^2$: $h$ è iniettiva, non suriettiva, $\operatorname{Im}h=[0,\infty)$.

![[parabola-ristretta-x-positivo.png]]

$\exists\, h^{-1}:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$ tale che $h(x)=y$ ammette un'unica soluzione $x\geq 0$, $\big(\mathcal{D}(h)=[0,\infty)\big)$, $\forall\, y\in\operatorname{Im}h=[0,\infty)$:
$$h^{-1}(y) = \sqrt{y} = x$$

**Osservazione.** Anche $g:(-\infty,0]\subseteq\mathbb{R}\to\mathbb{R}$, $g(x)=x^2$ è iniettiva, $\operatorname{Im}g=[0,\infty)$.

L'inversa è $g^{-1}:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$, dove $g^{-1}(y)$ è l'unica soluzione di $x^2=g(x)=y$ con $x\in\mathcal{D}(g)=(-\infty,0]$:
$$\Rightarrow \quad g^{-1}(y) = -\sqrt{y} \qquad \forall\, y\in\operatorname{Im}g=[0,\infty)$$

---
Precedente: [[Iniettività e Suriettività]] · Successivo: [[Monotonia e Invertibilità]]
