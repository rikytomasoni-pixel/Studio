---
created: 2026-09-18
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/3
  - argomento/numeri_complessi
aliases: []
origine: UpdateVault
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Modulo e Argomento

Per individuare $z\in\mathbb{C}$ possiamo assegnare $\operatorname{Re} z, \operatorname{Im} z \in \mathbb{R}$ ($z = \operatorname{Re} z + i\operatorname{Im} z$).

Alternativamente, possiamo individuare $z\in\mathbb{C}$ assegnando:
- $|z| = \sqrt{x^2+y^2} = \rho$, **distanza** di $z$ da $O$;
- $\theta = \arg z$ (**argomento** di $z$), l'angolo formato dal semiasse delle $x>0$ e dalla semiretta uscente da $O$ e passante per $z$ (dal semiasse alla semiretta: $+$ in senso antiorario, $-$ in senso orario).
![[modulo-e-argomento.png]]

$$|z| = \sqrt{x^2+y^2} = \rho \quad \text{(modulo di } z\text{)}, \qquad \theta = \arg z \quad \text{(argomento di } z\text{)}$$

## Osservazioni sull'argomento

![[luoghi-modulo-argomento-costanti.png]]

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

![[esempio-argomento-meno1-meno-i.png]]

$$\rho = |z| = \sqrt{2}, \qquad \theta = \arg z = \dfrac{5}{4}\pi$$

Infatti:
$$\arctan\dfrac{\operatorname{Im} z}{\operatorname{Re} z} = \arctan\dfrac{-1}{-1} = \arctan 1 = \dfrac{\pi}{4}$$

ma essendo $z$ nel III quadrante, va aggiunto $\pi$:
$$\arg z = \arctan\dfrac{\operatorname{Im} z}{\operatorname{Re} z} + \pi = \dfrac{\pi}{4}+\pi = \dfrac{5}{4}\pi$$

---
Precedente: [[Equazioni in C]] · Successivo: [[Forma Trigonometrica ed Esponenziale]]
