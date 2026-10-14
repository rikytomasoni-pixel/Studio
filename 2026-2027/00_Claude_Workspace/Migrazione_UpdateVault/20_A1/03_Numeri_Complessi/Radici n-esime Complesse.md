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

# Radici n-esime Complesse

> [!info] Def
> Sia $w\in\mathbb{C}$, $n\in\mathbb{N}$, $n\geq 1$ allora ogni numero complesso $z\in\mathbb{C}$ tale che
> $$z^n=w$$
> si chiama **radice $n$-esima complessa** di $w$.

**Es:** $\sqrt[2]{4}=2$ in $\mathbb{R}$
$$\sqrt[2]{4}=\pm 2 \quad \text{in } \mathbb{C}$$

> [!abstract] Teorema (sulle radici n-esime complesse)
> Sia $w\in\mathbb{C}$, $w\neq 0$, $n\in\mathbb{N}$, $n\geq 1$ allora esistono esattamente $n$ radici $n$-esime complesse distinte di $w$. In particolare se
> $$w=re^{i\varphi}=r(\cos\varphi+i\sin\varphi)$$
> allora le radici complesse $n$-esime $z_0,z_1,\dots,z_{n-1}$ di $w$ hanno la forma
> $$z_k = r^{1/n}(\cos\theta_k+i\sin\theta_k) = r^{1/n}e^{i\theta_k}$$
> con
> $$\theta_k = \dfrac{\varphi}{n}+\dfrac{2k\pi}{n}, \qquad k=0,\dots,n-1$$

**dim:** Dato $w=re^{i\varphi}$, $r\neq 0$. Cerchiamo $z=\rho e^{i\theta}$ tale che $z^n=w$
$$\Rightarrow \quad z^n = \rho^n e^{in\theta} = w=re^{i\varphi} \qquad \text{(de Moivre)}$$

$$\Rightarrow \quad \begin{cases} \rho^n = r \\ n\theta = \varphi+2h\pi \end{cases} \qquad h\in\mathbb{Z}$$

$$\Rightarrow \quad \begin{cases} \rho = r^{1/n} & \text{(radice reale)} \\ \theta = \dfrac{\varphi}{n}+\dfrac{2h\pi}{n} & h\in\mathbb{Z} \end{cases} \qquad (*)$$

sono tutte e sole le radici complesse $n$-esime di $w$ in $\mathbb{C}$, non distinte. Scriviamo
$$h = q\cdot n+k$$
con $q$ quoziente, $k$ resto della divisione di $h$ per $n$
$$\Rightarrow \quad q\in\mathbb{Z}, \quad k\in\{0,1,\dots,n-1\}$$
Vale
$$\dfrac{2\pi h}{n} = \dfrac{2\pi(qn+k)}{n} = 2\pi q+\dfrac{2\pi k}{n}$$

Se $h_1,h_2\in\mathbb{Z}$ hanno lo stesso resto $k$ nella divisione, quando si divide per $n$ essi individuano lo stesso numero complesso $z_k$ in $(*)$, con argomento $\dfrac{\varphi}{n}+\dfrac{2k\pi}{n}$, poiché danno luogo ad argomenti che sono sfasati di un multiplo intero di $2\pi$.

Quindi le radici $n$-esime complesse distinte di $w$ sono tante quante i possibili resti di una divisione di un intero per $n$, cioè $n$. Esse sono
$$z_k = r^{1/n}e^{i\theta_k} = r^{1/n}\left[\cos\theta_k+i\sin\theta_k\right]$$
con $\theta_k = \dfrac{\varphi}{n}+\dfrac{2k\pi}{n}$, $k=\{0,1,\dots,n-1\}$ $\blacksquare$

**Oss:** Tutte le radici complesse di $w=re^{i\varphi}\in\mathbb{C}\setminus\{0\}$ hanno lo stesso modulo
$$|z_0|=|z_1|=\cdots=|z_{n-1}|=r^{1/n}$$
Nel piano complesso giacciono sulla circonferenza di centro $O$ e raggio $r^{1/n}$.

Inoltre due radici successive hanno argomenti che differiscono di un numero fisso $\dfrac{2\pi}{n}$ (cioè l'angolo al centro della circonferenza formato da due radici successive è sempre lo stesso, $\dfrac{2\pi}{n}$).

Quindi le radici $n$-esime complesse si dispongono a formare un poligono regolare di $n$ lati inscritto nella circonferenza di centro $O$ e raggio $r^{1/n}$.

$n=2$: ![[radici-quadrate-diametro.png|305]] — diametro

$n=3$: ![[radici-cubiche-triangolo-equilatero.png|306]] — triangolo equilatero

$n=4$: … — quadrato

**Oss:** Le radici complesse $n$-esime ($n\geq 2$) di $w\in\mathbb{C}\setminus\{0\}$ formano un insieme di $n$ valori. La radice complessa $n$-esima **non è** una funzione da $\mathbb{C}$ in $\mathbb{C}$.

**Es:** calcolare e rappresentare in $\mathbb{C}$ le radici seste di $w=-1$
$$z^6=-1$$
$$w = -1e^{i0} \qquad \text{\small(vero ma non serve)}$$
$$= 1e^{i\pi}$$

![[radici-seste-di-meno-uno-punto-w.png]]

$$|w|=1 \qquad \arg w = \pi$$
$$z_k = 1^{1/6}\,e^{i\left(\frac{\pi}{6}+\frac{2k\pi}{6}\right)} \qquad k=0,1,2,3,4,5$$
$$= 1\cdot e^{i\left(\frac{\pi}{6}+\frac{k\pi}{3}\right)}$$

$$z_0 = e^{i\frac{\pi}{6}} = \cos\dfrac{\pi}{6}+i\sin\dfrac{\pi}{6} = \dfrac{\sqrt3}{2}+\dfrac{i}{2}$$
$$z_1 = e^{i\frac{\pi}{2}} = \cos\dfrac{\pi}{2}+i\sin\dfrac{\pi}{2} = i$$
$$z_2 = e^{i\frac{5}{6}\pi} = \cos\dfrac{5}{6}\pi+i\sin\dfrac{5}{6}\pi = -\dfrac{\sqrt3}{2}+\dfrac{i}{2}$$
$$z_3 = e^{i\frac{7}{6}\pi} = \cos\dfrac{7}{6}\pi+i\sin\dfrac{7}{6}\pi = -\dfrac{\sqrt3}{2}-\dfrac{i}{2}$$
$$z_4 = e^{i\frac{3}{2}\pi} = \cos\dfrac{3}{2}\pi+i\sin\dfrac{3}{2}\pi = -i$$
$$z_5 = e^{i\frac{11}{6}\pi} = \cos\dfrac{11}{6}\pi+i\sin\dfrac{11}{6}\pi = \dfrac{\sqrt3}{2}-\dfrac{i}{2}$$

![[radici-seste-di-meno-uno-esagono.png|469]] — esagono regolare

---
Precedente: [[Formule di de Moivre]] · Successivo: [[Equazioni di Secondo Grado e Teorema Fondamentale dell'Algebra]]
