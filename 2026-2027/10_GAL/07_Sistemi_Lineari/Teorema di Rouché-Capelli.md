---
created: 2026-10-12
materia: GAL
tags:
  - materia/gal
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/sistemi_lineari
aliases: []
---
[[00_GAL_Sistemi_Lineari|⬅️ Torna a Sistemi Lineari]]

# Teorema di Rouché-Capelli

### Teorema 9.1 (Teorema di Rouché-Capelli)

- **HP**: sia $A\underline{x} = \underline{b}$ un sistema lineare, $A \in M_{\mathbb{K}}(m,n)$.
- **TH1**: il sistema $A\underline{x} = \underline{b}$ è risolubile se, e solo se,

  $$r(A) = r([A \mid \underline{b}])$$

- **TH2**: se $r = r(A) = r([A \mid \underline{b}])$, allora esistono $n - r + 1$ vettori colonna $\underline{v}_0, \underline{v}_1, \dots, \underline{v}_{n-r} \in \mathbb{K}^n$ tali che tutte e sole le soluzioni del sistema sono descritte da

  $$\underline{x} = \underline{v}_0 + t_1\underline{v}_1 + \dots + t_{n-r}\underline{v}_{n-r}$$

  dove $t_1,\dots,t_{n-r} \in \mathbb{K}$ (**parametri liberi**).

---
Precedente: [[Risoluzione di un Sistema con il MEG]] · Successivo: [[Dimostrazione di Rouché-Capelli]]
