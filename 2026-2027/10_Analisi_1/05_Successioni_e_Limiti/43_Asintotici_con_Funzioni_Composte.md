---
tags:
  - AM1
  - successioni
  - asintotico
  - o-piccolo
  - funzioni-composte
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 2-4)"
---

# Asintotici con funzioni composte

## Richiamo
$$a_n\sim b_n\iff\lim_{n\to\infty}\frac{a_n}{b_n}=1\qquad a_n=o(b_n)\iff\lim_{n\to\infty}\frac{a_n}{b_n}=0\qquad a_n\sim b_n\iff a_n=b_n+o(b_n)$$
(vedi [[41_o_piccolo_e_Asintotico]] e [[42_Confronti_Asintotici_Proprieta_e_Notevoli]])

## Osservazione: le tre scritture equivalenti per $e^{\varepsilon_n}$
Se $\varepsilon_n\to0$:
$$\begin{cases} e^{\varepsilon_n}-1\sim\varepsilon_n\\ e^{\varepsilon_n}-1=\varepsilon_n+o(\varepsilon_n)\\ e^{\varepsilon_n}=1+\varepsilon_n+o(\varepsilon_n)\end{cases}$$
sono **equivalenti**. Esse **non sono equivalenti** a
$$e^{\varepsilon_n}\sim1+\varepsilon_n$$
Questa è più **debole** ed è equivalente a
$$e^{\varepsilon_n}\sim1+\frac1{n!},\qquad e^{\varepsilon_n}\sim1+\frac1{\log\varepsilon_n}\ \ (\text{se }\varepsilon_n>0\text{ definitivamente}),\qquad e^{\varepsilon_n}\sim1-\frac1{2^n},\qquad e^{\varepsilon_n}\sim1+o(1)$$

## Osservazione: composizione
> [!abstract] Osservazione
> È possibile usare la relazione di asintotico $\sim$ con **funzioni composte**, **partendo dalla più esterna** quando si fa lo sviluppo.

## Esempio
$$a_n=\sin\left(\log\left(\cos\frac1n\right)\right)\longrightarrow0$$

Va pensata come $a_n=\sin\varepsilon_n$ con $\varepsilon_n=\log\left(\cos\frac1n\right)\to0$:
$$\Rightarrow a_n=\sin\varepsilon_n\sim\varepsilon_n=\log\left(\cos\frac1n\right)=a_n'$$
e $a_n'=\log\left(\cos\frac1n\right)$ va pensata come $a_n'=\log(1+\varepsilon_n')$ con $\varepsilon_n'=\cos\frac1n-1\to0$:
$$\Rightarrow a_n'\sim\log(1+\varepsilon_n')\sim\varepsilon_n'=\cos\frac1n-1=a_n''$$
e $a_n''=\cos\frac1n-1$ va pensata come $a_n''=\cos(\varepsilon_n'')-1\sim-\frac{(\varepsilon_n'')^2}{2}$ con $\varepsilon_n''=\frac1n\to0$:
$$\Rightarrow a_n\sim\log\left(\cos\frac1n\right)\sim\cos\frac1n-1\sim-\frac1{2n^2}\ \Rightarrow\ \boxed{a_n\sim-\frac1{2n^2}}$$

Schema riassuntivo (annotato a mano con le parentesi):
$$a_n=\sin\Big(\underbrace{\log\big(\underbrace{\cos\tfrac1n}_{1+\varepsilon_n'}\big)}_{\varepsilon_n\to0}\Big)\ \sim\ \log\left(\cos\tfrac1n\right)\ \sim\ \underbrace{\cos\tfrac1n-1}_{\varepsilon_n''\to0}\ \sim\ -\frac1{2n^2}$$
**perché gli argomenti sono infinitesimi.**

## Note collegate
- [[44_Esempio_Asintotici_con_Logaritmo_e_Arctan]]
- [[45_Esercizio_Asintotici_Limite_21]]
- [[46_Asintotici_Notevoli_e_Limiti_Notevoli]]
- [[41_o_piccolo_e_Asintotico]]
- [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]
- [[00_MOC_Analisi_1]]

#AM1/successioni-e-limiti/asintotici-funzioni-composte
