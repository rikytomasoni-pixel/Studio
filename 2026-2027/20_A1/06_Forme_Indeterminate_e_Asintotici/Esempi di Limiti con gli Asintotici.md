---
created: 2026-10-09
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/9
  - argomento/forme_indeterminate_e_asintotici
aliases: []
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Esempi di Limiti con gli Asintotici

### Esempio 1: rapporto di «polinomi generalizzati»
$$a_n=\frac{3n^7+5n^{42/95}+\log n-\cos n+5}{2n^6-18n^3+\arctan n+(\log n)^2-2}.$$
Numeratore $N=3n^7+o(n^7)\sim3n^7$ e denominatore $D=2n^6+o(n^6)\sim2n^6$. Quindi
$$a_n=\frac{3n^7+o(n^7)}{2n^6+o(n^6)}\sim\frac{3n^7}{2n^6}=\frac32n\to+\infty\ \Rightarrow\ \lim a_n=+\infty.$$

### Esempio 2
$$a_n=\frac{\sin\frac1{n^2}}{e^{7/n}-1}\cdot n.$$
- $\varepsilon_n=\frac1{n^2}\to0$: $\sin\frac1{n^2}\sim\frac1{n^2}$;
- $\varepsilon_n=\frac7n\to0$: $e^{7/n}-1\sim\frac7n$.

$$a_n\sim\frac{\frac1{n^2}}{\frac7n}\cdot n=\frac17\ \Rightarrow\ \lim a_n=\frac17.$$

### Esempio 3
$$a_n=\frac{\sqrt[3]{1+n}-n^{1/3}}{1-e^{2/n}}\cdot\arctan\frac1{n^2}\cdot n^{5/3}.$$
- $\arctan\frac1{n^2}\sim\frac1{n^2}$ (con $\varepsilon_n=\frac1{n^2}\to0$);
- $1-e^{2/n}\sim-\frac2n$, perché $-(e^{\varepsilon_n}-1)\sim-\varepsilon_n$ con $\varepsilon_n=\frac2n\to0$;
- $\sqrt[3]{1+n}-n^{1/3}\sim\,?$

> [!warning] Errori da evitare
> - $\sqrt[3]{1+n}=(1+n)^{1/3}\neq1+\frac n3+o(n)$, perché $\varepsilon_n=n\not\to0$.
> - $\sqrt[3]{1+n}\sim n^{1/3}$ è vero, **ma** $\sqrt[3]{1+n}-n^{1/3}\not\sim n^{1/3}-n^{1/3}=0$: **non si usa $\sim$ nelle somme e sottrazioni**.

Si raccoglie $n$ in modo da avere $(1+\varepsilon_n)^\alpha$ con $\varepsilon_n=\frac1n$ e $\alpha=\frac13$:
$$\sqrt[3]{1+n}=n^{1/3}\left(1+\frac1n\right)^{1/3}=n^{1/3}\left(1+\frac1{3n}+o\!\left(\frac1n\right)\right)=n^{1/3}+\frac1{3n^{2/3}}+o\!\left(\frac1{n^{2/3}}\right).$$
Infatti $\dfrac{n^{1/3}\,o(1/n)}{1/n^{2/3}}=\dfrac{o(1/n)}{1/n}\to0$. Quindi
$$\sqrt[3]{1+n}-n^{1/3}=\frac1{3n^{2/3}}+o\!\left(\frac1{n^{2/3}}\right)\sim\frac1{3n^{2/3}}.$$
Mettendo tutto insieme:
$$a_n\sim\frac{\frac1{3n^{2/3}}}{-\frac2n}\cdot\frac1{n^2}\cdot n^{5/3}=-\frac16.$$

### Esempio 4
$$a_n=(n^3+n^2)^{1/3}-(n^3-n)^{1/3}.$$
Si potrebbe usare $a^3-b^3=(a-b)(a^2+ab+b^2)$; qui si usa invece lo sviluppo:
$$(n^3+n^2)^{1/3}=n\left(1+\frac1n\right)^{1/3}=n\left(1+\frac1{3n}+o\!\left(\frac1n\right)\right),$$
$$(n^3-n)^{1/3}=n\left(1-\frac1{n^2}\right)^{1/3}=n\left(1-\frac1{3n^2}+o\!\left(\frac1{n^2}\right)\right).$$
Quindi
$$a_n=n+\frac13+n\,o\!\left(\frac1n\right)-n+\frac1{3n}+n\,o\!\left(\frac1{n^2}\right)=\frac13+\frac1{3n}+o(1)=\frac13+o(1)\to\frac13.$$
(Infatti $\dfrac{n\,o(1/n)}{1}=\dfrac{o(1/n)}{1/n}\to0$ e $\dfrac{n\,o(1/n^2)}{1/n}=\dfrac{o(1/n^2)}{1/n^2}\to0$.)

---
Precedente: [[Proprietà del Calcolo Asintotico]] · Successivo: [[Regole del Calcolo con o-piccolo]]
