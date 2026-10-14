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

# Esempi di Funzioni Inverse

> [!info] Richiamo
> Se $f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$ è iniettiva, allora
> $$\exists\, f^{-1}: \operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R} \quad \text{con} \quad f^{-1}(y)=x \ \Longleftrightarrow\ y=f(x)$$
> $$x\in\mathcal{D}(f),\ y\in\operatorname{Im}f$$

**Osservazione.** Calcolare la regola analitica di calcolo di $f^{-1}(y)$, $\forall\, y\in\operatorname{Im}f$, vuol dire risolvere l'equazione
$$f(x)=y \qquad \forall\, x\in\mathcal{D}(f),\ y\in\operatorname{Im}f$$

**Esempio.** $f(x) = e^{x^3+2}$, $\operatorname{Im}f = (0,\infty)$

$$f(x)=y \quad \forall\, y>0$$
$$e^{x^3+2} = y$$
$$x^3+2 = \log y$$
$$x^3 = \log y - 2$$
$$x = \sqrt[3]{\log y - 2} = f^{-1}(y)$$

**Osservazione.** Il grafico di $f^{-1}$, $\mathcal{G}(f^{-1})$, si ottiene dal grafico di $f$, $\mathcal{G}(f)$, per simmetria rispetto alla retta $y=x$.

![[grafico-inversa-simmetria-bisettrice.png]]

Infatti
$$(a,b) \in \mathcal{G}(f) \ \Longleftrightarrow\ b=f(a),\ a\in\mathcal{D}(f),\ b\in\operatorname{Im}f$$
$$\Rightarrow \quad f^{-1}(b)=a,\ b\in\mathcal{D}(f^{-1}),\ a\in\operatorname{Im}f^{-1}$$
$$\Rightarrow \quad (b,a)\in\mathcal{G}(f^{-1})$$

cioè $(a,b)\in\mathcal{G}(f) \ \Longleftrightarrow\ (b,a)\in\mathcal{G}(f^{-1})$.

## Esempio — potenza $n$-esima

$f(x)=x^n$, $x\in\mathbb{R}$, $n\in\mathbb{N}$, $n\geq 1$, $f:\mathbb{R}\to\mathbb{R}$.

Se $n$ è pari, $f$ non è iniettiva né suriettiva.

Si consideri $g(x)=x^n$ ($n$ pari), $g:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$. $g$ è iniettiva (strettamente crescente), $\operatorname{Im}g = [0,\infty)$.

La sua inversa è $g^{-1}:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$, con $\operatorname{Im}g^{-1} = \mathcal{D}(g) = [0,\infty)$:
$$g^{-1}(y) = \sqrt[n]{y}$$
$x=\sqrt[n]{y}$ è l'unica soluzione di $x^n=g(x)=y$ con $x\geq 0$.

---
Precedente: [[Monotonia e Invertibilità]] · Successivo: [[Funzioni Trigonometriche Inverse]]
