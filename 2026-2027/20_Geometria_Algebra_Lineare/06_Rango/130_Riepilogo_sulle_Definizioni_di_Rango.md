---
tags: [GAL, rango, riepilogo, MEG, lezione-16]
data: 2026-11-04
lezione: 16
fonte: "GAL 2026-2027 - 20261104 - LEZIONE 16.pdf (slide 135, 137)"
---

# Riepilogo sulle varie definizioni di rango

Sia $A\in M_{\mathbb{K}}(m,n)$.

**(1) Definizione "a somma di rango 1".**
$$r(A)=\min\Big\{r\ \Big|\ A=\sum_{i=1}^{r}C_iR_i\Big\}\qquad C_i\in\mathbb{K}^m=M_{\mathbb{K}}(m,1),\quad R_i\in\mathbb{K}^n=M_{\mathbb{K}}(1,n)$$

**(2) Definizione tramite il MEG.** Se $A\xrightarrow{\ \text{MEG}\ }U$ a scala, allora
$$r(A)=r(U)=\#\text{pivot di }U=\#\text{righe}\neq0\text{ di }U$$

**(3) Definizione tramite lo spazio delle righe.** Da mercoledì 28/10 ([[119_Significato_della_Dimensione_Massimo_Indipendenti_e_Minimo_Generatori]], [[123_Base_per_Costruzione_Libera_con_il_MEG_sulle_Righe]]):
$$\#\text{pivot di }U=\dim\operatorname{Span}\big(R_1(U),\dots,R_m(U)\big)=\dim\operatorname{Span}\big(R_1(A),\dots,R_m(A)\big)$$
quindi
$$r(A)=\dim\operatorname{Span}\big(R_1(A),\dots,R_m(A)\big)$$

**(4) Definizione tramite lo spazio delle colonne** (da [[131_Spazio_delle_Righe_e_delle_Colonne]]): $r(A)=\dim\operatorname{col}(A)$.

**(5) Caratterizzazione con fattorizzazione.** $r(A)=r$ tale che $A=\sum_{i=1}^{r}C_iR_i$ con
- $\{C_1,\dots,C_r\}$ insieme di vettori linearmente indipendenti in $\mathbb{K}^m$
- $\{R_1,\dots,R_r\}$ insieme di vettori linearmente indipendenti in $\mathbb{K}^n$

(vedi l'esempio svolto in [[131_Spazio_delle_Righe_e_delle_Colonne]]).

## Note collegate
- [[63_Rango_di_una_Matrice]]
- [[73_MEG_e_Rango]]
- [[69_Pivot_e_Matrice_a_Scala]]
- [[108_Esercizio_EE1_Somma_di_Matrici_di_Rango_1]]
- [[131_Spazio_delle_Righe_e_delle_Colonne]]
- Indice: [[17_Indice_Lezione_16]] · [[00_MOC_GAL]]

#GAL/rango/riepilogo
