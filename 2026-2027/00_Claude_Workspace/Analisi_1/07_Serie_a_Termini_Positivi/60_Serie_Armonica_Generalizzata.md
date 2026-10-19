---
tags:
  - AM1
  - serie
  - serie-armonica-generalizzata
  - serie-geometrica
  - serie-a-termini-positivi
data: 2026-10-16
fonte: "AM1 L11 26-27.pdf (pag. 8)"
stato: da_verificare
destinazione: 10_Analisi_1/07_Serie_a_Termini_Positivi (cartella nuova)
---

# Serie armonica generalizzata (e richiamo serie geometrica)

## Serie armonica generalizzata
$$\sum_{n=1}^\infty\frac1{n^\alpha}=\begin{cases}\text{converge}&\alpha>1\\[1mm]\text{diverge}&\alpha\leq1\end{cases}$$

> [!note] Dimostrazione
> La dimostrazione si fa col **criterio del confronto integrale**, più in là nel corso. (Per $\alpha=1$ vedi già [[55_Serie_Armonica]].)

## Richiamo: serie geometrica con $q\geq0$
$$\sum_{n=0}^\infty q^n=\begin{cases}\text{converge a }\dfrac1{1-q}&0\leq q<1\\[2mm]\text{diverge a }+\infty&q\geq1\end{cases}$$

> [!warning] Nota sull'indice
> Negli appunti manoscritti la somma parte da $n=1$, ma il valore $\frac1{1-q}$ è quello della serie da $n=0$ (vedi [[50_Serie_Geometrica]]). Il carattere (converge/diverge) non cambia; da $n=1$ la somma sarebbe $\frac q{1-q}$. **Da verificare sul quaderno.**

Queste serie sono i termini di confronto più usati per il [[58_Criterio_del_Confronto_per_Serie]] e il [[62_Criterio_del_Confronto_Asintotico_per_Serie]].

## Note collegate
- [[55_Serie_Armonica]]
- [[50_Serie_Geometrica]]
- [[61_Serie_di_Bertrand_Generalizzata]]
- [[59_Esempio_Confronto_Serie_18_cos_n]]
- [[63_Esempio_Confronto_Asintotico_con_Parametro]]
- [[00_MOC_Analisi_1]]

#AM1/serie/serie-armonica-generalizzata
