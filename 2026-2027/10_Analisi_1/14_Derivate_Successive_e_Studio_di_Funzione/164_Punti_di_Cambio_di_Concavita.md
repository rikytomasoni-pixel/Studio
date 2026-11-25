---
tags:
  - AM1
  - derivate-successive
  - flesso
  - convessita
  - definizione
  - controesempio
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 11-13)"
---

# Punti di cambio di concavità

> [!abstract] Definizione (cambio di concavità)
> Data $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, $f$ **continua** in $x_0$. Diremo che $x_0$ è **punto di cambio di concavità** per $f$ se esiste $\delta>0$ tale che $f$ sia convessa in $(x_0-\delta,x_0]$ e $f$ sia concava in $[x_0,x_0+\delta)$ (oppure viceversa: concava a sinistra e convessa a destra).

![[CambioConc.png]]

> [!note] Osservazione
> Nel disegno precedente $x_0$ è punto di cambio di concavità, ma **non è un flesso** per $f$ (non esiste retta tangente in $(x_0,f(x_0))$).

## Cambio di concavità e flesso

> [!important] Cambio di concavità $\Rightarrow$ flesso, se $f$ è derivabile
> Se $f:(a,b)\to\mathbb{R}$ è derivabile in $x_0\in(a,b)$ e se $x_0$ è un punto di cambio di concavità, allora $x_0$ è un punto di flesso. (Vedi [[163_Punti_di_Flesso]]; il viceversa è falso.)

## Controesempio al viceversa

$$f(x)=\begin{cases}\left(2+\sin\dfrac1x\right)x^3 & x\ne0\\[2mm] 0 & x=0\end{cases}$$

Si ha $f(0)=0$ e $f'(0)=0$, quindi $y=0$ è la retta tangente in $(0,0)$. Inoltre $f(x)>0$ se $x>0$ e $f(x)<0$ se $x<0$ (il grafico sta tra due curve di tipo cubico, e oscilla tra di esse), quindi $x_0=0$ è **punto di flesso** per $f$, ma **non è punto di cambio di concavità**.

![[graph2+sin1suXperXcubo.png]]

> [!note] Osservazione (non presente negli appunti)
> $f'(0)=0$ segue da $\dfrac{f(h)-f(0)}{h}=(2+\sin\tfrac1h)h^2\to0$. Il motivo per cui non c'è cambio di concavità è che $f'$ oscilla in ogni intorno di $0$ (compare il termine $-x\cos\frac1x$ in $f'$), quindi $f$ non è né convessa né concava in nessun intorno destro o sinistro di $0$.

## Note collegate
- [[163_Punti_di_Flesso]]
- [[165_Flessi_e_Derivata_Seconda]]
- [[156_Funzioni_Convesse_e_Concave]]
- [[162_Test_di_Convessita]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/flesso
