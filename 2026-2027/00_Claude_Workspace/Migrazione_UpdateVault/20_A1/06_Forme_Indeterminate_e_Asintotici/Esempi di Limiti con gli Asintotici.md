---
created: 2026-10-09
materia: A1
tags:
  - stato/da-revisionare
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/forme_indeterminate_e_asintotici
aliases: []
origine: UpdateVault
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Esempi di Limiti con gli Asintotici

## Esempio

$$a_n = 3n^7+\log n + o(n^7) \sim 3n^7, \qquad b_n = 2n^6+o(n^6)\sim 2n^6$$
$$\Rightarrow \quad \dfrac{a_n}{b_n} \sim \dfrac{3n^7}{2n^6} = \dfrac32\, n \ \longrightarrow\ +\infty \qquad (n\to\infty)$$

## Esempio (sviluppo con radice cubica)

<DUBBIO posizione="esempio con (n^3+n^2)^(1/3) - (n^3-n)^(1/3)">Il passaggio è ricostruito a partire da appunti molto frammentati; i coefficienti numerici intermedi (in particolare l'ultimo valore del limite, trascritto in modo ambiguo tra "⅓" e "5") sono incerti.</DUBBIO>

$$a_n = \left(n^3+n^2\right)^{1/3} - \left(n^3-n\right)^{1/3}$$

Usando $a^3-b^3=(a-b)(a^2+ab+b^2)$ e gli sviluppi notevoli $(1+\varepsilon_n)^\alpha = 1+\alpha\varepsilon_n+o(\varepsilon_n)$:

$$\left(n^3+n^2\right)^{1/3} = n\left(1+\dfrac1n\right)^{1/3} = n\left(1+\dfrac{1}{3n}+o\!\left(\dfrac1n\right)\right) = n+\dfrac13+o(1)$$

$$\left(n^3-n\right)^{1/3} = n\left(1-\dfrac{1}{n^2}\right)^{1/3} = n\left(1-\dfrac{1}{3n^2}+o\!\left(\dfrac1{n^2}\right)\right) = n-\dfrac{1}{3n}+o\!\left(\dfrac1n\right)$$

$$a_n = \left(n+\dfrac13+o(1)\right) - \left(n-\dfrac{1}{3n}+o\!\left(\dfrac1n\right)\right) = \dfrac13+o(1) \ \longrightarrow\ \dfrac13 \qquad (n\to\infty)$$

## Esempio

<DUBBIO posizione="esempio con e^(1/n)-1 e arctan, poco dopo il richiamo degli asintotici notevoli">Il blocco di appunti relativo a un esempio con $a_n = e^{1/n}-1$ e uno con $\arctan$ è troppo frammentato (simboli sovrapposti, numeri di riga incerti) per essere trascritto senza rischio di errore. Andrebbe verificato sulla registrazione/slide della lezione.</DUBBIO>

---
Precedente: [[Proprietà del Calcolo Asintotico]] · Successivo: [[Regole del Calcolo con o-piccolo]]
