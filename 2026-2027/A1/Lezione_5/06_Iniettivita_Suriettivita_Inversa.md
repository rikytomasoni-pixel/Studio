---
tags:
  - AM1
  - funzioni
  - iniettivita
  - suriettivita
  - funzione-inversa
data: 2026-09-25
fonte: Lezione 5
---

# Iniettività, suriettività, funzione inversa

> [!info] Definizione
> Data $f:A\to B$:
> - se $\operatorname{Im}f=B$, $f$ si dice **suriettiva**
> - $f$ si dice **iniettiva** se (equivalentemente):
>   1. $\forall\, x_1,x_2\in A$: $\ x_1\neq x_2 \ \Rightarrow\ f(x_1)\neq f(x_2)$
>   2. $\forall\, x_1,x_2\in A$: $\ f(x_1)=f(x_2) \ \Rightarrow\ x_1=x_2$
>   3. $\forall\, y\in\operatorname{Im}f\ \ \exists!\, x\in A: \ f(x)=y$

**Osservazione.** Sull'equazione $f(x)=y$: se $y\in\operatorname{Im}f$ esiste $x\in\mathcal{D}(f)$ tale che $f(x)=y$, per definizione di $\operatorname{Im}f$.

Allora, se $f$ **suriettiva**, $f(x)=y$ ammette sempre **almeno** una soluzione $x\in\mathcal{D}(f)$, $\forall\, y\in B$.

Se $f$ **iniettiva**, $f(x)=y$ può non avere soluzioni $x\in\mathcal{D}(f)$ per qualche $y\in B$, ma se ne esiste una ($\Leftrightarrow y\in\operatorname{Im}f$) essa è **unica**. Quindi l'equazione ammette **al più** una soluzione, $\forall\, y\in B$.

> [!info] Definizione — Funzione inversa
> Data $f:A\to B$ **iniettiva**, la funzione che ad ogni $y\in\operatorname{Im}f$ associa l'unico $x\in A$ tale che $f(x)=y$ si chiama **inversa** di $f$ e si indica con
> $$f^{-1}: \operatorname{Im}f\subseteq B \longrightarrow A$$
> $$x=f^{-1}(y) \quad\Longleftrightarrow\quad f(x)=y, \qquad y\in\operatorname{Im}f \ \Longleftrightarrow\ x\in A$$

![[FunzioneInversa.png]]

**Osservazioni.**
- $\mathcal{D}(f^{-1}) = \operatorname{Im}f$, $\quad \operatorname{Im}f^{-1} = \mathcal{D}(f)$
- $f^{-1}(f(x)) = x \quad \forall\, x\in\mathcal{D}(f)$
- $f(f^{-1}(y)) = y \quad \forall\, y\in\operatorname{Im}f$

> [!info] Definizione — Invertibilità
> Se $f:A\to B$ è iniettiva, diremo che $f$ è **invertibile** (sulla sua immagine), cioè $\exists\, f^{-1}: \operatorname{Im}f\subseteq B\to A$.

## Esempi

**Esempio.** $f:\mathbb{R}\to\mathbb{R}$, $f(x)=x^2$: né iniettiva, né suriettiva.

**Esempio.** $h:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$, $h(x)=x^2$: $h$ è iniettiva, non suriettiva, $\operatorname{Im}h=[0,\infty)$.

![[LimitazioneXquadrato.png]]

$\exists\, h^{-1}:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$ tale che $h(x)=y$ ammette un'unica soluzione $x\geq 0$, $\big(\mathcal{D}(h)=[0,\infty)\big)$, $\forall\, y\in\operatorname{Im}h=[0,\infty)$:
$$h^{-1}(y) = \sqrt{y} = x$$

**Osservazione.** Anche $g:(-\infty,0]\subseteq\mathbb{R}\to\mathbb{R}$, $g(x)=x^2$ è iniettiva, $\operatorname{Im}g=[0,\infty)$.

L'inversa è $g^{-1}:[0,\infty)\subseteq\mathbb{R}\to\mathbb{R}$, dove $g^{-1}(y)$ è l'unica soluzione di $x^2=g(x)=y$ con $x\in\mathcal{D}(g)=(-\infty,0]$:
$$\Rightarrow \quad g^{-1}(y) = -\sqrt{y} \qquad \forall\, y\in\operatorname{Im}g=[0,\infty)$$

### Note collegate
- [[00_MOC_A1]]
- [[02_Funzioni_Generalità]] — suriettività, immagine, dominio e codominio
- [[00_Esempi_Funzioni_Inverse]] — esempi: potenza n-esima, tangente, seno, coseno
- [[07_Teorema_Monotone_Invertibili]] — le funzioni strettamente monotone sono invertibili
- [[03_Monotonia]]
- [[05_Composizione_di_Funzioni]]
- [[00_Logaritmi]] — inversa dell'esponenziale
- [[05_Radici_e_Potenze]] — radice $n$-esima come inversa di $t^n$