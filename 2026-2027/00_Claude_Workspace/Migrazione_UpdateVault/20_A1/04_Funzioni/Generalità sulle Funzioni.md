---
created: 2026-09-23
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/funzioni
aliases: []
origine: UpdateVault
---
[[00_A1_Funzioni|⬅️ Torna a Funzioni]]

# Generalità sulle Funzioni

> [!info] Def
> Dati due insiemi $A,B$ una funzione $f:A\to B$ è una legge che associa a ciascun $x\in A$ uno e un solo elemento $y\in B$. Scriveremo
> $$y=f(x)$$
> $A$ si chiama **dominio** di $f$
> $B$ si chiama **codominio** di $f$
> Se $x\in A$, l'elemento $y=f(x)\in B$ si dice **immagine** di $x$ tramite la funzione.

**DISEGNO NON RAPPRESENTABILE** (segnaposto originale «QUA DISEGNO», subito dopo la definizione di funzione $f:A\to B$: probabilmente il diagramma a frecce tra gli insiemi $A$ e $B$ con $x$ e la sua immagine $f(x)$; da cercare negli appunti della Lezione 4, 23-09-2026, nella pagina «Generalità sulle funzioni»)

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

![[grafico-di-funzione-dominio-immagine.png]]
Il fatto che $\forall\, x_0\in A$ esiste un unico $y_0\in B$ immagine di $x_0$ tramite $f$ ($A,B\subseteq\mathbb{R}$) si interpreta geometricamente sul grafico di $f$ osservando che ogni retta verticale $x=x_0$ interseca il grafico di $f$ al più una volta: $0$ volte se $x_0\notin A$, $1$ volta se $x_0\in A$. In tal caso l'ordinata del punto sul grafico è $y_0=f(x_0)$.

$A=\mathcal{D}(f)$ è la proiezione sull'asse delle ascisse (in direzione parallela all'asse delle $y$) di $\mathcal{G}(f)$.

Inoltre $y_0\in\operatorname{Im}f$ se e solo se esiste un punto $(x_0,y_0)\in\mathcal{G}(f)$ di ordinata $y_0=f(x_0)$, cioè se e solo se la retta orizzontale $y=y_0$ interseca il grafico $\mathcal{G}(f)$ (in almeno un punto).

$\operatorname{Im}f$ è la proiezione di $\mathcal{G}(f)$ sull'asse delle ordinate, in direzione parallela all'asse $x$.

In questo corso ci occupiamo sostanzialmente di funzioni $f:A\subseteq\mathbb{R}\to\mathbb{R}$.

Quando il codominio di $f$ non è esplicitamente dichiarato, è sottinteso che esso sia $\mathbb{R}$.

---
Successivo: [[Funzioni Limitate ed Estremi]]
