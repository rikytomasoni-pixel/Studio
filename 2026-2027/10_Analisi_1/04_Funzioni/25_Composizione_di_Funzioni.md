---
tags:
  - AM1
  - funzioni
  - composizione
  - dominio
data: 2026-09-25
fonte: Lezione 5
---

# Composizione di funzioni

> [!info] Definizione
> Date due funzioni $f:A\to B$, $g:B\to C$

![[ComposizioneDiFunzioni.png]]

> si chiama $g\circ f: A\to C$ la funzione
> $$g\circ f(x) = g(f(x)) \qquad \forall\, x\in A$$

**Esempio.** $h(x)=\log(x^2+1)$, $x\in\mathbb{R}$
$$h(x) = g(f(x)) = g\circ f(x)$$
$$f(x)=x^2+1 \quad \forall\, x\in\mathbb{R}, \qquad g(t)=\log t \quad t\in(0,\infty)$$

**Osservazione.** Ovviamente si possono comporre 3 o più funzioni. Vale sempre $\forall\, h,g,f$:
$$(h\circ g)\circ f = h\circ(g\circ f)$$
In generale
$$f\circ g \neq g\circ f$$

**Esempio.** $f(x)=x+1$, $g(x)=x^2$, $x\in\mathbb{R}$
$$g\circ f(x) = (x+1)^2 = x^2+2x+1 \qquad \forall\, x\in\mathbb{R}$$
$$f\circ g(x) = x^2+1$$
$$f\circ g \neq g\circ f$$

**Osservazione.** Non tutte le funzioni possono essere composte.
$$g(t)=\log t, \qquad f(x)=-x^2$$
$$\Rightarrow \quad g\circ f(x) = \log(-x^2)$$
non è definita per alcun $x\in\mathbb{R}$.

## Dominio della composizione

**Osservazione.** Se $f:A\to B$, $g:D\subseteq B\to C$:

![[DominioFunzioneComposta.png]]

$$g\circ f : \mathcal{D} \subseteq A \longrightarrow C$$
$$g\circ f(x) = g(f(x)) \qquad \forall\, x\in\mathcal{D}$$
$$\mathcal{D} = \{x\in A : f(x)\in D\} \subseteq A$$

**Esempio.** $f(x)=1-x^2$, $g(t)=\log t$
$$g\circ f(x) = \log(1-x^2)$$
$$\mathcal{D} = \{x\in\mathbb{R} : 1-x^2>0\} = \{x\in\mathbb{R} : -1<x<1\}$$

**Esempio.** $f(x)=\sqrt{x}$, $g(t)=t^2$
$$g\circ f(x) = (\sqrt{x})^2 = x$$
$$\mathcal{D} = \{x\in[0,\infty) : \sqrt{x}\in\mathbb{R}\} = [0,\infty)$$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[19_Funzioni_Generalita]] — dominio, codominio
- [[21_Campo_di_Esistenza]] — dominio assegnato tramite espressione analitica
- [[26_Iniettivita_Suriettivita_Inversa]] — $f^{-1}(f(x))=x$, $f(f^{-1}(y))=y$
- [[12_Logaritmi]]
- [[11_Radici_e_Potenze]]

#AM1/funzioni/composizione-di-funzioni
