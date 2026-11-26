---
tags: [GAL, diagonalizzabilita, autovalori, molteplicita, teorema, criterio, dimostrazione, lezione-26]
data: 2026-11-26
lezione: 26
fonte: "GAL 2026-2027 - 20261126 - LEZIONE 26.pdf (slide 212)"
---

# Teorema 26.3: secondo criterio di diagonalizzabilità

> [!abstract] Teorema 26.3 (secondo criterio di diagonalizzabilità)
> Sia $A\in M_{\mathbb{K}}(n,n)$. Le seguenti affermazioni sono tra loro equivalenti:
> - **(I)** $A$ è diagonalizzabile su $\mathbb{K}$;
> - **(II)**
>   - $\chi_A(x)$ ha $n$ radici in $\mathbb{K}$ (contate con la loro molteplicità), cioè
>     $$a_{\lambda_1}+a_{\lambda_2}+\dots+a_{\lambda_s}=n$$
>   - per ogni autovalore $\lambda_i$, $\;g_{\lambda_i}=a_{\lambda_i}$.

## Dimostrazione

Negli esempi e per le proprietà viste finora, ciò che sono in grado di trovare sono
$$g_{\lambda_1}+g_{\lambda_2}+\dots+g_{\lambda_s}$$
autovettori **linearmente indipendenti** ([[187_Autospazi_di_Autovalori_Distinti_e_Somma_Diretta]]). Vale la catena
$$g_{\lambda_1}+\dots+g_{\lambda_s}\ \overset{(\star)}{\le}\ a_{\lambda_1}+\dots+a_{\lambda_s}\ \overset{(\star\star)}{\le}\ n$$
dove $(\star)$ segue da $g_\lambda\le a_\lambda$ ([[186_Definizione_26_2_Molteplicita_Algebrica_Autospazio_Molteplicita_Geometrica]]) e $(\star\star)$ dal fatto che $\chi_A$ ha grado $n$ ([[185_Definizione_26_1_Polinomio_Caratteristico]]).

Per il [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita|primo criterio]]:
$$A\text{ diagonalizzabile su }\mathbb{K}\ \overset{\text{primo criterio}}{\iff}\ g_{\lambda_1}+\dots+g_{\lambda_s}=n$$

- La **prima condizione** $a_{\lambda_1}+\dots+a_{\lambda_s}=n$ garantisce l'uguaglianza nella seconda parte $(\star\star)$.
- La **seconda condizione** $g_{\lambda_i}=a_{\lambda_i}\ \forall i$ garantisce l'uguaglianza nella prima parte $(\star)$.

Quindi (II) $\iff g_{\lambda_1}+\dots+g_{\lambda_s}=n\iff$ (I). $\square$

> [!tip] In pratica
> Per decidere se $A$ è diagonalizzabile su $\mathbb{K}$: (1) calcolo $\chi_A$ e controllo che si spezzi in fattori lineari su $\mathbb{K}$; (2) per ogni autovalore confronto $g_\lambda$ con $a_\lambda$ ([[189_Autovalori_Semplici_e_Regolari]]).

## Note collegate
- [[178_Teorema_25_2_Primo_Criterio_di_Diagonalizzabilita]]
- [[185_Definizione_26_1_Polinomio_Caratteristico]]
- [[186_Definizione_26_2_Molteplicita_Algebrica_Autospazio_Molteplicita_Geometrica]]
- [[187_Autospazi_di_Autovalori_Distinti_e_Somma_Diretta]]
- [[189_Autovalori_Semplici_e_Regolari]]
- Indice: [[27_Indice_Lezione_26]] · [[00_MOC_GAL]]

#GAL/diagonalizzabilita/secondo-criterio
