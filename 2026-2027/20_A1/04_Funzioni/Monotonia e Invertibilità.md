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

# Monotonia e Invertibilità

> **Teorema.** Sia $f:A\subseteq\mathbb{R}\to\mathbb{R}$ **strettamente monotona** in $A$. Allora $f$ è **iniettiva**. Inoltre $f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$ è **strettamente monotona come $f$**.

**Dimostrazione.** Supponiamo $f$ strettamente crescente: $\forall x_1,x_2\in A$, $x_1<x_2\Rightarrow f(x_1)<f(x_2)$.

*Iniettività.* Se $x_1\neq x_2$, allora $x_1<x_2$ oppure $x_2<x_1$. Per monotonia stretta si ha $f(x_1)<f(x_2)$ oppure $f(x_2)<f(x_1)$; in ogni caso $f(x_1)\neq f(x_2)$. Quindi $f$ è iniettiva e $\exists f^{-1}:\operatorname{Im}f\to\mathbb{R}$.

*Monotonia dell'inversa* (per assurdo). Supponiamo che esistano $y_1,y_2\in\operatorname{Im}f=\mathcal{D}(f^{-1})$ con
$$y_1<y_2\quad\text{e}\quad f^{-1}(y_1)\ge f^{-1}(y_2).$$
Siano $x_1=f^{-1}(y_1)$, $x_2=f^{-1}(y_2)$, con $x_1,x_2\in\mathcal{D}(f)$. Poiché $x_1\ge x_2$ ed $f$ è crescente,
$$f(x_1)\ge f(x_2).\tag{$*$}$$
Ma $f(x_1)=f(f^{-1}(y_1))=y_1$ e $f(x_2)=y_2$: quindi $(*)$ significa $y_1\ge y_2$, assurdo perché per ipotesi $y_1<y_2$. Dunque $\forall y_1,y_2\in\operatorname{Im}f$, se $y_1<y_2$ allora $f^{-1}(y_1)<f^{-1}(y_2)$, cioè $f^{-1}$ è strettamente crescente. $\square$

### Controesempio al viceversa
Esistono funzioni **invertibili ma non monotone** (su un intervallo):
$$f(x)=\begin{cases}x & x\in[0,1)\\ 3-x & x\in[1,2]\end{cases},\qquad f:[0,2]\to\mathbb{R},\ \ \operatorname{Im}f=[0,2].$$
$f$ è invertibile e non monotona, con inversa $f^{-1}:[0,2]\to\mathbb{R}$
$$f^{-1}(y)=\begin{cases}y & y\in[0,1)\\ 3-y & y\in[1,2]\end{cases}.$$

![[funzione-invertibile-non-monotona.png]]

---
Precedente: [[Funzione Inversa]] · Successivo: [[Esempi di Funzioni Inverse]]
