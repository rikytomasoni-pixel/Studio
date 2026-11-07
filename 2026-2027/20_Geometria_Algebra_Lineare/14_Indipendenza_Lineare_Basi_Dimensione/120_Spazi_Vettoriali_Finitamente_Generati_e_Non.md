---
tags: [GAL, spazi-vettoriali, finitamente-generati, polinomi, lezione-15]
data: 2026-10-28
lezione: 15
fonte: "GAL_2026-2027_-_20261028_-_LEZIONE_15.pdf (slide 123-124)"
---

# Spazi vettoriali finitamente generati e non

> [!abstract] Osservazione 2
> - $V$ **finitamente generato** $\Rightarrow$ il numero massimo di vettori linearmente indipendenti è **limitato**.
> - $V$ **non finitamente generato** $\Leftarrow$ il numero massimo di vettori linearmente indipendenti è **illimitato**.
>
> Per spazi non finitamente generati **non bastano le combinazioni lineari** (finite).

## Esempio: $\mathbb{K}[t]$
Gli spazi di polinomi formano una catena di insiemi linearmente indipendenti sempre più grandi:
$$\{1\}\subseteq\{1,t\}\subseteq\{1,t,t^2\}\subseteq\dots\subseteq\{1,t,\dots,t^d\}\subseteq\dots\qquad(\text{infiniti step})$$
$\Rightarrow$ $\mathbb{K}[t]$ **non è finitamente generato**.

> [!note] Osservazione (non presente negli appunti)
> Motivazione diretta: dato un insieme finito di polinomi, sia $D$ il massimo grado; ogni loro combinazione lineare ha grado $\le D$, quindi $t^{D+1}$ non appartiene allo span e l'insieme non può generare $\mathbb{K}[t]$. Vedi anche [[92_Esempi_di_Spazi_Vettoriali]].

## Note collegate
- [[119_Significato_della_Dimensione_Massimo_Indipendenti_e_Minimo_Generatori]]
- [[92_Esempi_di_Spazi_Vettoriali]]
- [[96_Insieme_di_Generatori]]
- Successiva: [[121_Basi_Canoniche]]
- Indice: [[16_Indice_Lezione_15]] · [[00_MOC_GAL]]

#GAL/spazi-vettoriali/finitamente-generati
