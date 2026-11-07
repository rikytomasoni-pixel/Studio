---
tags:
  - AM1
  - continuita
  - invertibilita
  - monotonia
  - teorema
data: 2026-11-06
lezione: 16
fonte: "AM1 L16 26-27.pdf (pag. 13-15)"
---

# Continuità e invertibilità

Abbiamo già visto ([[27_Teorema_Monotone_Invertibili]]) che se $f:I\subseteq\mathbb{R}\to\mathbb{R}$ è strettamente monotona allora essa è invertibile e $f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$ è strettamente monotona come $f$.

**Il viceversa non è vero.**

> [!example] Controesempio
> $$f(x)=\begin{cases}x&x\in[0,1)\\3-x&x\in[1,2]\end{cases}\qquad f^{-1}(y)=\begin{cases}y&y\in[0,1)\\3-y&y\in[1,2]\end{cases}$$
> $\operatorname{Im}f=\mathcal{D}(f^{-1})=[0,2]$ e $\mathcal{D}(f)=\operatorname{Im}(f^{-1})=[0,2]$. $f$ è invertibile ma **non è monotona**.
>
> > [!warning] DISEGNO NON RAPPRESENTABILE
> > AM1 L16 pag. 13: grafico di $f$ in rosso: segmento da $(0,0)$ a $(1,1)$ con cerchietto vuoto in $(1,1)$, poi segmento decrescente da $(1,2)$ a $(2,1)$, con punti pieni in $(1,2)$ e $(2,1)$ e $(0,0)$; tratteggi a quote $1$ e $2$.

> [!abstract] Teorema
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo, $f$ **continua** in $I$. Allora
> $$f\text{ strettamente monotona}\iff f\text{ invertibile}$$
> In tal caso $f^{-1}$ è strettamente monotona come $f$, $\operatorname{Im}f=\mathcal{D}(f^{-1})\subseteq\mathbb{R}$ è un intervallo e $f^{-1}:\operatorname{Im}f\subseteq\mathbb{R}\to\mathbb{R}$ è continua sul suo dominio.

> [!abstract] Corollario
> Le funzioni elementari sono continue sui loro domini → [[117_Continuita_delle_Funzioni_Elementari]].

## Note collegate
- [[26_Iniettivita_Suriettivita_Inversa]]
- [[27_Teorema_Monotone_Invertibili]]
- [[113_Teorema_dei_Valori_Intermedi]]
- [[115_Teorema_sui_Limiti_di_Funzioni_Monotone]]
- [[117_Continuita_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]

#AM1/continuita/continuita-e-invertibilita
