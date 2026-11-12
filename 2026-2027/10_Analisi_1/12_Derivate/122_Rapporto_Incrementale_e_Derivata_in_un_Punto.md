---
tags:
  - AM1
  - derivate
  - definizione
  - rapporto-incrementale
  - retta-tangente
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 6-10, 14)"
---

# Rapporto incrementale e derivata in un punto

## Costruzione
Sia $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$ e $h\in\mathbb{R}$, $h\neq0$, con $|h|$ piccolo affinché $x_0+h\in(a,b)$. Consideriamo i due punti
$$P_0=(x_0,f(x_0)),\qquad P_h=(x_0+h,f(x_0+h))$$
sul grafico di $f$ ($P_h$ è a destra/sinistra di $P_0$ a seconda che sia $h>0$ / $h<0$).

> [!warning] DISEGNO NON RAPPRESENTABILE
> **AM1 L17, pag. 7**: grafico di una funzione con i punti $P_0$ e $P_h$ e la retta secante $r_h$ (in rosso) che passa per entrambi. In blu sono indicati $\Delta x=h$ (segmento orizzontale da $x_0$ a $x_0+h$) e $\Delta f=f(x_0+h)-f(x_0)$ (segmento verticale).

La retta per $P_0,P_h$ ha coefficiente angolare
$$m_h=\frac{\Delta f}{\Delta x}=\frac{f(x_0+h)-f(x_0)}{h}$$
$m_h$ è la "pendenza media" del grafico di $f$ nel segmento di estremi $x_0,x_0+h$.

Per $h\to0$, $P_h$ si sposta sul grafico di $f$ (verso $P_0$ se $f$ è continua in $x_0$, ma non sarà necessario chiederlo a priori). Contestualmente $m_h$ varia e può accadere che, al tendere di $h\to0$, essa tenda a un valore limite finito. In tal caso la retta individuata da $P_0,P_h$ si stabilizza su una posizione limite per $h\to0$. Vogliamo definire tale retta come la **retta tangente** al grafico di $f$ in $P_0$.

## Definizioni
> [!abstract] Definizione — rapporto incrementale
> Sia $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, $h\in\mathbb{R}\setminus\{0\}$ con $x_0+h\in(a,b)$. Allora
> $$\frac{f(x_0+h)-f(x_0)}{h}$$
> viene chiamato **rapporto incrementale** di $f$ in $x_0$ con incremento $h$.

> [!abstract] Definizione — derivabilità e derivata prima
> Data $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, diremo che $f$ è **derivabile in $x_0$** se esiste **finito**
> $$\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}\in\mathbb{R}$$
> Tale limite si chiama **derivata prima** di $f$ in $x_0$ e si indica con
> $$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}\in\mathbb{R}$$

Notazioni: $f'(x_0)$, $\dfrac{df}{dx}(x_0)$, $Df(x_0)$, $\dot f(x_0)$.

> [!note] Osservazione — forma equivalente
> Con il cambio di variabile $x-x_0=h$ ([[104_Cambio_di_Variabile_nei_Limiti]])
> $$f'(x_0)=\lim_{h\to0}\frac{f(x_0+h)-f(x_0)}{h}=\lim_{x\to x_0}\frac{f(x)-f(x_0)}{x-x_0}$$

> [!abstract] Definizione — retta tangente
> Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$ e $f$ è derivabile in $x_0$, si definisce **retta tangente al grafico di $f$ in $P_0=(x_0,f(x_0))$** la retta
> $$y=f'(x_0)(x-x_0)+f(x_0)$$

## Derivata destra e sinistra
> [!abstract] Definizione — derivata destra e sinistra
> $$f'_+(x_0)=\lim_{h\to0^+}\frac{f(x_0+h)-f(x_0)}{h}\qquad f'_-(x_0)=\lim_{h\to0^-}\frac{f(x_0+h)-f(x_0)}{h}$$
> Se tali limiti esistono finiti, le rette
> $$y=f'_+(x_0)(x-x_0)+f(x_0)\qquad y=f'_-(x_0)(x-x_0)+f(x_0)$$
> prendono il nome di **retta tangente al grafico di $f$ in $P_0=(x_0,f(x_0))$ da destra / da sinistra**.

Il collegamento con i limiti destro e sinistro è quello di [[91_Limiti_Destro_e_Sinistro_e_Asintoto_Verticale]].

## Note collegate
- [[121_Problemi_Motivanti_delle_Derivate]]
- [[123_Esempi_di_Derivata_e_Retta_Tangente]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[125_Derivata_Infinita_e_Tangente_Verticale]]
- [[129_Derivabilita_e_Continuita]]
- [[93_Continuita_in_un_Punto]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/definizione
