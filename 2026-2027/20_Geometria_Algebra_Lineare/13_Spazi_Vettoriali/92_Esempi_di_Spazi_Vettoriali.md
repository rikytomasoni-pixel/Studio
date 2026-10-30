---
tags: [GAL, spazi-vettoriali, esempi, successioni, funzioni, polinomi, lezione-11]
data: 2026-10-15
lezione: 11
fonte: "GAL_2026-2027_-_20261015_-_LEZIONE_11.pdf (slide 103-104)"
---

# Esempi di spazi vettoriali

Per la definizione vedi [[91_Spazio_Vettoriale_Definizione]].

1. $M_{\mathbb{K}}(m,n)$ è uno spazio vettoriale su $\mathbb{K}$ (operazioni: [[35_Somma_tra_Matrici]], [[36_Prodotto_di_una_Matrice_per_uno_Scalare]]).

2. $V_L=\{\text{vettori liberi}\}$ è uno spazio vettoriale su $\mathbb{R}$ (vedi [[22_Operazioni_tra_Vettori]]).

3. $S=\{\underline{x}\in\mathbb{K}^n\mid A\underline{x}=\underline{0}\}$ è uno spazio vettoriale su $\mathbb{K}$ (vedi [[90_Sistemi_Omogenei_e_Chiusura_della_Somma]]).

4. **Successioni numeriche.** $S=\{\text{successioni numeriche}\}=\{\{a_n\}_{n\in\mathbb{N}}\mid a_n\in\mathbb{R}\}$ è uno spazio vettoriale su $\mathbb{R}$ rispetto alle operazioni
   - $+:\ \{a_n\}_{n\in\mathbb{N}}+\{b_n\}_{n\in\mathbb{N}}=\{a_n+b_n\}_{n\in\mathbb{N}}$
   - $\cdot:\ \lambda\{a_n\}_{n\in\mathbb{N}}=\{\lambda a_n\}_{n\in\mathbb{N}}$

5. **Funzioni.** Sia $I\subseteq\mathbb{R}$ e $V(I)=\{f:I\to\mathbb{R}\}=\mathcal{F}(I,\mathbb{R})$. $V(I)$ è uno spazio vettoriale su $\mathbb{R}$ rispetto alle operazioni
   - $+:\ f,g\in V(I)$, $\ (f+g)(x)=f(x)+g(x)$ *(a sinistra somma di funzioni, a destra somma in $\mathbb{R}$)*
   - $\cdot:\ \lambda\in\mathbb{R}$, $f\in V(I)$, $\ (\lambda f)(x)=\lambda f(x)$

6. **Polinomi.** $\mathbb{K}[t]=\{\text{polinomi nella variabile }t\text{ con coefficienti in }\mathbb{K}\}$, $\ p(t)=\sum a_kt^k$, $a_k\in\mathbb{K}\ \forall k$. Interessano:
   - la somma di polinomi: $p(t)=\sum a_kt^k$, $q(t)=\sum b_kt^k$, $\ p(t)+q(t)=\sum(a_k+b_k)t^k$
   - il prodotto per scalari: $\forall\lambda\in\mathbb{K}$, $\forall p(t)=\sum a_kt^k$: $\ \lambda p(t)=\sum(\lambda a_k)t^k$

Spazi vettoriali contenuti in altri spazi: vedi [[94_Sottospazi_Vettoriali]].

## Note collegate
- [[91_Spazio_Vettoriale_Definizione]]
- [[93_Proprieta_Fondamentali_degli_Spazi_Vettoriali]]
- [[94_Sottospazi_Vettoriali]]
- [[32_Definizione_di_Matrice]]
- [[29_Successioni_Definizioni_Base]] (Analisi 1: successioni)
- [[19_Funzioni_Generalità]] (Analisi 1: funzioni)
- Indice: [[12_Indice_Lezione_11]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/esempi
