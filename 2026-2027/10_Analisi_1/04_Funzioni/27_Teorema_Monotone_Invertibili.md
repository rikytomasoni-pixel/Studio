---
tags:
  - AM1
  - funzioni
  - teorema
  - monotonia
  - funzione-inversa
data: 2026-09-25
fonte: Lezione 5
---

# Teorema: funzioni strettamente monotone sono invertibili

> [!abstract] Teorema
> $f:A\subseteq\mathbb{R}\to\mathbb{R}$ strettamente monotona in $A$. Allora $f$ è iniettiva. Inoltre $f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$ è strettamente monotona come $f$.

**dim:** Per fissare le idee supponiamo $f$ strettamente crescente, cioè $\forall\, x_1,x_2\in A$
$$x_1<x_2 \ \Rightarrow\ f(x_1)<f(x_2)$$

Vogliamo mostrare che $x_1\neq x_2 \ \Rightarrow\ f(x_1)\neq f(x_2)$, cioè $f$ iniettiva.

Infatti se $x_1\neq x_2$, allora $x_1<x_2$ o $x_2<x_1$. Per monotonia stretta:
$$x_1<x_2 \ \Rightarrow\ f(x_1)<f(x_2)$$
$$x_2<x_1 \ \Rightarrow\ f(x_2)<f(x_1)$$
In ogni caso $f(x_1)\neq f(x_2)$. Quindi $f$ iniettiva per definizione, pertanto $\exists\, f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$.

Mostriamo per assurdo che $f^{-1}$ deve essere monotona strettamente crescente come $f$.

Per assurdo, $\exists\, y_1,y_2\in\operatorname{Im}f=\mathcal{D}(f^{-1})$ tali che $y_1<y_2$ e $f^{-1}(y_1)\geq f^{-1}(y_2)$.

Siano $x_1=f^{-1}(y_1)$, $x_2=f^{-1}(y_2)$ con $x_1,x_2\in\mathcal{D}(f)=\operatorname{Im}f^{-1}$.

Poiché $x_1=f^{-1}(y_1)\geq f^{-1}(y_2)=x_2$, essendo $f$ crescente:
$$f(x_1)\geq f(x_2) \qquad (*)$$

Ma $f(x_1)=f(f^{-1}(y_1))=y_1$ e $f(x_2)=f(f^{-1}(y_2))=y_2$. Quindi $(*)$ vuol dire
$$y_1\geq y_2$$
Assurdo perché per ipotesi $y_1<y_2$.

$$\Rightarrow \quad \forall\, y_1,y_2\in\operatorname{Im}f: \quad \text{se } y_1<y_2 \text{ allora } f^{-1}(y_1)<f^{-1}(y_2)$$

cioè $f^{-1}$ strettamente crescente. $\blacksquare$

## Esempio — funzione invertibile ma non monotona

**Esempio.** Esistono funzioni invertibili ma non monotone (su un intervallo):

![[FunzioneInvertibileNonMonotona.png]]

$$f(x) = \begin{cases} x & x\in[0,1) \\ 3-x & x\in[1,2] \end{cases}$$

$f:[0,2]\subseteq\mathbb{R}\to\mathbb{R}$, $\operatorname{Im}f=[0,2]$

$f$ invertibile e **non** monotona, con inversa $f^{-1}:[0,2]\to\mathbb{R}$:
$$f^{-1}(y) = \begin{cases} y & y\in[0,1) \\ 3-y & y\in[1,2] \end{cases}$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[23_Monotonia]] — definizione di funzione monotona
- [[26_Iniettivita_Suriettivita_Inversa]] — iniettività e funzione inversa
- [[04_Dimostrazione_per_Assurdo]] — metodo di dimostrazione usato
- [[03_Dimostrazioni]]
- [[12_Logaritmi]] — applicazione: esistenza del logaritmo
- [[31_Successioni_Monotone]] — teorema analogo per successioni

#AM1/funzioni/teorema-monotone-invertibili
