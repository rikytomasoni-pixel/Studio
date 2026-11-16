---
tags:
  - AM1
  - derivate
  - estremi
  - definizione
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 6-8)"
---

# Massimi e minimi locali e globali

> [!abstract] Definizione (estremi locali)
> Sia $f:\mathcal{D}(f)\subseteq\mathbb{R}\to\mathbb{R}$ e $x_0\in\mathcal{D}(f)$. Diremo che $x_0$ è punto di **massimo (minimo) locale** per $f$ se esiste un intorno $(x_0-\delta,x_0+\delta)$ di $x_0$, con $\delta>0$, tale che
> $$f(x)\le f(x_0)\quad\big(f(x)\ge f(x_0)\big)\qquad\forall x\in(x_0-\delta,x_0+\delta)\cap\mathcal{D}(f)$$
> Il corrispondente valore $f(x_0)$ si dice massimo (minimo) locale. Diremo che esso è **stretto** se
> $$f(x)<f(x_0)\quad\big(f(x)>f(x_0)\big)\qquad\forall x\in(x_0-\delta,x_0+\delta)\cap\mathcal{D}(f),\ x\neq x_0$$

> [!abstract] Definizione (estremi assoluti o globali)
> $x_0$ è punto di **massimo (minimo) assoluto o globale** se
> $$f(x)\le f(x_0)\quad\big(f(x)\ge f(x_0)\big)\qquad\forall x\in\mathcal{D}(f)$$
> Il valore $f(x_0)$ si dice massimo (minimo) assoluto o globale di $f$. È **stretto** se $f(x)<f(x_0)$ ($f(x)>f(x_0)$) per ogni $x\in\mathcal{D}(f)$, con $x\neq x_0$.

> [!abstract] Definizione (punto di estremo)
> Se $x_0$ è punto di massimo o di minimo per $f$ (locale o globale, stretto oppure no), diremo che $x_0$ è **punto di estremo** o **estremante** per $f$.

> [!note] Osservazione
> In un punto di estremo per $f$, la funzione può essere continua oppure no; se è continua può essere anche derivabile un certo numero di volte oppure no.

## Esempi
**$f(x)=|x|$** ha minimo (globale stretto) in $x_0=0$; è continua ma non derivabile in $x_0=0$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> Pag. 8: grafico di $|x|$ (due semirette a V con vertice nell'origine). Da cercare sul quaderno/PDF a pag. 8.

**$f(x)=\begin{cases}x+1&x>0\\-x&x\le0\end{cases}$** ha minimo (globale stretto) in $x_0=0$ ed è discontinua in $x_0=0$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> Pag. 8: grafico della funzione a tratti: semiretta decrescente per $x\le0$ che arriva a $f(0)=0$ (pallino pieno) e semiretta crescente per $x>0$ che parte da $(0,1)$ (pallino vuoto). Da cercare a pag. 8.

## Note collegate
- [[137_Teorema_di_Fermat]]
- [[138_Punti_Stazionari_e_Punti_Critici]]
- [[139_Ricerca_di_Massimi_e_Minimi_Assoluti_su_Intervallo_Chiuso]]
- [[20_Funzioni_Limitate_Estremi]]
- [[23_Monotonia]]
- [[112_Teorema_di_Weierstrass]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/estremi
