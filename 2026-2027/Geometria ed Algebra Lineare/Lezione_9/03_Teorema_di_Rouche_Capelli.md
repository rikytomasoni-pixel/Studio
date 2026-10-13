---
tags: [GAL, sistemi-lineari, teorema, rouche-capelli, rango, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL 2026-2027 - 20261012 - LEZIONE 9.pdf (slide 78)"
---

# Teorema di Rouché-Capelli

> [!abstract] Teorema 9.1 (Teorema di Rouché-Capelli)
> **Ipotesi.** Sia $A\underline{x}=\underline{b}$ un sistema lineare, $A\in M_{\mathbb{K}}(m,n)$.
>
> **Tesi 1.** Il sistema $A\underline{x}=\underline{b}$ è risolubile se, e solo se,
> $$r(A)=r(A\,|\,\underline{b})$$
>
> **Tesi 2.** Se $r=r(A)=r(A\,|\,\underline{b})$, allora esistono $n-r+1$ vettori colonna $\underline{v}_0,\underline{v}_1,\dots,\underline{v}_{n-r}\in\mathbb{K}^n$ tali che tutte e sole le soluzioni del sistema sono descritte da
> $$\underline{x}=\underline{v}_0+t_1\underline{v}_1+\cdots+t_{n-r}\underline{v}_{n-r}$$
> dove $t_1,\dots,t_{n-r}\in\mathbb{K}$ (parametri liberi).

Dimostrazione: [[04_Dimostrazione_del_Teorema_di_Rouche_Capelli]].

> [!note] Lettura del teorema (commento aggiunto, non presente nelle slide)
> - Il numero di parametri liberi è $n-r$ (numero di incognite meno rango); se $r=n$ non ci sono parametri e la soluzione è unica ($\underline{x}=\underline{v}_0$).
> - $\underline{v}_0$ è la **parte costante** della soluzione (indicata così nelle slide).

### Note collegate
- [[00_Indice_Lezione_9]] · [[00_MOC_GAL]]
- [[04_Dimostrazione_del_Teorema_di_Rouche_Capelli]]
- [[04_Rango_di_una_Matrice]] — rango
- [[04_MEG_e_Rango]] — calcolo del rango con il MEG
- [[02_Risoluzione_di_un_Sistema_con_il_MEG]] — esempio
