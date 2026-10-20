---
tags: [GAL, spazi-vettoriali, generatori, span, lezione-13]
data: 2026-10-19
lezione: 13
fonte: "GAL_2026-2027_-_20261019_-_LEZIONE_13.pdf (slide 110-111)"
stato: da-revisionare
destinazione: "20_Geometria_Algebra_Lineare/13_Spazi_Vettoriali"
---

# Insieme di generatori

> [!abstract] Definizione 13.2
> Sia $(V,+,\cdot)$ uno spazio vettoriale su un campo $\mathbb{K}$. Un insieme di vettori $\{\underline{v}_1,\dots,\underline{v}_n\}$ si dice **insieme di generatori** di $V$ se
> $$V=\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$$

> [!note] N.B.
> $\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)\subseteq V$ è **sempre vero**. Quindi "essere generatori" equivale a
> $$V\subseteq\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$$

Vedi [[95_Combinazioni_Lineari_e_Span]] per la definizione di span.

## Esempi

### Polinomi
Per ogni $p(t)=a_0+a_1t+\dots+a_dt^d\in\mathbb{K}[t]_{\leq d}$ si ha $p(t)\in\operatorname{Span}(1,t,\dots,t^d)$, quindi
$$\mathbb{K}[t]_{\leq d}\subseteq\operatorname{Span}(1,t,\dots,t^d)$$
e $\{1,t,\dots,t^d\}$ è un insieme di generatori di $\mathbb{K}[t]_{\leq d}$.

### Nucleo di una matrice
Sia $A\in M_{\mathbb{K}}(m,n)$ e $\ker(A)=\{\underline{x}\in\mathbb{K}^n\mid A\underline{x}=\underline{0}\}$. Il [[82_Teorema_di_Rouche_Capelli|teorema di Rouché-Capelli]] dice che le soluzioni sono del tipo
$$\underline{x}=\underline{0}+t_1\underline{v}_1+\dots+t_{n-r}\underline{v}_{n-r}$$
che è una combinazione lineare. Dunque $\ker(A)=\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_{n-r})$ (vedi [[84_Nucleo_e_Sistema_Omogeneo_Associato]]).

In generale $\ker(A)\subsetneq\mathbb{K}^n$, quindi $\{\underline{v}_1,\dots,\underline{v}_{n-r}\}$ **non** sono generatori di $\mathbb{K}^n$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** slide 111, a metà pagina. **Cosa cercare:** un grande ovale $\mathbb{K}^n$ che contiene un ovale rosso più piccolo $\ker(A)$; fuori dall'ovale rosso ma dentro quello grande c'è un vettore $\underline{w}$ (blu), che non è generato dai vettori del nucleo.

### Retta per l'origine in $\mathbb{R}^3$
Sia $n=3$, $\mathbb{R}^3$ spazio euclideo, $r$ una retta passante per l'origine:
$$r=\left\{\begin{bmatrix}x\\y\\z\end{bmatrix}=t\,\underline{v}\ \middle|\ t\in\mathbb{R}\right\}=\operatorname{Span}(\underline{v})$$
$\underline{v}$ è un generatore della retta ma **non** è un generatore di $\mathbb{R}^3$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> **Dove:** slide 111, a destra di "$n=3$". **Cosa cercare:** piccolo schizzo di tre assi cartesiani di $\mathbb{R}^3$.

## Note collegate
- [[95_Combinazioni_Lineari_e_Span]]
- [[94_Sottospazi_Vettoriali]]
- [[84_Nucleo_e_Sistema_Omogeneo_Associato]]
- [[82_Teorema_di_Rouche_Capelli]]
- Successiva: [[97_Esempio_Generatori_di_R3_e_Rappresentazioni_Multiple]]
- Indice: [[14_Indice_Lezione_13]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/generatori
