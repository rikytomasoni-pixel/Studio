---
created: 2026-10-07
materia: A1
tags:
  - materia/a1
  - tipo/nota-atomica
  - fonte/handwritten
  - lezione/8
  - argomento/forme_indeterminate_e_asintotici
aliases: []
---
[[00_A1_Forme_Indeterminate_e_Asintotici|⬅️ Torna a Forme Indeterminate e Asintotici]]

# Tecniche per le Forme Infinito meno Infinito

**Razionalizzazione.** $a_n=\sqrt{n^2+n}-\sqrt{n^2-n}$. Posti $a=\sqrt{n^2+n}$, $b=\sqrt{n^2-n}$, si usa $a-b=\dfrac{a^2-b^2}{a+b}$:
$$a_n=\frac{(n^2+n)-(n^2-n)}{\sqrt{n^2+n}+\sqrt{n^2-n}}=\frac{2n}{n\left(\sqrt{1+\frac1n}+\sqrt{1-\frac1n}\right)}\to\frac2{1+1}=1.$$

**Radice $m$-esima.** Per $\sqrt[7]{n^2+n}-\sqrt[7]{n^2-n}$ si usa la formula
$$a^m-b^m=(a-b)\sum_{k=0}^{m-1}a^{m-1-k}b^k.$$
(per $m=7$: $a^7-b^7=(a-b)(a^6+a^5b+a^4b^2+a^3b^3+a^2b^4+ab^5+b^6)$.) Lo stesso metodo si può applicare, ad esempio, a $a_n=(n^2+n)^{1/\sqrt2}-(n^2-n)^{1/\sqrt2}$, il cui limite viene lasciato come esercizio.

---
Precedente: [[Aritmetizzazione dell'Infinito e Forme di Indeterminazione]] · Successivo: [[Potenze con Base ed Esponente Variabili]]
