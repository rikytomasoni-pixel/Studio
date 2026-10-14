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

# Proprietà del Calcolo Asintotico

## Proprietà di compatibilità di $\sim$ con prodotto, quoziente, potenza e limite

> [!abstract] Teorema (Proprietà)
> 1. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora $a_n b_n \sim a_n' b_n'$
> 2. Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$
> 3. Se $a_n\sim a_n'$, $\alpha\in\mathbb{R}$, allora $a_n^{\,\alpha}\sim (a_n')^{\,\alpha}$ (assumendo che l'operazione abbia senso)
> 4. Se $a_n\sim b_n$ allora le due successioni hanno lo stesso carattere, cioè: convergono entrambe allo stesso limite, oppure divergono entrambe a $+\infty$, oppure divergono entrambe a $-\infty$, oppure sono entrambe irregolari (non ammettono limite)

**dim:**

1. $$\dfrac{a_nb_n}{a_n'b_n'} = \dfrac{a_n}{a_n'}\cdot\dfrac{b_n}{b_n'} \to 1\cdot 1 = 1$$

2. analoga a 1) con il quoziente al posto del prodotto

3. $$\left(\dfrac{a_n}{a_n'}\right)^{\alpha} \to 1^{\alpha} = 1$$

4. Se $\exists\, \lim_{n\to\infty} a_n = l \in\overline{\mathbb{R}}$, allora $b_n = a_n\cdot\dfrac{b_n}{a_n} \to l\cdot 1 = l$, quindi $\exists\, \lim_{n\to\infty} b_n = l$.
   Se invece $\nexists\, \lim_{n\to\infty} b_n$: per assurdo supponiamo $\exists\, \lim_{n\to\infty} a_n = l$; per quanto appena dimostrato dovrebbe allora essere $\exists\, \lim_{n\to\infty} b_n = l$, assurdo. Quindi $\nexists\, \lim_{n\to\infty} a_n$. $\blacksquare$

> [!danger] Attenzione
> In generale, se $a_n\sim a_n'$ e $b_n\sim b_n'$, **non è detto** che
> $$a_n^{\,b_n} \sim (a_n')^{\,b_n'} \qquad \text{oppure} \qquad \log(a_n) \sim \log(a_n')$$

> [!danger] Attenzione
> In generale $a_n\sim b_n$ **non implica** $a_n-b_n\to 0$.

---
Precedente: [[Asintotici Notevoli]] · Successivo: [[Esempi di Limiti con gli Asintotici]]
