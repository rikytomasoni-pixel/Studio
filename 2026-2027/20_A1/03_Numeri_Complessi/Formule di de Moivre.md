---
created: 2026-09-23
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/4
  - argomento/numeri_complessi
aliases: []
origine: UpdateVault
---
[[00_A1_Numeri_Complessi|⬅️ Torna a Numeri Complessi]]

# Formule di de Moivre

> [!abstract] Teorema (Formule di de Moivre)
> Siano $w,z\in\mathbb{C}$, se
> $$w = R(\cos\varphi+i\sin\varphi) = Re^{i\varphi}$$
> $$z = r(\cos\theta+i\sin\theta) = re^{i\theta}$$
> $$\Rightarrow \quad w\cdot z = rR\left[\cos(\theta+\varphi)+i\sin(\theta+\varphi)\right] = rRe^{i(\theta+\varphi)}$$
> inoltre se $w\neq 0$
> $$\Rightarrow \quad \dfrac{z}{w} = \dfrac{r}{R}\left[\cos(\theta-\varphi)+i\sin(\theta-\varphi)\right] = \dfrac{r}{R}e^{i(\theta-\varphi)}$$

**Oss:**
$$|z\cdot w| = |z|\cdot|w|$$
$$\arg(zw) = \arg z+\arg w$$
$$\left|\dfrac{z}{w}\right| = \dfrac{|z|}{|w|} \qquad (w\neq 0)$$
$$\arg\left(\dfrac{z}{w}\right) = \arg z-\arg w$$

**Oss:** se $z=1=1\cdot e^{i0}$ troviamo che se $w=Re^{i\varphi}\neq 0$
$$w^{-1} = \dfrac{1}{w} = \dfrac{1}{R}(\cos\varphi-i\sin\varphi) = \dfrac{1}{R}e^{-i\varphi}$$

**Oss:** Dato $z\in\mathbb{C}$ con $z=r(\cos\theta+i\sin\theta)=re^{i\theta}$ allora $\forall\, n\in\mathbb{N}$
$$z^n = r^n(\cos n\theta+i\sin n\theta) = r^n e^{in\theta}$$
se $z\neq 0$
$$z^{-n} = \dfrac{1}{r^n}(\cos n\theta-i\sin n\theta) = r^{-n}e^{-in\theta}$$

**Oss:** sono formule coerenti con l'algebra degli esponenziali, anche se coinvolgono i numeri complessi.

**Es:** $z=-1-i\sqrt{3}$, $n=7$
$$z^7 = ?$$
$$z=re^{i\theta} \ \Rightarrow\ z^7 = r^7 e^{i7\theta}$$

![[esempio-z-meno1-meno-i-radice3.png]]

$$r=\sqrt{1+3}=2 \qquad \theta=\arg z$$

$$\cos\theta=-\dfrac{1}{2}, \qquad \sin\theta=-\dfrac{\sqrt3}{2}, \qquad \operatorname{tg}\theta=\sqrt3$$
$$\theta = \arctan\sqrt3+\pi = \dfrac{\pi}{3}+\pi = \dfrac{4}{3}\pi$$
$$z = 2e^{i\frac{4}{3}\pi} \quad \Rightarrow \quad z^7 = 2^7 e^{i\frac{28}{3}\pi} = 2^7 e^{i\frac{4}{3}\pi}$$

$$z^7 = 2^7 e^{i\frac{4}{3}\pi} = 2^7\left(\cos\dfrac{4}{3}\pi+i\sin\dfrac{4}{3}\pi\right)$$
$$= -2^7\left(\dfrac{1}{2}+i\dfrac{\sqrt3}{2}\right) = -2^6-2^6\sqrt3\, i$$

## Formule di De Moivre (prodotto)

$$z = re^{i\theta} = r(\cos\theta+i\sin\theta)$$
$$w = Re^{i\varphi} = R(\cos\varphi+i\sin\varphi)$$
$$\Rightarrow \quad z\cdot w = rR\left[\cos(\theta+\varphi)+i\sin(\theta+\varphi)\right] = rRe^{i(\theta+\varphi)}$$

**dim:**
$$z\cdot w = r(\cos\theta+i\sin\theta)\cdot R(\cos\varphi+i\sin\varphi)$$
$$= rR\left[(\cos\theta\cos\varphi-\sin\theta\sin\varphi) + i(\sin\theta\cos\varphi+\cos\theta\sin\varphi)\right] \qquad \text{\small(identità trigonometriche)}$$
$$= rR\left[\cos(\theta+\varphi)+i\sin(\theta+\varphi)\right]$$
$$= rRe^{i(\theta+\varphi)} \qquad \blacksquare$$

**Oss:** Per il quoziente la dimostrazione è analoga
$$\dfrac{z}{w} = \dfrac{z\cdot\overline{w}}{|w|^2} = \cdots$$

**Oss:** Dati $z=re^{i\theta}$, $w=Re^{i\varphi}$ vale $z\cdot w=rRe^{i(\theta+\varphi)}$

![[prodotto-complessi-rotoomotetia.png]]

Moltiplicare $z$ per $w$ corrisponde a ruotare $z$ nel piano complesso di un angolo pari a $\varphi=\arg w$ ($+$ in senso antiorario, $-$ in senso orario) e a dilatare $z$ di un fattore pari a $R=|w|$
(rotazione - omotetia)

---
Precedente: [[Forma Trigonometrica ed Esponenziale]] · Successivo: [[Radici n-esime Complesse]]
