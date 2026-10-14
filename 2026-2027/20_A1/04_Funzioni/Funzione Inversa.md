---
created: 2026-09-25
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/5
  - argomento/funzioni
aliases: []
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Funzione Inversa

**Definizione.** Data $f:A\to B$ **iniettiva**, la funzione che a ogni $y\in\operatorname{Im}f$ associa l'unico $x\in A$ tale che $f(x)=y$ si chiama **inversa** di $f$ e si indica
$$f^{-1}:\operatorname{Im}f\subseteq B\to A,\qquad x=f^{-1}(y)\iff f(x)=y\quad(y\in\operatorname{Im}f,\ x\in A).$$

![[funzione-inversa-diagramma.png]]

**Osservazioni.**
- $\mathcal{D}(f^{-1})=\operatorname{Im}f$ e $\operatorname{Im}f^{-1}=\mathcal{D}(f)$.
- $f^{-1}(f(x))=x\ \ \forall x\in\mathcal{D}(f)$ e $f(f^{-1}(y))=y\ \ \forall y\in\operatorname{Im}f$.

**Definizione.** Se $f:A\to B$ è iniettiva diciamo che $f$ è **invertibile** (sulla sua immagine), cioè $\exists f^{-1}:\operatorname{Im}f\subseteq B\to A$.

### Esempi
- $f:\mathbb{R}\to\mathbb{R}$, $f(x)=x^2$: né iniettiva né suriettiva.
- $h:[0,\infty)\to\mathbb{R}$, $h(x)=x^2$: **iniettiva**, non suriettiva, $\operatorname{Im}h=[0,\infty)$. Esiste $h^{-1}:[0,\infty)\to\mathbb{R}$ perché $h(x)=y$ ha un'unica soluzione $x\ge0$ per ogni $y\in[0,\infty)$: $h^{-1}(y)=\sqrt y$.
- $g:(-\infty,0]\to\mathbb{R}$, $g(x)=x^2$: iniettiva, $\operatorname{Im}g=[0,\infty)$; l'inversa $g^{-1}:[0,\infty)\to\mathbb{R}$ è l'unica soluzione di $x^2=y$ con $x\le0$: $g^{-1}(y)=-\sqrt y$.

![[parabola-ristretta-x-positivo.png]]

---
Precedente: [[Iniettività e Suriettività]] · Successivo: [[Monotonia e Invertibilità]]
