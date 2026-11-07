---
tags: [GAL, dimensione, misura, lezione-16]
data: 2026-11-04
lezione: 16
fonte: "GAL 2026-2027 - 20261104 - LEZIONE 16.pdf (slide 138)"
---

# Significato della dimensione (seconda parte): la dimensione è una misura

Sia $V$ uno spazio vettoriale finitamente generato. Allora
$$\dim V=\#\text{ elementi di una base di }V=\text{gradi di libertà per muoversi in }V=\#\text{ parametri liberi per descrivere un elemento di }V$$

> **"La dimensione è una misura!"**

## Altre misure note
| Misura | Dominio → codominio |
|---|---|
| Area $\mathcal{A}$ | $\{\text{regioni limitate di }\mathbb{R}^2\}\to\mathbb{R}_{\ge0}$ |
| Volume $\mathcal{V}$ | $\{\text{regioni limitate di }\mathbb{R}^3\}\to\mathbb{R}_{\ge0}$ |
| Probabilità $\mathbb{P}$ | $\{\text{eventi}\}\to[0,1]$ |
| Integrale definito $\int$ | $\{\text{funzioni continue su }[a,b]\}\to\mathbb{R}$ |
| Dimensione $\dim$ | $\{\text{spazi vettoriali finitamente generati}\}\to\mathbb{N}$ |

## Proprietà delle misure (dell'area)
- Per $A,B$ **disgiunti**: $\mathcal{A}(A\cup B)=\mathcal{A}(A)+\mathcal{A}(B)$ (**additività** della misura).
- In generale (con sovrapposizione): $\mathcal{A}(A\cup B)=\mathcal{A}(A)+\mathcal{A}(B)-\mathcal{A}(A\cap B)$.

> [!warning] DISEGNO NON RAPPRESENTABILE
> GAL L16 slide 138: due figure: un cerchio azzurro $A$ e un rettangolo verde $B$ disgiunti (additività), poi gli stessi due che si sovrappongono parzialmente (la zona comune è $A\cap B$).

Questa formula è l'analogo che si cerca per i sottospazi: [[135_Formula_di_Grassmann_Teorema_16_3]].

## Note collegate
- [[119_Significato_della_Dimensione_Massimo_Indipendenti_e_Minimo_Generatori]] (prima parte)
- [[102_Dimensione_di_uno_Spazio_Vettoriale]]
- [[118_Teorema_della_Dimensione_Teorema_15_2]]
- [[133_Intersezione_di_Sottospazi_Vettoriali]]
- Indice: [[17_Indice_Lezione_16]] · [[00_MOC_GAL]]

#GAL/dimensione/misura
