---
tags: [GAL, spazi-vettoriali, combinazioni-lineari, span, lezione-13]
data: 2026-10-19
lezione: 13
fonte: "GAL_2026-2027_-_20261019_-_LEZIONE_13.pdf (slide 109-110)"
---

# Combinazioni lineari e span

> [!question] Domanda guida
> Come si descrivono e si manipolano gli elementi di uno spazio vettoriale?

> [!abstract] Definizione 13.1
> Sia $(V,+,\cdot)$ uno spazio vettoriale su un campo $\mathbb{K}$. Sia $\underline{v}_1,\dots,\underline{v}_n$ una collezione finita di elementi di $V$.
> - Una **combinazione lineare** di $\underline{v}_1,\dots,\underline{v}_n$ è un vettore della forma
>   $$\lambda_1\underline{v}_1+\lambda_2\underline{v}_2+\dots+\lambda_n\underline{v}_n\qquad\lambda_1,\dots,\lambda_n\in\mathbb{K}$$
> - L'insieme di tutte le combinazioni lineari di $\underline{v}_1,\dots,\underline{v}_n$ si dice **sottospazio vettoriale generato** da $\underline{v}_1,\dots,\underline{v}_n$ (o **linear span**) e si denota con $\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$.

## Osservazioni
- $\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)=\{\underline{v}\in V\mid \underline{v}=\lambda_1\underline{v}_1+\dots+\lambda_n\underline{v}_n,\ \lambda_i\in\mathbb{K}\}$
- L'insieme delle combinazioni lineari è **chiuso** rispetto a somma e prodotto per scalari (quindi è davvero un sottospazio, vedi [[94_Sottospazi_Vettoriali]]).

> [!todo] Verifica per casa
> Verificare la chiusura di $\operatorname{Span}(\underline{v}_1,\dots,\underline{v}_n)$ rispetto a somma e prodotto per scalari.

## Esempi

### Polinomi
Sia $p(t)\in\mathbb{K}[t]_{\leq d}$, cioè $p(t)=a_0+a_1t+a_2t^2+\dots+a_dt^d$. Con $1,t,t^2,\dots,t^d\in\mathbb{K}[t]_{\leq d}$:
- $a_0+a_1t+\dots+a_dt^d$ è una combinazione lineare di $1,t,\dots,t^d$;
- quindi $p(t)\in\operatorname{Span}(1,t,\dots,t^d)$.

### Sistema lineare (rappresentazione del I tipo)
Per un sistema lineare $A\underline{x}=\underline{b}$ la [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare|rappresentazione del I tipo]] è
$$x_1\,C_1(A)+x_2\,C_2(A)+\dots+x_n\,C_n(A)=\underline{b}$$
dove $C_j(A)$ è la $j$-esima colonna di $A$.

> [!tip] Interpretazione
> Avere un sistema risolubile equivale a poter scrivere $\underline{b}$ come combinazione lineare delle colonne di $A$, cioè $\underline{b}\in\operatorname{Span}(C_1(A),\dots,C_n(A))$.

## Note collegate
- [[91_Spazio_Vettoriale_Definizione]]
- [[94_Sottospazi_Vettoriali]]
- [[80_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]
- [[82_Teorema_di_Rouche_Capelli]]
- Successiva: [[96_Insieme_di_Generatori]]
- Indice: [[14_Indice_Lezione_13]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/span
