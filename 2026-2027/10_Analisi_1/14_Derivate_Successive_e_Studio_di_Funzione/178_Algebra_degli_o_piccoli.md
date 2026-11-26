---
tags:
  - AM1
  - o-piccolo
  - asintotico
  - algebra
  - richiamo
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 15-16)"
---

# Algebra degli $o$-piccoli (richiamo)

Richiami per $x\to x_0$ ([[106_Asintotico_e_o_piccolo_per_Funzioni]], [[107_Proprieta_degli_Asintotici_per_Funzioni]]):

- $f\sim g\iff\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=1\iff f=g+o(g)$
- $f=o(g)\iff\displaystyle\lim_{x\to x_0}\frac{f(x)}{g(x)}=0$

> [!abstract] Proprietà
> - $o(f)\pm o(f)=o(f)$
> - $c\,o(f)=o(cf)=o(f)\quad\forall c\in\mathbb{R}\setminus\{0\}$
> - $o(f)\cdot o(g)=o(f\cdot g)=f\cdot g\cdot o(1)$
> - $f\cdot o(g)=o(f\cdot g)=f\cdot g\cdot o(1)$
> - se $f\sim g$ allora $o(f)=o(g)$ (ad es. $o\big((\sin x)^3\big)=o(x^3)$ per $x\to0$)

Inoltre:

- $o(x)+o(x^2)=o(x)$ per $x\to0$
- $o(x)+o(x^2)=o(x^2)$ per $x\to\infty$

> [!tip] Regola
> Per $x\to0$ "vince" l'$o$-piccolo di grado **più basso**; per $x\to\infty$ quello di grado **più alto**.

## Note collegate
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[107_Proprieta_degli_Asintotici_per_Funzioni]]
- [[41_o_piccolo_e_Asintotico]]
- [[176_Esempio_Limite_con_Sviluppi_di_Taylor]]
- [[00_MOC_Analisi_1]]

#AM1/o-piccolo/algebra
