---
tags:
  - AM1
  - derivate
  - teorema
  - dimostrazione
  - prolungamento-derivata
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 23-24)"
---

# Dimostrazione del teorema di prolungamento della derivata prima

Teorema: [[148_Teorema_di_Prolungamento_della_Derivata_Prima]]. Si applica il [[142_Teorema_di_Lagrange|teorema del valor medio di Lagrange]].

**Dimostrazione.** Sia $h>0$ piccolo in modo che $a+h\in(a,b)$. Applichiamo il teorema di Lagrange alla funzione $f$ in $[a,a+h]$.

Osserviamo che $[a,a+h]\subset[a,b)$ e $f$ è continua in $[a,b)$, derivabile in $(a,b)$ $\Rightarrow$ $f$ è continua in $[a,a+h]$, derivabile in $(a,a+h)$.

Per Lagrange esiste $c_h\in(a,a+h)$ tale che
$$\frac{f(a+h)-f(a)}{h}=f'(c_h)$$
Poiché $a<c_h<a+h$, per il teorema dei due carabinieri ([[100_Teorema_del_Confronto_per_Limiti_di_Funzioni]]) vale
$$\lim_{h\to0^+}c_h=a^+$$
Pertanto
$$\lim_{h\to0^+}\frac{f(a+h)-f(a)}{h}=\lim_{h\to0^+}f'(c_h)\overset{t=c_h}{=}\lim_{t\to a^+}f'(t)=m\in\overline{\mathbb{R}}$$
dove si è usato il [[104_Cambio_di_Variabile_nei_Limiti|teorema di cambio di variabile nei limiti]] con $t=c_h$. Quindi
$$\exists\ f'_+(a)=\lim_{h\to0^+}\frac{f(a+h)-f(a)}{h}=m\in\overline{\mathbb{R}}\qquad\square$$

## Note collegate
- [[148_Teorema_di_Prolungamento_della_Derivata_Prima]]
- [[142_Teorema_di_Lagrange]]
- [[100_Teorema_del_Confronto_per_Limiti_di_Funzioni]]
- [[104_Cambio_di_Variabile_nei_Limiti]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/prolungamento-derivata-dimostrazione
