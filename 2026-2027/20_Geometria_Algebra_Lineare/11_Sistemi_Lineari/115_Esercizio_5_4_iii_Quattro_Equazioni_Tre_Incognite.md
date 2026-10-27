---
tags: [GAL, sistemi-lineari, esercizio, parametri, eliminazione]
data: 2026-10-27
lezione: esercizi
fonte: "Esercizio 5.4 (iii); svolgimento redatto da Claude, non presente negli appunti"
---

# Esercizio 5.4 (iii): quattro equazioni in tre incognite

> [!question] Sistema
> $$\begin{cases}x_1+x_2+ax_3=1\\ x_1+x_2+a^3x_3=3\\ 2x_1+x_2+2x_3=0\\ x_1+x_2+x_3=0\end{cases}$$

La matrice dei coefficienti è $4\times3$: non è quadrata, quindi non ha senso il determinante. Si procede per eliminazione, usando l'equazione 4 (senza parametro) come riferimento.

## 1. Sottraggo l'equazione 4 dalle altre
- eq.1 $-$ eq.4: $(a-1)x_3=1$
- eq.2 $-$ eq.4: $(a^3-1)x_3=3$
- eq.3 $-$ eq.4: $x_1+x_3=0\Rightarrow x_1=-x_3$

Dall'equazione 4: $x_2=-x_1-x_3=0$.

## 2. Discussione
- $a=1$: la prima diventa $0=1$, **nessuna soluzione**.
- $a\neq1$: $x_3=\dfrac{1}{a-1}$. Dalla seconda, con $a^3-1=(a-1)(a^2+a+1)$:
$$a^2+a+1=3\Rightarrow a^2+a-2=0\Rightarrow(a+2)(a-1)=0$$
$a=1$ è già escluso, resta $a=-2$.

## 3. Verifica con $a=-2$
$x_3=-\tfrac13$, $x_1=\tfrac13$, $x_2=0$:
- eq.1: $\tfrac13+\tfrac23=1$ ✓
- eq.2: $\tfrac13+\tfrac83=3$ ✓
- eq.3: $\tfrac23-\tfrac23=0$ ✓
- eq.4: $\tfrac13-\tfrac13=0$ ✓

> [!success] Risultato
> Soluzioni $\iff a=-2$, e in tal caso la soluzione è **unica**: $(x_1,x_2,x_3)=\left(\tfrac13,\,0,\,-\tfrac13\right)$ ($r(A)=3$, nessun parametro libero: [[82_Teorema_di_Rouche_Capelli]]).

## Note collegate
- [[112_Esercizio_5_4_Sistemi_con_Parametro]]
- [[68_Metodo_di_Eliminazione_di_Gauss]]
- [[82_Teorema_di_Rouche_Capelli]]

#GAL/sistemi-lineari/esercizio-5-4
