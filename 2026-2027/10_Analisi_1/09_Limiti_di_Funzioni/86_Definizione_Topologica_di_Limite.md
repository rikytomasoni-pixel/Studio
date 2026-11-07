---
tags:
  - AM1
  - limiti-di-funzioni
  - limite-topologico
  - teorema-ponte
  - definizione
data: 2026-10-23
fonte: "AM1 L13 26-27.pdf (pag. 7-9)"
---

# Definizione topologica di limite

> [!abstract] Definizione (definizione topologica di limite)
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in\overline{\mathbb{R}}$ punto di accumulazione per $I$ ([[83_Punti_di_Accumulazione]]), $\ell\in\overline{\mathbb{R}}$. Diremo che
> $$\lim_{x\to x_0}f(x)=\ell$$
> se e solo se $\forall\,\mathcal{U}(\ell)$ intorno di $\ell$ esiste $\mathcal{U}(x_0)$ intorno di $x_0$ ([[82_Intorni_di_un_Punto_e_di_Infinito]]) tale che
> $$\begin{cases}x\in\mathcal{U}(x_0)\\ x\in I\\ x\neq x_0\end{cases}\Longrightarrow\ f(x)\in\mathcal{U}(\ell)$$
> (le tre condizioni a sinistra equivalgono a $x\in\big(\mathcal{U}(x_0)\cap I\big)\setminus\{x_0\}$).

> [!abstract] Teorema (ponte)
> La definizione successionale di $\displaystyle\lim_{x\to x_0}f(x)=\ell$ ([[84_Definizione_Successionale_di_Limite]]) e la definizione topologica di $\displaystyle\lim_{x\to x_0}f(x)=\ell$ sono **equivalenti**, per $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in\overline{\mathbb{R}}$ punto di accumulazione per $I$, $\ell\in\overline{\mathbb{R}}$.
>
> *(Dimostrazione omessa: «no dim.»)*

## Il caso delle successioni
Il caso $f:\mathbb{N}\subseteq\mathbb{R}\to\mathbb{R}$ delle successioni è **incluso** nella definizione topologica di limite, con $I=\mathbb{N}$, $x_0=+\infty$, $\displaystyle\lim_{n\to\infty}f(n)=\ell\in\overline{\mathbb{R}}$. Si recuperano così le definizioni già date ([[30_Limiti_di_Successioni]]). Infatti:

- **$\ell=+\infty$**, $\mathcal{U}(+\infty)=(M,\infty)$, $M\in\mathbb{R}$: $\ \forall M\ \exists N$ tale che $\forall n>N$, $n\in\mathbb{N}$: $f(n)>M$.
- **$\ell=-\infty$**, $\mathcal{U}(-\infty)=(-\infty,M)$, $M\in\mathbb{R}$: $\ \forall M\ \exists N$ tale che $\forall n>N$, $n\in\mathbb{N}$: $f(n)<M$.
- **$\ell\in\mathbb{R}$**, $\mathcal{U}(\ell)=(\ell-\varepsilon,\ell+\varepsilon)$, $\varepsilon>0$: $\ \forall\varepsilon>0\ \exists N$ tale che $\forall n>N$, $n\in\mathbb{N}$: $\ell-\varepsilon<f(n)<\ell+\varepsilon$ (cioè $|f(n)-\ell|<\varepsilon$).

## Esistenza e non esistenza del limite

> [!note] Osservazione — esiste il limite
> Esiste $\displaystyle\lim_{x\to x_0}f(x)$ in $\overline{\mathbb{R}}$ se e solo se
> $$\exists\,\ell\in\overline{\mathbb{R}}:\ \forall\,\mathcal{U}(\ell)\ \exists\,\mathcal{U}(x_0)\text{ tale che }\forall x\in\big(\mathcal{U}(x_0)\cap I\big)\setminus\{x_0\}\quad f(x)\in\mathcal{U}(\ell)$$

> [!note] Osservazione — non esiste il limite
> **Non** esiste $\displaystyle\lim_{x\to x_0}f(x)$ in $\overline{\mathbb{R}}$ se e solo se
> $$\forall\,\ell\in\overline{\mathbb{R}}\ \exists\,\mathcal{U}(\ell)\text{ tale che }\forall\,\mathcal{U}(x_0)\ \exists\,x\in\big(\mathcal{U}(x_0)\cap I\big)\setminus\{x_0\}\text{ tale che }f(x)\notin\mathcal{U}(\ell)$$

Specificando la forma esplicita degli intorni si ottengono le definizioni metriche: [[87_Definizioni_Metriche_di_Limite_all_Infinito]].

## Note collegate
- [[84_Definizione_Successionale_di_Limite]]
- [[85_Teorema_di_Unicita_del_Limite]]
- [[87_Definizioni_Metriche_di_Limite_all_Infinito]]
- [[82_Intorni_di_un_Punto_e_di_Infinito]]
- [[30_Limiti_di_Successioni]]
- [[00_MOC_Analisi_1]]

#AM1/limiti-di-funzioni/definizione-topologica
