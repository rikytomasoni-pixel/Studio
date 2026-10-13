---
tags:
  - AM1
  - numeri-complessi
  - piano-di-argand-gauss
  - coniugato
  - modulo
data: 2026-09-18
fonte: Lezione 3
---

# Piano di Argand-Gauss, coniugato e modulo

## Rappresentazione geometrica

**Osservazione.** $\mathbb{R}$ può essere identificato con i punti di una retta orientata. $\mathbb{C}$ può essere identificato con i punti di un **piano**.

A $z=x+iy\in\mathbb{C}$, $x,y\in\mathbb{R}$, corrisponde il punto nel piano cartesiano di coordinate $(x,y)\in\mathbb{R}^2$:
$$x = \operatorname{Re} z \ \text{(ascissa)}, \qquad y = \operatorname{Im} z \ \text{(ordinata)}$$

![[PianoArgandGauss.png]]
In questa identificazione, $\mathbb{R}$ corrisponde all'asse delle ascisse (**asse reale**); il piano nel suo complesso si chiama **piano di Argand-Gauss** (o piano complesso).

## Numero complesso come vettore

In particolare, ogni numero complesso può essere pensato come **vettore** nel piano $\mathbb{R}^2=\mathbb{C}$, applicato in $O$ e avente il secondo estremo in $(x,y) = x+iy = z$, orientato da $O$ a $(x,y)$.
![[ModuloDelVettoreComplesso.png]]
**Osservazione.** Poiché $\forall\, z=x+iy\in\mathbb{C}$, $\forall\, w=a+ib\in\mathbb{C}$:
$$z+w = (x+a)+i(y+b)$$

![[ComposizioneDiVettoriComplessi.png]]

**Sommare due numeri complessi corrisponde a sommare, nel piano, i corrispondenti vettori che li rappresentano**, tramite la regola del parallelogramma: sommando si compongono gli spostamenti. Il significato geometrico della somma in $\mathbb{C}$ (piano complesso) è una **traslazione**.

**Osservazione.** Il piano complesso si chiama anche piano di **Argand-Gauss**.

## Coniugato e modulo

> [!warning] Definizione — Complesso coniugato
> Dato $z=x+iy\in\mathbb{C}$, chiamiamo
> $$\overline{z} = x-iy$$
> **complesso coniugato** di $z\in\mathbb{C}$.

> [!warning] Definizione — Modulo
> Indichiamo con
> $$|z| = \sqrt{x^2+y^2}$$
> il **modulo** di $z\in\mathbb{C}$.

**Osservazioni.**
- $|z|=0$ se e solo se $z=0$
- $|z|\geq 0 \ \ \forall\, z\in\mathbb{C}$

![[RelazioneModuloConiugato.png]]

- $\overline{z}$ è il simmetrico di $z$ rispetto all'asse reale
- $|z|$ è la distanza di $z\in\mathbb{C}$ da $0$ nel piano complesso (teorema di Pitagora), per ogni $z\in\mathbb{C}$
- Più in generale, $|z-w|$ è la distanza di $z\in\mathbb{C}$ da $w\in\mathbb{C}$ nel piano complesso: se $z=x+iy$, $w=a+ib$,
$$|z-w| = \sqrt{(x-a)^2+(y-b)^2}$$
- $z=\overline{z}$ se e solo se $z\in\mathbb{R}$ (cioè $\operatorname{Im} z = 0$)

## Luoghi geometrici notevoli

- $\operatorname{Re} z = \text{costante}$ → retta **verticale**
- $\operatorname{Im} z = \text{costante}$ → retta **orizzontale**
- $|z| = \text{costante} = \rho \geq 0$ → circonferenza centrata in $O$, di raggio $\rho$
![[RappresentazioneCostantiComplesse.png]]

## Proprietà algebriche

$$z\cdot \overline{z} = (x+iy)(x-iy) = x^2+y^2 = |z|^2 \qquad \forall\, z\in\mathbb{C}$$
$$|z| = |\overline{z}| \qquad \forall\, z\in\mathbb{C}$$
$$z^{-1} = \dfrac{1}{z} = \dfrac{\overline{z}}{\overline{z}\, z} = \dfrac{\overline{z}}{|z|^2} = \dfrac{x-iy}{x^2+y^2} \qquad \forall\, z\in\mathbb{C}\setminus\{0\},\ \ z=x+iy$$
$$\overline{(w\cdot z)} = \overline{w}\cdot \overline{z} \qquad \forall\, z,w\in\mathbb{C}$$
$$\overline{(w+z)} = \overline{w}+\overline{z} \qquad \forall\, z,w\in\mathbb{C}$$
$$\dfrac{z}{w} = \dfrac{z}{w}\cdot\dfrac{\overline{w}}{\overline{w}} = \dfrac{z\cdot \overline{w}}{|w|^2} \qquad \forall\, z\in\mathbb{C},\ \forall\, w\in\mathbb{C}\setminus\{0\}$$

**Esempio.** $z=3-2i$, $w=1+7i$:
$$\dfrac{z}{w} = \dfrac{z\cdot \overline{w}}{|w|^2} = \dfrac{(3-2i)(1-7i)}{1+49} = \dfrac{-11-23i}{50} = -\dfrac{11}{50} - \dfrac{23}{50}i$$

### Note collegate
- [[00_MOC_A1]]
- [[01_Numeri_Complessi]] — forma algebrica, somma e prodotto
- [[03_Forma_Trigonometrica_Esponenziale]] — modulo e argomento
- [[00_Formule_di_De_Moivre]] — moltiplicazione come rotazione-omotetia
- [[03_Valore_Assoluto]] — analogo del modulo in $\mathbb{R}$
- [[04_Retta_Reale_Intervalli]] — rappresentazione geometrica di $\mathbb{R}$
- [[04_Equazioni_in_C]]