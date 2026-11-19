---
tags:
  - AM1
  - derivate
  - teorema
  - dimostrazione
  - discontinuita
  - prolungamento-derivata
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 24-25)"
---

# Discontinuità della funzione derivata

> [!abstract] Corollario
> Sia $f:I\subseteq\mathbb{R}\to\mathbb{R}$ con $I$ intervallo. Supponiamo che esista $f':I\to\mathbb{R}$ (cioè $f$ derivabile in $x$ per ogni $x\in I$). Allora $f'$ può avere in $I$ solo punti di discontinuità di **II specie** (no discontinuità eliminabili, no discontinuità a salto).

**Dimostrazione.** Poiché $f$ è derivabile in $x_0$ per ogni $x_0\in I$, cioè esiste $f'(x_0)\in\mathbb{R}$ per ogni $x_0\in I$, per il [[148_Teorema_di_Prolungamento_della_Derivata_Prima|teorema di prolungamento della derivata prima]], se esistono
$$\lim_{x\to x_0^+}f'(x),\qquad\lim_{x\to x_0^-}f'(x)$$
essi devono coincidere necessariamente con (rispettivamente) $f'_+(x_0)$ e $f'_-(x_0)$. Se $x_0$ è punto interno, inoltre, essi devono coincidere con $f'(x_0)$.

In particolare non sono ammesse
- **discontinuità eliminabili** ([[96_Discontinuita_Eliminabile_e_Prolungamento_per_Continuita]]): i limiti da destra e da sinistra esistono finiti e uguali, ma diversi da $f'(x_0)$;
- **discontinuità a salto** ([[97_Discontinuita_di_Prima_Specie_a_Salto]]): i limiti da destra e da sinistra esistono finiti ma diversi tra loro. $\square$

Rimangono possibili solo discontinuità di seconda specie ([[98_Discontinuita_di_Seconda_Specie]]), come nell'esempio $x^2\sin\frac1x$ di [[150_Osservazioni_sul_Prolungamento_della_Derivata]], dove $f'$ è discontinua in $0$ perché $\cos\frac1x$ non ha limite.

## Note collegate
- [[148_Teorema_di_Prolungamento_della_Derivata_Prima]]
- [[150_Osservazioni_sul_Prolungamento_della_Derivata]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[96_Discontinuita_Eliminabile_e_Prolungamento_per_Continuita]]
- [[97_Discontinuita_di_Prima_Specie_a_Salto]]
- [[98_Discontinuita_di_Seconda_Specie]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/discontinuita-derivata
