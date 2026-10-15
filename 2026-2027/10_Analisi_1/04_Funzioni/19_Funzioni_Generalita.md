---
tags:
  - AM1
  - funzioni
  - dominio
  - codominio
  - immagine
  - grafico
  - successioni
data: 2026-09-23
fonte: Lezione 4
---

# Generalità sulle funzioni

> [!info] Def
> Dati due insiemi $A,B$ una funzione $f:A\to B$ è una legge che associa a ciascun $x\in A$ uno e un solo elemento $y\in B$. Scriveremo
> $$y=f(x)$$
> $A$ si chiama **dominio** di $f$
> $B$ si chiama **codominio** di $f$
> Se $x\in A$, l'elemento $y=f(x)\in B$ si dice **immagine** di $x$ tramite la funzione.

**QUA DISEGNO**

> [!info] Def
> Si chiama **immagine di $A$ tramite $f$** (o immagine di $f$) l'insieme
> $$\operatorname{Im}f = f(A) = \{y\in B : \exists\, x\in A \text{ tale che } f(x)=y\} \subseteq B$$
> degli elementi di $B$ che "provengono" da qualche elemento di $A$ tramite $f$.

**Es:** $f:\mathbb{R}\to\mathbb{R}$, $f(x)=x^2$

l'immagine di $\pm2$ è $4$
il dominio di $f$ è $\mathbb{R}$
il codominio di $f$ è $\mathbb{R}$
$$\operatorname{Im}f = f(\mathbb{R}) = [0,\infty) \subsetneq \mathbb{R}$$

**Oss:** In generale $\operatorname{Im}f\subseteq B$, ma può essere $\operatorname{Im}f \subsetneq B$.

**Oss:**
$$f:\mathbb{R}\to\mathbb{R}, \quad f(x)=x^2$$
$$g:\mathbb{R}\to[0,\infty), \quad g(x)=x^2$$
$$h:[0,\infty)\to[0,\infty), \quad h(x)=x^2$$
$$u:[0,\infty)\to\mathbb{R}, \quad u(x)=x^2$$
Vengono pensate come funzioni diverse.

> [!info] Def
> Data $f:A\to B$, se $\operatorname{Im}f=B$ allora $f$ si dice **suriettiva**.

**Es:** per le funzioni precedenti $g$ e $h$ sono suriettive, $f$ e $u$ no.

**Oss:** Una funzione è assegnata dichiarando dominio $A$, codominio $B$ e la legge $y=f(x)\ \forall\, x\in A$.

**Oss:** A volte indicheremo il dominio di $f$ con $\mathcal{D}(f)=A$.

> [!info] Def
> Il **grafico** di una funzione $f:A\to B$ è il sottoinsieme di $A\times B$ definito da
> $$\mathcal{G}(f) = \{(x,y)\in A\times B : x\in A,\ y=f(x)\}$$
> $$= \{(x,f(x))\in A\times B : x\in A\}$$

**Oss:** Se $f:A\to B$ e $A,B\subseteq\mathbb{R}$ allora $\mathcal{G}(f)\subset\mathbb{R}^2$

![[GraficoDiFconIm.png]]
Il fatto che $\forall\, x_0\in A$ esiste un unico $y_0\in B$ immagine di $x_0$ tramite $f$ ($A,B\subseteq\mathbb{R}$) si interpreta geometricamente sul grafico di $f$ osservando che ogni retta verticale $x=x_0$ interseca il grafico di $f$ al più una volta: $0$ volte se $x_0\notin A$, $1$ volta se $x_0\in A$. In tal caso l'ordinata del punto sul grafico è $y_0=f(x_0)$.

$A=\mathcal{D}(f)$ è la proiezione sull'asse delle ascisse (in direzione parallela all'asse delle $y$) di $\mathcal{G}(f)$.

Inoltre $y_0\in\operatorname{Im}f$ se e solo se esiste un punto $(x_0,y_0)\in\mathcal{G}(f)$ di ordinata $y_0=f(x_0)$, cioè se e solo se la retta orizzontale $y=y_0$ interseca il grafico $\mathcal{G}(f)$ (in almeno un punto).

$\operatorname{Im}f$ è la proiezione di $\mathcal{G}(f)$ sull'asse delle ordinate, in direzione parallela all'asse $x$.

In questo corso ci occupiamo sostanzialmente di funzioni $f:A\subseteq\mathbb{R}\to\mathbb{R}$.

Quando il codominio di $f$ non è esplicitamente dichiarato, è sottinteso che esso sia $\mathbb{R}$.

## Successioni

> [!info] Def
> Una funzione $f:\mathbb{N}\subseteq\mathbb{R}\to\mathbb{R}$ si chiama **successione di numeri reali**.
>
> Più in generale si chiamano successioni di numeri reali le funzioni
> $$f: A\subseteq\mathbb{N}\subseteq\mathbb{R} \to \mathbb{R}$$
> con $A=\{n\in\mathbb{N}: n\geq n_0\}$ per qualche $n_0\in\mathbb{N}$.

**Es:**
$$f(n) = \dfrac{1}{n}, \quad n\geq 1$$
$$g(n) = \dfrac{1}{(n-42)^2}, \quad \forall\, n\geq 43$$
$$h(n) = \log(n-5), \quad \forall\, n\geq 6$$

**Oss:** Spesso si usa la notazione $a_n$, $\{a_n\}$, $\{a_n\}_{n\geq n_0}$ invece di usare $f(n)$, con $f:\mathbb{N}\to\mathbb{R}$.

### Note collegate
- [[00_MOC_Analisi_1]]
- 
- [[20_Funzioni_Limitate_Estremi]] — limitatezza, $\sup$, $\inf$ di una funzione
- [[21_Campo_di_Esistenza]] — dominio assegnato tramite espressione analitica
- [[23_Monotonia]]
- [[25_Composizione_di_Funzioni]]
- [[26_Iniettivita_Suriettivita_Inversa]] — suriettività, iniettività, inversa
- - [[29_Successioni_Definizioni_Base]] — ulteriori esempi e definizione di limitatezza
- [[01_Insiemi_Numerici]] — $\mathbb{N}$, $\mathbb{R}$

#AM1/funzioni/funzioni-generalita
