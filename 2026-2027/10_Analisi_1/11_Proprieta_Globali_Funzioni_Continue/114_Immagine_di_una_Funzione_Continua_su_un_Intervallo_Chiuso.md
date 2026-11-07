---
tags:
  - AM1
  - continuita
  - immagine
  - weierstrass
  - corollario
data: 2026-11-06
lezione: 16
fonte: "AM1 L16 26-27.pdf (pag. 9-10)"
---

# Immagine di una funzione continua su $[a,b]$

> [!abstract] Corollario
> Se $f:[a,b]\to\mathbb{R}$ è continua, $a,b\in\mathbb{R}$, $a<b$, allora
> $$\operatorname{Im}f=[m,M]\qquad\text{con }m=\min_{[a,b]}f,\ M=\max_{[a,b]}f\in\mathbb{R}$$

**Dimostrazione.** Per il [[112_Teorema_di_Weierstrass|teorema di Weierstrass]], $\exists$
$$m=\min_{[a,b]}f=f(x_m)\in\mathbb{R},\qquad M=\max_{[a,b]}f=f(x_M)\in\mathbb{R}$$
con $x_m,x_M\in[a,b]$. In particolare $m,M\in\operatorname{Im}f$, ed essi coincidono con
$$m=\inf_{[a,b]}f\qquad M=\sup_{[a,b]}f$$
Per il [[113_Teorema_dei_Valori_Intermedi|teorema dei valori intermedi]] ogni valore intermedio viene assunto, quindi $[m,M]=\operatorname{Im}f$. $\square$

## Note collegate
- [[112_Teorema_di_Weierstrass]]
- [[113_Teorema_dei_Valori_Intermedi]]
- [[00_MOC_Analisi_1]]

#AM1/proprieta-globali/immagine-intervallo-chiuso
