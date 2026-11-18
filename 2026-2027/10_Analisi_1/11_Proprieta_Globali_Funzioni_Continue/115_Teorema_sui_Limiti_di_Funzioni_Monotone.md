---
tags:
  - AM1
  - monotonia
  - limiti-di-funzioni
  - discontinuita
  - teorema
data: 2026-11-06
lezione: 16
fonte: "AM1 L16 26-27.pdf (pag. 10-13)"
---

# Teorema sui limiti di funzioni monotone su un intervallo

> [!abstract] Teorema
> Sia $f:(a,b)\to\mathbb{R}$ monotona **crescente** (decrescente). Allora $\forall x_0\in(a,b)$ esistono finiti i limiti
> $$\lim_{x\to x_0^-}f(x),\quad\lim_{x\to x_0^+}f(x)\in\mathbb{R}$$
> Inoltre, per $f$ crescente,
> $$\lim_{x\to x_0^-}f(x)=\sup_{(a,x_0)}f(x)\in\mathbb{R}\qquad\lim_{x\to x_0^+}f(x)=\inf_{(x_0,b)}f(x)\in\mathbb{R}$$
> $$\lim_{x\to x_0^-}f(x)\le f(x_0)\le\lim_{x\to x_0^+}f(x)$$
>![[MononiaDiscontinua.png]]
Infine esistono, eventualmente infiniti,
> $$\lim_{x\to a^+}f(x)=\inf_{(a,b)}f(x)\in\mathbb{R}\cup\{-\infty\}\qquad\lim_{x\to b^-}f(x)=\sup_{(a,b)}f(x)\in\mathbb{R}\cup\{+\infty\}$$


> [!abstract] Caso $f$ decrescente
> $\forall x_0\in(a,b)$:
> $$\lim_{x\to x_0^-}f(x)=\inf_{(a,x_0)}f(x)\in\mathbb{R}\qquad\lim_{x\to x_0^+}f(x)=\sup_{(x_0,b)}f(x)\in\mathbb{R}$$
> $$\lim_{x\to x_0^-}f(x)\ge f(x_0)\ge\lim_{x\to x_0^+}f(x)$$
> Inoltre esistono, eventualmente infiniti,
> $$\lim_{x\to a^+}f(x)=\sup_{(a,b)}f(x)\in\mathbb{R}\cup\{+\infty\}\qquad\lim_{x\to b^-}f(x)=\inf_{(a,b)}f(x)\in\mathbb{R}\cup\{-\infty\}$$

*Senza dimostrazione: simile alla dimostrazione del teorema di regolarità per le successioni monotone ([[31_Successioni_Monotone]]).*

> [!abstract] Corollario
> Se $f:(a,b)\to\mathbb{R}$ è monotona, i suoi eventuali punti di discontinuità in $(a,b)$ sono solo di **tipo salto** ([[97_Discontinuita_di_Prima_Specie_a_Salto]]). Inoltre in $x=a$, $x=b$ $f$ ammette limite finito (quindi è ivi prolungabile per continuità se $a,b\in\mathbb{R}$, [[96_Discontinuita_Eliminabile_e_Prolungamento_per_Continuita]]), oppure infinito (quindi ammette asintoto verticale se $a,b\in\mathbb{R}$, [[91_Limiti_Destro_e_Sinistro_e_Asintoto_Verticale]]).

## Note collegate
- [[23_Monotonia]]
- [[31_Successioni_Monotone]]
- [[116_Continuita_e_Invertibilita]]
- [[00_MOC_Analisi_1]]

#AM1/proprieta-globali/limiti-funzioni-monotone
