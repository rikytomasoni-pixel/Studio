---
tags:
  - AM1
  - derivate
  - estremi
  - punti-stazionari
  - controesempi
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 10-12)"
---

# Punti stazionari (o critici)

> [!abstract] Definizione (punto critico o stazionario)
> Se $f$ è derivabile in $x_0\in(a,b)$ e se $f'(x_0)=0$, diremo che $x_0$ è punto **critico** o **stazionario** per $f$.

Per il [[137_Teorema_di_Fermat]], un punto di estremo in cui $f$ è derivabile è stazionario. Il viceversa è falso.

> [!note] Osservazione
> Esistono funzioni derivabili con $f'(x_0)=0$ in un punto $x_0$ che **non** è punto di estremo per $f$.

## Esempio: $f(x)=x^3$ in $\mathbb{R}$
$f'(x)=3x^2$ per ogni $x\in\mathbb{R}$ e $f'(0)=0$. Tuttavia $f$ è strettamente crescente in $\mathbb{R}$, quindi non ha né massimi né minimi.

![[GraficoxCubo.png|303]]

> [!note] Osservazione
> Esistono funzioni derivabili che hanno punti stazionari che non sono né massimi, né minimi, né flessi a tangente orizzontale.

## Esempio: $f(x)=\begin{cases}x^2\sin\frac1x&x\neq0\\0&x=0\end{cases}$
$$f'(x)=\begin{cases}2x\sin\frac1x-\cos\frac1x&x\neq0\\0&x=0\end{cases}$$
Infatti
$$f'(0)=\lim_{h\to0}\frac{f(h)-f(0)}{h}=\lim_{h\to0}\frac{h^2\sin\frac1h}{h}=\lim_{h\to0}h\sin\frac1h=0$$
$f$ è derivabile in $\mathbb{R}$ e $f'(0)=0$, quindi $x_0=0$ è punto stazionario; ma $x_0=0$ non è né massimo, né minimo, né flesso.

![[xquadratosin1sux.png]]

## Note collegate
- [[137_Teorema_di_Fermat]]
- [[136_Massimi_e_Minimi_Locali_e_Globali]]
- [[123_Esempi_di_Derivata_e_Retta_Tangente]]
- [[139_Ricerca_di_Massimi_e_Minimi_Assoluti_su_Intervallo_Chiuso]]
- [[00_MOC_Analisi_1]]
- [[145_Test_di_Monotonia_Controesempi_e_Osservazioni]]
- [[150_Osservazioni_sul_Prolungamento_della_Derivata]]

#AM1/derivate/punti-stazionari
