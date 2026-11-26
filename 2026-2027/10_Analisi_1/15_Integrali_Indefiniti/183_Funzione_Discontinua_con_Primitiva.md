---
tags:
  - AM1
  - integrali
  - primitive
  - controesempio
  - discontinuita
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 22-23)"
---

# Esistono funzioni discontinue che ammettono primitive

Continuità non è necessaria per avere primitive. Sia
$$F(x)=\begin{cases}x^2\sin\dfrac1x&x\ne0\\[2mm]0&x=0\end{cases}$$
Allora
$$f(x)=F'(x)=\begin{cases}2x\sin\dfrac1x-\cos\dfrac1x&x\ne0\\[2mm]0&x=0\end{cases}$$

- $f$ **ammette primitiva** $F$ in $\mathbb{R}$;
- $f$ è **discontinua** in $x_0=0$, punto di discontinuità di **II specie** ([[98_Discontinuita_di_Seconda_Specie]]): $\cos\frac1x$ non ha limite per $x\to0$.

È coerente con [[182_Funzione_a_Salto_senza_Primitive]]: una derivata può avere solo discontinuità di II specie.

## Note collegate
- [[181_Primitiva_di_una_Funzione]]
- [[182_Funzione_a_Salto_senza_Primitive]]
- [[151_Discontinuita_della_Funzione_Derivata]]
- [[98_Discontinuita_di_Seconda_Specie]]
- [[00_MOC_Analisi_1]]

#AM1/integrali/primitiva-discontinua
