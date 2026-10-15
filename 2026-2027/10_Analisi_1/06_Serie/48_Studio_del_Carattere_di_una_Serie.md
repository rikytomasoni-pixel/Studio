---
tags:
  - AM1
  - serie
  - carattere-di-una-serie
  - somme-parziali
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 10-12)"
stato: da_verificare
immagini_mancanti: false
---

# Studio del carattere di una serie

## Relazione ricorsiva tra le somme parziali
$$S_N=\sum_{n=0}^Na_n=\sum_{n=0}^{N-1}a_n+a_N=S_{N-1}+a_N\quad\forall N\geq1\qquad S_0=a_0$$

## Studiare una serie
- Studiare una serie coinvolge **due successioni**: $a_n$ e $S_N$.
- **Studiare il carattere** di una serie significa stabilire se essa è convergente, divergente (a $\pm\infty$) o irregolare.
- Se la serie converge, calcolare esplicitamente il valore
$$S=\sum_{n=0}^{\infty}a_n\in\mathbb{R}$$
è in generale un problema **molto difficile**. Il problema è che spesso non si riesce a determinare una forma "semplice ed esplicita" per
$$S_N=\sum_{n=0}^Na_n$$

Diventa quindi **fondamentale trovare condizioni necessarie o sufficienti** affinché una serie converga o diverga. Successivamente, se la serie converge, si può provare a calcolare un valore approssimato della sua somma.

## Quali termini contano?
- I primi $n_0\in\mathbb{N}$ termini della successione $a_n$ sono **ininfluenti** per determinare il **carattere** della serie $\sum_{n=0}^\infty a_n$ (cioè convergente, divergente a $\pm\infty$ o irregolare).
- Se la serie converge, allora ovviamente **tutti** i termini della successione $a_n$ sono rilevanti per stabilire il **valore** $S=\sum_{n=0}^\infty a_n\in\mathbb{R}$.
- In una serie, i termini della successione $a_n$ vanno sommati **nel giusto ordine** senza alterarlo:
$$S_0=a_0,\qquad S_1=a_0+a_1,\qquad S_2=a_0+a_1+a_2,\ \dots$$

## Note collegate
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[49_Esempi_Elementari_di_Serie]]
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[00_MOC_Analisi_1]]

#AM1/serie/studio-del-carattere
