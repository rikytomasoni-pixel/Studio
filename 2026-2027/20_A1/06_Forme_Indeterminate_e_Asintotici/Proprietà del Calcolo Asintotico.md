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

# Proprietà del Calcolo Asintotico

> **Proposizione.** Se $a_n\sim a_n'$ e $b_n\sim b_n'$ allora:
> 1. $a_nb_n\sim a_n'b_n'$;
> 2. $\dfrac{a_n}{b_n}\sim\dfrac{a_n'}{b_n'}$;
> 3. $a_n^\alpha\sim(a_n')^\alpha$ per $\alpha\in\mathbb{R}$ (assumendo che l'operazione abbia senso);
> 4. se $a_n\sim a_n'$ allora le due successioni hanno **lo stesso carattere**: o convergono entrambe allo stesso limite $\ell\in\mathbb{R}$, o divergono entrambe a $+\infty$, o entrambe a $-\infty$, o sono entrambe indeterminate.

**Dimostrazione.**
1. $\dfrac{a_n'b_n'}{a_nb_n}=\dfrac{a_n'}{a_n}\cdot\dfrac{b_n'}{b_n}\to1\cdot1=1$.
2. $\dfrac{a_n/b_n}{a_n'/b_n'}=\dfrac{a_n}{a_n'}\cdot\left(\dfrac{b_n}{b_n'}\right)^{-1}\to1\cdot1^{-1}=1$.
3. $\dfrac{a_n^\alpha}{(a_n')^\alpha}=\left(\dfrac{a_n}{a_n'}\right)^\alpha\to1^\alpha=1$.
4. Se $\exists\lim a_n'=\ell\in\overline{\mathbb{R}}$, allora $a_n=\dfrac{a_n}{a_n'}\cdot a_n'\to1\cdot\ell=\ell$. Se invece $a_n'$ non ammette limite in $\overline{\mathbb{R}}$ e per assurdo $\exists\lim a_n=\ell\in\overline{\mathbb{R}}$, allora $a_n'=\dfrac{a_n'}{a_n}\cdot a_n\to1\cdot\ell=\ell$: **assurdo**. $\square$

> [!warning] Attenzione: cosa NON vale
> In generale, $a_n\sim a_n'$ e $b_n\sim b_n'$ **non** implicano
> - $a_n\pm b_n\sim a_n'\pm b_n'$ (somme e sottrazioni),
> - $a_n^{b_n}\sim(a_n')^{b_n'}$,
> - $e^{a_n}\sim e^{a_n'}$,
> - $\log(a_n)\sim\log(a_n')$.
>
> Inoltre, in generale:
> - $a_n\sim b_n\not\Rightarrow a_n-b_n\to0$;
> - $a_n-b_n\to0\not\Rightarrow a_n\sim b_n$.

---
Precedente: [[Asintotici Notevoli]] · Successivo: [[Esempi di Limiti con gli Asintotici]]
