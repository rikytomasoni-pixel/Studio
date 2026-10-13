---
tags: [GAL, sistemi-lineari, MEG, riduzione, parametri, lezione-9]
data: 2026-10-12
lezione: 9
fonte: "GAL 2026-2027 - 20261012 - LEZIONE 9.pdf (slide 76-77)"
---

# Risoluzione di un sistema lineare con il MEG

## Risoluzione

> [!abstract] Le due domande
> 1. Il sistema è risolubile?
> 2. Se la risposta a 1 è sì, quante e quali sono le soluzioni?

**Quale metodo risolutivo?** confronto, sostituzione, **riduzione** (è quella scelta, tramite il [[09_Metodo_di_Eliminazione_di_Gauss]]).

## Esempio con parametri

$$\begin{cases} 3x-2y=1 \\ 6x+ay=b \end{cases}\qquad x,y\ \text{incognite};\quad a,b\in\mathbb{R}\ \text{parametri}$$

Rappresentazione del III tipo:
$$\left[\begin{array}{cc|c} 3&-2&1\\ 6&a&b\end{array}\right]\in M_{\mathbb{R}}(2,2+1)=M_{\mathbb{R}}(2,3)$$

Operazione $\mathrm{II}-2\,\mathrm{I}\to\mathrm{II}$ (sul sistema e sulla matrice):
$$\begin{cases} 3x-2y=1\\ (a+4)y=b-2\end{cases}\qquad\longleftrightarrow\qquad\left[\begin{array}{cc|c} 3&-2&1\\ 0&a+4&b-2\end{array}\right]$$

### Discussione

**Caso $a+4=0$, cioè $a=-4$:**
$$\left[\begin{array}{cc|c} 3&-2&1\\ 0&0&b-2\end{array}\right]$$

- Se $b-2=0$ (cioè $b=2$): matrice $\left[\begin{array}{cc|c} 3&-2&1\\ 0&0&0\end{array}\right]$.
  - **1** Sì, il sistema è risolubile: resta $3x-2y=1$ (l'equazione $0=0$ si cancella).
  - **2** **Infinite soluzioni**: $2y=3x-1$, $\ y=\tfrac12(3x-1)$.
- Se $b-2\neq0$: dividendo $\frac{1}{b-2}\mathrm{II}\to\mathrm{II}$ si ottiene $\left[\begin{array}{cc|c} 3&-2&1\\ 0&0&1\end{array}\right]$.
  - **1** **No**: il sistema contiene $0=1$, **impossibile**.

**Caso $a+4\neq0$, cioè $a\neq-4$:** $\ \frac{1}{a+4}\mathrm{II}\to\mathrm{II}$ dà
$$\left[\begin{array}{cc|c} 3&-2&1\\ 0&1&\frac{b-2}{a+4}\end{array}\right]$$

- **1** Sì: $\begin{cases}3x-2y=1\\ y=\frac{b-2}{a+4}\end{cases}$ e, sostituendo, $3x-2\left(\frac{b-2}{a+4}\right)=1$.
- **2** **Soluzione unica**.

### Riepilogo

| **1** Sì | **1** Sì | **1** No |
|---|---|---|
| $\left[\begin{array}{cc\|c} 3&-2&1\\ 0&1&\frac{b-2}{a+4}\end{array}\right]$ | $\left[\begin{array}{cc\|c} 3&-2&1\\ 0&0&0\end{array}\right]$ | $\left[\begin{array}{cc\|c} 3&-2&1\\ 0&0&1\end{array}\right]$ |
| soluzione unica (due pivot nelle colonne dei coefficienti) | infinite soluzioni (un solo pivot, nella colonna dei coefficienti) | $\varnothing$ (un pivot cade nella colonna dei termini noti) |

Nelle slide il riepilogo è accompagnato dal disegno dei pivot sulla matrice a scala (cerchiati in blu, con la "scala" in rosso): con soluzione unica i pivot sono nelle prime due colonne; con infinite soluzioni c'è un solo pivot; con nessuna soluzione il secondo pivot cade nell'ultima colonna (termini noti).

### Note collegate
- [[00_Indice_Lezione_9]] · [[00_MOC_GAL]]
- [[01_Rappresentazioni_Matriciali_di_un_Sistema_Lineare]]
- [[09_Metodo_di_Eliminazione_di_Gauss]] — MEG
- [[08_Operazioni_Elementari_sulle_Righe]]
- [[10_Pivot_e_Matrice_a_Scala]]
- [[03_Teorema_di_Rouche_Capelli]] — la discussione generale
