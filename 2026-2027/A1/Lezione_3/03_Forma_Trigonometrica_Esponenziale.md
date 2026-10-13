---
tags:
  - AM1
  - numeri-complessi
  - forma-trigonometrica
  - forma-esponenziale
  - formula-di-eulero
  - argomento
data: 2026-09-18
fonte: Lezione 3 e Lezione 4
---

# Forma trigonometrica e forma esponenziale (di $z\in\mathbb{C}$)

Per individuare $z\in\mathbb{C}$ possiamo assegnare $\operatorname{Re} z, \operatorname{Im} z \in \mathbb{R}$ ($z = \operatorname{Re} z + i\operatorname{Im} z$).

Alternativamente, possiamo individuare $z\in\mathbb{C}$ assegnando:
- $|z| = \sqrt{x^2+y^2} = \rho$, **distanza** di $z$ da $O$;
- $\theta = \arg z$ (**argomento** di $z$), l'angolo formato dal semiasse delle $x>0$ e dalla semiretta uscente da $O$ e passante per $z$ (dal semiasse alla semiretta: $+$ in senso antiorario, $-$ in senso orario).
![[FormaTrigonometricaComplessa.png]]

$$|z| = \sqrt{x^2+y^2} = \rho \quad \text{(modulo di } z\text{)}, \qquad \theta = \arg z \quad \text{(argomento di } z\text{)}$$

## Osservazioni sull'argomento

![[CostantiComplesseTrigonometriche.png]]

- $|z|=\rho=\text{costante}$ → circonferenza centrata in $O$ di raggio $\rho\geq 0$
- $\arg z = \text{costante} = \theta$ → semiretta uscente da $O$ (senza $O$) che forma angolo orientato $\theta$ con l'asse delle $x>0$

**Osservazioni.**
- $\arg 0$ **non è ben definito**
- L'argomento di $z\in\mathbb{C}\setminus\{0\}$ è definito **a meno di multipli interi di $2\pi$**, cioè se $\theta=\arg z$ allora anche $\theta+2k\pi$ è argomento di $z$, $\forall\, k\in\mathbb{Z}$

Riassumendo: $\rho\geq 0,\ \theta\in\mathbb{R}$ individuano $z=x+iy$, con $x,y\in\mathbb{R}$.

## Relazioni tra coordinate cartesiane e polari

$$\rho = \sqrt{x^2+y^2}$$
$$\begin{cases} x = \rho\cos\theta \\ y = \rho\sin\theta \end{cases}$$

Inoltre, per $z=x+iy\neq 0$:
$$\cos\theta = \dfrac{x}{\sqrt{x^2+y^2}} = \dfrac{x}{\rho}, \qquad \sin\theta = \dfrac{y}{\sqrt{x^2+y^2}} = \dfrac{y}{\rho}$$

In particolare, se $x\neq 0$:
$$\operatorname{tg}\theta = \dfrac{\sin\theta}{\cos\theta} = \dfrac{y}{x}$$

> [!danger] Attenzione
> - **Può non essere** $\theta = \arccos \dfrac{x}{\sqrt{x^2+y^2}}$
> - **Può non essere** $\theta = \arcsin \dfrac{y}{\sqrt{x^2+y^2}}$
> - **Può non essere** $\theta = \arctan \dfrac{y}{x}$
>
> Dipende dal **quadrante** in cui si trova $z$!

Nello specifico:
$$\theta = \arctan\dfrac{y}{x} \qquad \text{se } z \in \text{I, IV quadrante}$$
$$\theta = \arctan\dfrac{y}{x} + \pi \qquad \text{se } z \in \text{II, III quadrante}$$

### Esempio

$z = -1-i$: $\operatorname{Im} z = -1$, $\operatorname{Re} z = -1$ ($z$ è nel III quadrante).

![[ProblematicaCalcoloArgomento.png]]

$$\rho = |z| = \sqrt{2}, \qquad \theta = \arg z = \dfrac{5}{4}\pi$$

Infatti:
$$\arctan\dfrac{\operatorname{Im} z}{\operatorname{Re} z} = \arctan\dfrac{-1}{-1} = \arctan 1 = \dfrac{\pi}{4}$$

ma essendo $z$ nel III quadrante, va aggiunto $\pi$:
$$\arg z = \arctan\dfrac{\operatorname{Im} z}{\operatorname{Re} z} + \pi = \dfrac{\pi}{4}+\pi = \dfrac{5}{4}\pi$$

---

## Forma trigonometrica ed esponenziale

$z\in\mathbb{C}$, $z=x+iy$, $x=\operatorname{Re}z$, $y=\operatorname{Im}z$

$\rho=|z|$, $\theta=\arg(z)$

**![[NumeroComplessoPolare.png]]**

**Oss:** Si chiama argomento principale di $z\in\mathbb{C}\setminus\{0\}$ l'unico argomento di $z$ in $[0,2\pi)$ o in $[-\pi,\pi)$ a seconda delle convenzioni.

> [!warning] Def
> Dato $z\in\mathbb{C}$, $z=x+iy$
> $$z = x+iy \quad \text{forma algebrica}$$
> $$= \rho(\cos\theta+i\sin\theta) \quad \text{forma trigonometrica}$$
> si dice rappresentazione di $z$ in forma trigonometrica.
> $$x=\operatorname{Re}z\ (\in\mathbb{R}), \quad y=\operatorname{Im}z\ (\in\mathbb{R}), \quad \rho=|z|\ (\in[0,\infty)), \quad \theta=\arg z\ (\in\mathbb{R})$$

**Es:**
$$z=-1=-1+i0$$
$$= -1(\cos 0+i\sin 0) \qquad \text{NO} \quad \text{(algebricamente corretta)}$$
$$= 1(\cos\pi+i\sin\pi) \qquad \text{SÌ}$$
con $1=|-1|$, $\pi=\arg(-1)$

> [!warning] Def
> Dato $z\in\mathbb{C}$
> $$z = x+iy = \rho(\cos\theta+i\sin\theta) = \rho e^{i\theta} \quad \text{forma esponenziale}$$
> rappresentazione di $z\in\mathbb{C}$ in forma esponenziale.

**Oss:** $\forall\,\theta\in\mathbb{R}$
$$e^{i\theta} = \cos\theta+i\sin\theta \qquad \text{Formula di Eulero}$$
$$\left(e^{i\pi}+1=0\right)$$

### Note collegate
- [[00_MOC_A1]]
- [[01_Numeri_Complessi]] — forma algebrica
- [[02_Piano_di_Argand_Gauss]] — modulo e rappresentazione geometrica
- [[00_Formule_di_De_Moivre]] — prodotto, quoziente, potenze
- [[01_Radici_Complesse]] — radici $n$-esime in forma esponenziale