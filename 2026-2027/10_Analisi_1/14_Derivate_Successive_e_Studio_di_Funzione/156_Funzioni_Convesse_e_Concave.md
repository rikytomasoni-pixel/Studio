---
tags:
  - AM1
  - derivate-successive
  - convessita
  - definizione
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 26)"
---

# Funzioni concave e convesse

> [!abstract] Definizione (funzione convessa)
> $f:I\subseteq\mathbb{R}\to\mathbb{R}$ con $I$ intervallo si dice **convessa** in $I$ se
> $$\forall x_0,x_1\in I,\ \forall t\in[0,1]\qquad f(tx_1+(1-t)x_0)\le t\,f(x_1)+(1-t)\,f(x_0)$$
> La funzione si dice **strettamente convessa** se
> $$\forall x_0,x_1\in I,\ x_0\ne x_1,\ \forall t\in(0,1)\qquad f(tx_1+(1-t)x_0)<t\,f(x_1)+(1-t)\,f(x_0)$$

> [!abstract] Definizione (funzione concava)
> La funzione $f$ si dice (strettamente) **concava** se $-f$ è (strettamente) convessa.

> [!note] Osservazione (non presente negli appunti)
> Geometricamente, $tx_1+(1-t)x_0$ descrive i punti del segmento $[x_0,x_1]$ e $t f(x_1)+(1-t)f(x_0)$ i punti della corda tra $(x_0,f(x_0))$ e $(x_1,f(x_1))$: $f$ è convessa se il grafico sta sempre **sotto** ogni sua corda.

> [!info] Sviluppi (L20)
> Interpretazione con le corde: [[159_Interpretazione_Geometrica_della_Convessita]] (preliminari: [[158_Segmento_e_Retta_per_due_Punti]]). Regolarità: [[160_Teorema_di_Regolarita_delle_Funzioni_Convesse]]. Caratterizzazioni: [[161_Convessita_e_Rette_Tangenti]] (rette tangenti) e [[162_Test_di_Convessita]] (monotonia di $f'$, segno di $f''$). Flessi: [[163_Punti_di_Flesso]], [[164_Punti_di_Cambio_di_Concavita]], [[165_Flessi_e_Derivata_Seconda]]. Nello [[157_Studio_del_Grafico_di_una_Funzione|studio del grafico]] la convessità si studia con il segno di $f''$.

## Note collegate
- [[157_Studio_del_Grafico_di_una_Funzione]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[140_Test_di_Monotonia]]
- [[158_Segmento_e_Retta_per_due_Punti]]
- [[159_Interpretazione_Geometrica_della_Convessita]]
- [[160_Teorema_di_Regolarita_delle_Funzioni_Convesse]]
- [[161_Convessita_e_Rette_Tangenti]]
- [[162_Test_di_Convessita]]
- [[163_Punti_di_Flesso]]
- [[164_Punti_di_Cambio_di_Concavita]]
- [[165_Flessi_e_Derivata_Seconda]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/convessita
