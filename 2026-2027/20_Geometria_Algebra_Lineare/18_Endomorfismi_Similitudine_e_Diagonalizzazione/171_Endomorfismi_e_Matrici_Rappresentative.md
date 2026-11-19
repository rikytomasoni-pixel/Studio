---
tags: [GAL, applicazioni-lineari, endomorfismi, matrice-rappresentativa, cambio-di-base, lezione-23]
data: 2026-11-19
lezione: 23
fonte: "GAL 2026-2027 - 20261119 - LEZIONE 23.pdf (slide 192)"
---

# Endomorfismi e matrici rappresentative

Ci concentriamo sul caso specifico $L:V\to V$. Se un'applicazione lineare ha dominio e codominio uguali, parliamo di $L$ come di un **endomorfismo**.

Considero due basi di $V$: $\mathcal{B}$ e $\mathcal{C}$, e il diagramma:

$$A=M_{\mathcal{B}}^{\mathcal{B}}(L),\qquad B=M_{\mathcal{C}}^{\mathcal{C}}(L),\qquad P=M_{\mathcal{C}}^{\mathcal{B}}(\mathrm{id})$$

> [!warning] DISEGNO NON RAPPRESENTABILE (slide 192)
> Cerca nelle slide: il diagramma di cambio di base dell'esempio della simmetria, ma in generale: $V\xrightarrow{L}V$ in alto con $\mathcal{X}_{\mathcal{C}}$, $\mathcal{X}_{\mathcal{B}}$ su ciascun lato; in basso a sinistra freccia verde $B$ tra le copie di $\mathbb{K}^n$ in coordinate $\mathcal{C}$, frecce blu $P$ verso le coordinate $\mathcal{B}$, freccia viola $A$ in basso.

> [!note] OSS
> $L:V\to V\ \Rightarrow$ le matrici rappresentative sono sempre **quadrate**: $A,B,P\in M_{\mathbb{K}}(n,n)$.

La relazione tra $A$ e $B$ è:
$$A=P\,B\,P^{-1}\qquad\qquad B=P^{-1}A\,P$$

## Note collegate
- [[168_Matrice_del_Cambio_di_Base_Definizione_23_1]]
- [[169_Esempio_Cambio_di_Base_per_la_Simmetria_Assiale]]
- [[172_Matrici_Simili_Definizione_23_2]]
- [[141_Composizione_e_Inversione_di_Applicazioni_Lineari]]
- Indice: [[24_Indice_Lezione_23]] · [[00_MOC_GAL]]

#GAL/endomorfismi/matrici-rappresentative
