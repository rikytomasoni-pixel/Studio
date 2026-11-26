---
tags:
  - AM1
  - taylor
  - polinomio-di-taylor
  - osservazione
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 2-3)"
---

# Derivata del polinomio di Taylor

> [!abstract] Osservazione
> La derivata del [[167_Polinomio_di_Taylor|polinomio di Taylor]] di ordine $n$ di $f$ centrato in $x_0$ è il polinomio di Taylor di ordine $n-1$ di $f'$ centrato in $x_0$.

## Calcolo

$$P_n'(x)=\Big(\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k\Big)'=\sum_{k=1}^n\frac{f^{(k)}(x_0)}{k!}\,k\,(x-x_0)^{k-1}=\sum_{k=1}^n\frac{f^{(k)}(x_0)}{(k-1)!}(x-x_0)^{k-1}$$

Con la sostituzione $j=k-1$:

$$P_n'(x)=\sum_{j=0}^{n-1}\frac{f^{(j+1)}(x_0)}{j!}(x-x_0)^j=\sum_{j=0}^{n-1}\frac{(f')^{(j)}(x_0)}{j!}(x-x_0)^j$$

che è il polinomio di Taylor di ordine $n-1$ di $f'$ in $x_0$.

> [!info] A cosa serve
> È il passaggio chiave della [[170_Dimostrazione_del_Teorema_di_Taylor_con_Resto_di_Peano|dimostrazione per induzione]] del teorema di Taylor con resto di Peano.

## Note collegate
- [[167_Polinomio_di_Taylor]]
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[170_Dimostrazione_del_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/derivata-polinomio
