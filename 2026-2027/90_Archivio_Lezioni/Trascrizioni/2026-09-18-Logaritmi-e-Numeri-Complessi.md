---
created: 2026-09-18
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
aliases: []
---
[[00_A1_Indice|⬅️ Torna all'Indice A1]]

# Logaritmi e Numeri Complessi

La lezione chiude il discorso sulle [[2026-09-16-Campi-Ordinati-Estremo-Superiore-e-Potenze|potenze con esponente reale]] introducendo il **logaritmo**, poi estende $\mathbb{R}$ a un campo (non ordinato) in cui $x^2+1=0$ ha soluzione: i **numeri complessi**.

## 1. Logaritmi

Abbiamo definito $a^b$ per ogni $a\in\mathbb{R}$, $a>0$, e per ogni $b\in\mathbb{R}$.

> **Teorema.** Siano $y>0$ e $a>0$, $a\neq 1$. Allora esiste **un unico** $x\in\mathbb{R}$ tale che $a^x=y$.

*(Segue dal fatto che $f(x)=a^x$ è strettamente monotona su $\mathbb{R}$, ha limiti $+\infty$ e $0$ agli estremi del dominio ed è continua.)*

**Definizione.** Tale $x$ si chiama **logaritmo in base $a$ di $y$**:
$$x=\log_a y \qquad(\text{unica soluzione di } a^x=y).$$

**Osservazione:**
$$a^{\log_a y}=y\qquad \forall y>0,\ \forall a>0,\ a\neq1.$$

> [!note] Da sapere
> Le proprietà dei logaritmi (e delle potenze) sono da rivedere sul libro di testo.

## 2. Numeri complessi: motivazione

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

> **Teorema.** $\mathbb{C}$ con $+,\cdot$ è un [[2026-09-16-Campi-Ordinati-Estremo-Superiore-e-Potenze|campo]].

- Elemento neutro della somma: $0=0+i0$. Elemento neutro del prodotto: $1=1+i0$.
- Opposto: se $z=a+ib$ allora $-z=-a-ib$.
- **Inverso**: se $z\neq0$ (cioè $a^2+b^2\neq0$),
$$z^{-1}=\frac1z=\frac{a}{a^2+b^2}-i\,\frac{b}{a^2+b^2}.$$

Verifica:
$$z\cdot z^{-1}=(a+ib)\left(\frac{a}{a^2+b^2}-i\frac{b}{a^2+b^2}\right)=\frac{a^2+b^2}{a^2+b^2}=1+i0=1.$$

**Esempio.** $z=3-4i\ \Rightarrow\ -z=-3+4i,\ \ \dfrac1z=\dfrac{3}{25}+\dfrac{4}{25}i$.

Si ha $\mathbb{R}\subset\mathbb{C}$ tramite l'identificazione $x\in\mathbb{R}\leftrightarrow z=x+i0\in\mathbb{C}$.

## 4. Il piano complesso

$\mathbb{R}$ si identifica con i punti di una retta orientata; $\mathbb{C}$ si identifica con i punti di un **piano** (piano di **Argand–Gauss**). A $z=x+iy$ corrisponde il punto $(x,y)\in\mathbb{R}^2$, con $x=\operatorname{Re}z$ (ascissa) e $y=\operatorname{Im}z$ (ordinata). In questa identificazione $\mathbb{R}$ corrisponde all'**asse delle ascisse** (**asse reale**).

![[piano-complesso-punto-z.png]]

Ogni numero complesso si può pensare come **vettore** del piano $\mathbb{R}^2=\mathbb{C}$ applicato in $O$, con secondo estremo in $(x,y)$ (cfr. [[00_GAL_Indice|vettori in GAL]]).

![[numero-complesso-come-vettore.png]]

### Somma e regola del parallelogramma
Poiché $z+w=(x+a)+i(y+b)$, sommare due complessi equivale a sommare i vettori corrispondenti con la **regola del parallelogramma**. Il significato geometrico della somma è una **traslazione**.

![[somma-complessi-parallelogramma.png]]

## 5. Coniugato e modulo

Dato $z=x+iy\in\mathbb{C}$:

- **Complesso coniugato**: $\bar z=x-iy$.
- **Modulo**: $|z|=\sqrt{x^2+y^2}$.

![[coniugato-e-modulo.png]]

Proprietà:

- $|z|=0\iff z=0$; $\ |z|\ge0\ \ \forall z$.
- $\bar z$ è il **simmetrico** di $z$ rispetto all'asse reale.
- $|z|$ è la **distanza** di $z$ da $O$ nel piano complesso (teorema di Pitagora). Più in generale $|z-w|$ è la distanza tra $z$ e $w$:
$$|z-w|=\sqrt{(x-a)^2+(y-b)^2}\qquad (z=x+iy,\ w=a+ib).$$
- $z=\bar z\iff z\in\mathbb{R}\ (\operatorname{Im}z=0)$.

### Luoghi notevoli
- $\operatorname{Im}z=\text{costante}$: **retta orizzontale**.
- $\operatorname{Re}z=\text{costante}$: **retta verticale**.
- $|z|=\rho\ge0$: **circonferenza** centrata in $O$ di raggio $\rho$.

![[luoghi-notevoli-piano-complesso.png]]

### Identità utili
- $z\bar z=(x+iy)(x-iy)=x^2+y^2=|z|^2$
- $|z|=|\bar z|$
- $z^{-1}=\dfrac1z\cdot\dfrac{\bar z}{\bar z}=\dfrac{\bar z}{|z|^2}=\dfrac{x-iy}{x^2+y^2}$ per $z\neq0$
- $\overline{w\cdot z}=\bar w\cdot\bar z$ e $\overline{w+z}=\bar w+\bar z$
- $\dfrac zw=\dfrac zw\cdot\dfrac{\bar w}{\bar w}=\dfrac{z\bar w}{|w|^2}$ per $w\neq0$

**Esempio.** $z=3-2i,\ w=1+7i$:
$$\frac zw=\frac{z\bar w}{|w|^2}=\frac{(3-2i)(1-7i)}{1+49}=\dots=-\frac{11}{50}-\frac{23}{50}i.$$

## 6. Equazioni in $\mathbb{C}$

Un'equazione in una variabile complessa $z\in\mathbb{C}$ equivale a un **sistema di due equazioni** nelle variabili reali $(x,y)\in\mathbb{R}^2$ (uguagliando parte reale e parte immaginaria).

**Esempio.** $z^2+2\operatorname{Re}z-i\operatorname{Im}z+\bar z=0$, con $z=x+iy$:
$$(x+iy)^2+2x-iy+x-iy=0\ \Rightarrow\ (x^2-y^2+3x)+i(2xy-2y)=0+i0$$
$$\begin{cases}x^2-y^2+3x=0 & (\operatorname{Re})\\ 2xy-2y=0 & (\operatorname{Im})\end{cases}$$
La seconda dà $2y(x-1)=0$: o $y=0$ (e allora $x=0$ oppure $x=-3$), o $x=1$ (e allora $y=\pm2$). Soluzioni:
$$z_0=0,\quad z_1=-3,\quad z_2=1+2i,\quad z_3=1-2i.$$
In questo sistema $x,y\in\mathbb{R}$.

## 7. Forma trigonometrica ed esponenziale (introduzione)

Per individuare $z\in\mathbb{C}$ si possono assegnare $\operatorname{Re}z,\operatorname{Im}z$, oppure, alternativamente, il **modulo** $\rho=|z|=\sqrt{x^2+y^2}$ (distanza da $O$) e l'**argomento** $\theta=\arg z$, l'angolo formato dal semiasse $x>0$ e dalla semiretta uscente da $O$ e passante per $z$ (positivo in senso antiorario, negativo in senso orario).

![[modulo-e-argomento.png]]

Luoghi: $|z|=\rho$ costante è una circonferenza centrata in $O$; $\arg z=\theta$ costante è una **semiretta** uscente da $O$ (esclusa $O$) che forma l'angolo orientato $\theta$ con il semiasse $x>0$.

![[luoghi-modulo-argomento-costanti.png]]

### Osservazioni
- $\arg0$ **non è ben definito**.
- L'argomento di $z\neq0$ è definito **a meno di multipli interi di $2\pi$**: se $\theta=\arg z$, anche $\theta+2k\pi$ ($k\in\mathbb{Z}$) è argomento di $z$.
- Con $\rho\ge0$, $\theta\in\mathbb{R}$:
$$\rho=\sqrt{x^2+y^2},\qquad\begin{cases}x=\rho\cos\theta\\ y=\rho\sin\theta\end{cases}$$
e per $z\neq0$:
$$\cos\theta=\frac{x}{\sqrt{x^2+y^2}}=\frac x\rho,\qquad \sin\theta=\frac{y}{\sqrt{x^2+y^2}}=\frac y\rho,\qquad \tan\theta=\frac yx\ \ (x\neq0).$$

> [!warning] Attenzione
> **Non sempre** $\theta=\arccos\frac{x}{\sqrt{x^2+y^2}}$, né $\theta=\arcsin\frac{y}{\sqrt{x^2+y^2}}$, né $\theta=\arctan\frac yx$: dipende dal **quadrante** in cui si trova $z$.

Per l'arcotangente:
$$\theta=\begin{cases}\arctan\dfrac yx & z\in\text{I, IV quadrante}\\[2mm] \arctan\dfrac yx+\pi & z\in\text{II, III quadrante}\end{cases}$$

**Esempio.** $z=-1-i$ (III quadrante): $\operatorname{Re}z=\operatorname{Im}z=-1$, $\rho=|z|=\sqrt2$, $\arctan\frac{-1}{-1}=\arctan1=\frac\pi4$, quindi
$$\theta=\arg z=\arctan\frac{\operatorname{Im}z}{\operatorname{Re}z}+\pi=\frac54\pi.$$

![[esempio-argomento-meno1-meno-i.png]]
