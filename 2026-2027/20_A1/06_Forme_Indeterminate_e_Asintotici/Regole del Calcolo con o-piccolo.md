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

# Regole del Calcolo con o-piccolo

- $a_n\cdot o(b_n)=o(a_nb_n)$. Infatti $\dfrac{a_n\,o(b_n)}{a_nb_n}=\dfrac{o(b_n)}{b_n}\to0$.
- $o(a_n)=a_n\cdot o(1)$.
- $c\cdot o(a_n)=o(a_n)$ per ogni costante $c\neq0$: $\dfrac{c\,o(a_n)}{a_n}\to c\cdot0=0$.
- $\pm\,o(a_n)=o(a_n)$.
- $o\!\left(\frac1n\right)+o\!\left(\frac1{n^2}\right)=o\!\left(\frac1n\right)$ e $o(n)+o(n^2)=o(n^2)$ (vince l'ordine «più grande»).
- Se $a_n\sim b_n$ allora $o(a_n)=o(b_n)$. Infatti $\dfrac{o(a_n)}{b_n}=\dfrac{o(a_n)}{a_n}\cdot\dfrac{a_n}{b_n}\to0\cdot1=0$. Ad esempio $o\!\left(\sin\frac1n\right)=o\!\left(\frac1n\right)$.

### Esempio da completare (forma $\frac00$)
$$a_n=\frac{\sin\frac1n-\frac1n}{\frac1{n^3}}.$$
Poiché $\sin\varepsilon_n=\varepsilon_n+o(\varepsilon_n)$ con $\varepsilon_n=\frac1n$:
$$\sin\frac1n-\frac1n=\frac1n+o\!\left(\frac1n\right)-\frac1n=o\!\left(\frac1n\right)\ \Rightarrow\ a_n=\frac{o(1/n)}{1/n^3}=n^3\,o\!\left(\frac1n\right)=o(n^2).$$
Con questo livello di approssimazione **non si riesce a concludere** quanto vale $\lim a_n$: la stima $o(n^2)$ è troppo debole. *(L'esempio nel quaderno termina con «$\lim a_n=\,?$»: servirebbe uno sviluppo di $\sin\varepsilon_n$ a un ordine successivo.)*

---
Precedente: [[Esempi di Limiti con gli Asintotici]]
