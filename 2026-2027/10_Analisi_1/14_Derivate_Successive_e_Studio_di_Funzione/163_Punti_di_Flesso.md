---
tags:
  - AM1
  - derivate-successive
  - flesso
  - definizione
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 10-11)"
---

# Punti di flesso

> [!abstract] Definizione (punto di flesso)
> Data $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, $f$ **derivabile** in $x_0$. Allora $x_0$ è **punto di flesso** per $f$ se esiste $\delta>0$ tale che
> $$f(x)\ge f(x_0)+f'(x_0)(x-x_0)\ \text{ in }[x_0,x_0+\delta)\qquad\text{e}\qquad f(x)\le f(x_0)+f'(x_0)(x-x_0)\ \text{ in }(x_0-\delta,x_0]$$
> oppure con le disuguaglianze invertite ($\le$ a destra di $x_0$, $\ge$ a sinistra).

In parole: la retta tangente in $x_0$ **attraversa** il grafico (da una parte sta sotto, dall'altra sopra).

![[puntiFlesso.png]]

> [!note] Osservazione (abuso di notazione)
> Per estensione, se $f$ è continua in $x_0$ e $f'(x_0)=\pm\infty$, con retta tangente verticale $x=x_0$, si dice ancora che $x_0$ è punto di flesso per $f$ (**a tangente verticale**): vedi [[125_Derivata_Infinita_e_Tangente_Verticale]] e [[130_Classificazione_dei_Punti_di_Non_Derivabilita]].

## Note collegate
- [[164_Punti_di_Cambio_di_Concavita]]
- [[165_Flessi_e_Derivata_Seconda]]
- [[161_Convessita_e_Rette_Tangenti]]
- [[156_Funzioni_Convesse_e_Concave]]
- [[125_Derivata_Infinita_e_Tangente_Verticale]]
- [[130_Classificazione_dei_Punti_di_Non_Derivabilita]]
- [[157_Studio_del_Grafico_di_una_Funzione]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/flesso
