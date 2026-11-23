---
tags:
  - AM1
  - derivate-successive
  - convessita
  - retta-tangente
  - teorema
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 8-9)"
---

# Convessità e rette tangenti

> [!abstract] Teorema
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$, $I$ intervallo, $f$ derivabile in $I$. Allora $f$ è **convessa** (**concava**) in $I$ se e solo se
> $$f(x)\ge f(x_0)+f'(x_0)(x-x_0)\qquad(\le)\qquad\forall x\in I,\ \forall x_0\in I$$

Cioè $f$ giace interamente **sopra** (**sotto**) la retta tangente al suo grafico in $P_0=(x_0,f(x_0))$, per ogni $x_0\in I$. La retta tangente è $y=f'(x_0)(x-x_0)+f(x_0)$ (vedi [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]).

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Pag. 8:** grafico di una funzione convessa $f$ con punto $P_0=(x_0,f(x_0))$ sul grafico, $f(x_0)$ e $x_0$ segnati sugli assi, e in rosso la retta tangente $y=f'(x_0)(x-x_0)+f(x_0)$ che sta tutta sotto il grafico.

> [!note] Osservazione
> $f(x)=|x|$ è convessa in $\mathbb{R}$ anche se non è derivabile in $x_0=0$ ($x_0$ punto angoloso): l'ipotesi di derivabilità serve solo per scrivere la retta tangente nell'enunciato.

## Note collegate
- [[156_Funzioni_Convesse_e_Concave]]
- [[159_Interpretazione_Geometrica_della_Convessita]]
- [[160_Teorema_di_Regolarita_delle_Funzioni_Convesse]]
- [[162_Test_di_Convessita]]
- [[163_Punti_di_Flesso]]
- [[130_Classificazione_dei_Punti_di_Non_Derivabilita]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/convessita
