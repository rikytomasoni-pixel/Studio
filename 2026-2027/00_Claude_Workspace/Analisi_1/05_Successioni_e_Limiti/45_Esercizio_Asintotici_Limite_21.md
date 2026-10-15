---
tags:
  - AM1
  - successioni
  - asintotico
  - limiti
  - esercizio
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 4 e 22-23)"
stato: da_verificare
immagini_mancanti: false
destinazione: "10_Analisi_1/05_Successioni_e_Limiti"
---

# Esercizio: limite con asintotici (risultato $21$)

**Testo** (assegnato per casa a lezione, con risultato indicato $\lim a_n=21$):
$$a_n=n^3\left[\log(n^2+7)-2\log n\right]\frac{\log\left(1+\arctan\frac1{n^2}\right)}{e^{\frac1{3n}}-1}$$

## Svolgimento (riportato in fondo agli appunti)

- $\log(n^2+7)-2\log n=\log\left(n^2\left(1+\frac7{n^2}\right)\right)-\log n^2=\log n^2+\log\left(1+\frac7{n^2}\right)-\log n^2=\frac7{n^2}+o\left(\frac1{n^2}\right)\sim\frac7{n^2}$
  perché $\log(1+\varepsilon_n)\sim\varepsilon_n$ con $\varepsilon_n=\frac7{n^2}\to0$.

- $\log\left(1+\arctan\frac1{n^2}\right)\sim\arctan\frac1{n^2}\sim\frac1{n^2}$
  perché $\log(1+\varepsilon_n)\sim\varepsilon_n$ con $\varepsilon_n=\arctan\frac1{n^2}\to0$, e $\arctan\varepsilon_n\sim\varepsilon_n$ con $\varepsilon_n=\frac1{n^2}\to0$.

- $e^{\frac1{3n}}-1\sim\frac1{3n}$
  perché $e^{\varepsilon_n}-1\sim\varepsilon_n$ con $\varepsilon_n=\frac1{3n}\to0$.

$$\Rightarrow a_n\sim n^{\not3}\cdot\frac7{\not n^{2}}\cdot\frac{\frac1{\not n^{2}}}{\frac1{3\not n}}=21\ \Rightarrow\ \lim_{n\to\infty}a_n=21$$

Verifica del conto: $n^3\cdot\frac7{n^2}\cdot\frac{1/n^2}{1/(3n)}=7n\cdot\frac{3n}{n^2}=21$.

## Note collegate
- [[43_Asintotici_con_Funzioni_Composte]]
- [[44_Esempio_Asintotici_con_Logaritmo_e_Arctan]]
- [[46_Asintotici_Notevoli_e_Limiti_Notevoli]]
- [[42_Confronti_Asintotici_Proprieta_e_Notevoli]]
- [[00_MOC_Analisi_1]]

#AM1/successioni-e-limiti/esercizio-asintotici-limite-21
