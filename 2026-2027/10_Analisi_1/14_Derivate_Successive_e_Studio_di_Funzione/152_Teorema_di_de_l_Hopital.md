---
tags:
  - AM1
  - derivate
  - de-l-hopital
  - limiti-di-funzioni
  - teorema
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 15-16)"
---

# Teorema di de l'Hôpital

> [!abstract] Teorema (di de l'Hôpital)
> Siano $f,g:(a,b)\to\mathbb{R}$ derivabili, con $g,g'\ne0$ in $(a,b)$. Se
> 1. $\displaystyle\lim_{x\to a^+}f(x)=\lim_{x\to a^+}g(x)=0$
>    oppure
>    $\displaystyle\lim_{x\to a^+}f(x)=\pm\infty$, $\displaystyle\lim_{x\to a^+}g(x)=\pm\infty$ (qualunque segno, anche discordi)
> 2. esiste $\displaystyle\lim_{x\to a^+}\frac{f'(x)}{g'(x)}=L\in\overline{\mathbb{R}}$
>
> allora esiste
> $$\lim_{x\to a^+}\frac{f(x)}{g(x)}=L\qquad\left[\tfrac00,\ \tfrac\infty\infty\right]$$

*— no dimostrazione —*

## Osservazioni
- Vale sia nel caso $a\in\mathbb{R}$ che nel caso $a=-\infty$.
- Vale anche se si considerano i casi $\displaystyle\lim_{x\to b^-}(\dots)$ o $\displaystyle\lim_{x\to x_0}(\dots)$, con $b\in\mathbb{R}\cup\{+\infty\}$ e $x_0\in\mathbb{R}$.
- Copre **solo** le forme di indeterminazione $\dfrac00$ e $\dfrac\infty\infty$.

> [!warning] Il teorema non si inverte
> Se **non esiste** $\displaystyle\lim_{x\to a^+}\frac{f'(x)}{g'(x)}$ in $\overline{\mathbb{R}}$, **non si può concludere nulla** sul $\displaystyle\lim_{x\to a^+}\frac{f(x)}{g(x)}$ (che può esistere o no). Controesempio: [[153_Controesempio_de_l_Hopital_Limite_delle_Derivate_Inesistente]].

Esempi di uso: [[154_Esempi_di_Applicazione_de_l_Hopital]]; applicazione importante: [[155_Dimostrazione_della_Gerarchia_degli_Infiniti_con_de_l_Hopital]].

## Note collegate
- [[153_Controesempio_de_l_Hopital_Limite_delle_Derivate_Inesistente]]
- [[154_Esempi_di_Applicazione_de_l_Hopital]]
- [[155_Dimostrazione_della_Gerarchia_degli_Infiniti_con_de_l_Hopital]]
- [[102_Algebra_dei_Limiti_di_Funzioni]]
- [[142_Teorema_di_Lagrange]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/de-l-hopital
