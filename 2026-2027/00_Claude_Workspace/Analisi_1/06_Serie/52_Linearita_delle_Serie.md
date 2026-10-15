---
tags:
  - AM1
  - serie
  - linearita
  - algebra-dei-limiti
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 15-16)"
stato: da_verificare
immagini_mancanti: false
destinazione: "10_Analisi_1/06_Serie"
---

# Linearità delle serie

**Osservazione.** Dal teorema sull'algebra dei limiti ([[34_Algebra_dei_Limiti]]) e dall'aritmetizzazione parziale di $\infty$ ([[37_Algebra_Limiti_Infiniti]]) segue che, date due serie **regolari** $\sum_{n=0}^\infty a_n$, $\sum_{n=0}^\infty b_n$ e $\alpha,\beta\in\mathbb{R}$, vale
$$\sum_{n=0}^\infty(\alpha a_n+\beta b_n)=\alpha\sum_{n=0}^\infty a_n+\beta\sum_{n=0}^\infty b_n$$
**se l'espressione a destra non è una forma di indeterminazione.**

**Infatti**
$$\sum_{n=0}^\infty(\alpha a_n+\beta b_n)=\lim_{N\to\infty}\sum_{n=0}^N(\alpha a_n+\beta b_n)=\lim_{N\to\infty}\left[\alpha\sum_{n=0}^Na_n+\beta\sum_{n=0}^Nb_n\right]$$
$$=\alpha\lim_{N\to\infty}\sum_{n=0}^Na_n+\beta\lim_{N\to\infty}\sum_{n=0}^Nb_n=\alpha\sum_{n=0}^\infty a_n+\beta\sum_{n=0}^\infty b_n$$

Applicazione: [[51_Rappresentazione_Decimale_e_Serie]] (si porta fuori il fattore $9$).

## Note collegate
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[34_Algebra_dei_Limiti]]
- [[37_Algebra_Limiti_Infiniti]]
- [[53_Serie_Telescopiche_e_Mengoli]]
- [[00_MOC_Analisi_1]]

#AM1/serie/linearita
