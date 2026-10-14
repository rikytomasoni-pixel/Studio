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

# Esempi di Funzioni Inverse

Se $f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$ è **iniettiva**, allora esiste $f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$ con
$$f^{-1}(y)=x\iff y=f(x),\qquad x\in\mathcal{D}(f),\ y\in\operatorname{Im}f.$$

**Osservazione.** Calcolare la regola analitica di $f^{-1}(y)$ per ogni $y\in\operatorname{Im}f$ significa **risolvere l'equazione** $f(x)=y$ in $x\in\mathcal{D}(f)$, $\forall y\in\operatorname{Im}f$.

**Esempio.** $f(x)=e^{x^3+2}$, $\operatorname{Im}f=(0,\infty)$. Per $y>0$:
$$e^{x^3+2}=y\ \Rightarrow\ x^3+2=\log y\ \Rightarrow\ x^3=\log y-2\ \Rightarrow\ x=\sqrt[3]{\log y-2}=f^{-1}(y).$$

### Grafico dell'inversa
Il grafico $\mathcal{G}(f^{-1})$ si ottiene da $\mathcal{G}(f)$ per **simmetria rispetto alla bisettrice $y=x$**.

![[grafico-inversa-simmetria-bisettrice.png]]

Infatti:
$$(a,b)\in\mathcal{G}(f)\iff b=f(a)\iff f^{-1}(b)=a\iff(b,a)\in\mathcal{G}(f^{-1}).$$

### Esempio: potenze $x^n$
$f:\mathbb{R}\to\mathbb{R}$, $f(x)=x^n$, $n\in\mathbb{N}$, $n\ge1$.

- Se $n$ è **pari**, $f$ non è né iniettiva né suriettiva.
- Se $n$ è **dispari**, $f$ è biettiva.

> **Figura (disegno senza immagine disponibile):**
>
> A sinistra ($n$ dispari): curva $f$ crescente su tutto $\mathbb{R}$ con punto di flesso nell'origine, ramo $x\ge0$ evidenziato in rosso ($g$). A destra ($n$ pari): parabola-like $f$ simmetrica rispetto all'asse $y$, con il solo ramo $x\ge0$ in rosso ($g$).

Si considera la restrizione $g(x)=x^n$, $g:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$: è **iniettiva** (strettamente crescente), $\operatorname{Im}g=[0,\infty)$. La sua inversa è
$$g^{-1}:[0,\infty)\to\mathbb{R},\qquad g^{-1}(y)=\sqrt[n]{y}=x,\qquad \operatorname{Im}g^{-1}=\mathcal{D}(g)=[0,\infty),$$
ed è l'unica soluzione di $x^n=y$ con $x\ge0$.

> **Figura (disegno senza immagine disponibile):**
>
> Curva rossa $g^{-1}$ che parte dall'origine, concava, crescente e con tangente verticale nell'origine.

---
Precedente: [[Monotonia e Invertibilità]] · Successivo: [[Funzioni Trigonometriche Inverse]]
