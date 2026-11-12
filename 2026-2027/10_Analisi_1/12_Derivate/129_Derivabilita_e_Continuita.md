---
tags:
  - AM1
  - derivate
  - continuita
  - teorema
  - dimostrazione
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 23-25)"
---

# Derivabilità e continuità

> [!abstract] Teorema (continuità delle funzioni derivabili)
> Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$ e $f$ è derivabile in $x_0$, allora $f$ è continua in $x_0$.

**Dimostrazione.** Vogliamo mostrare che $\displaystyle\lim_{x\to x_0}f(x)=f(x_0)$. Vale
$$\lim_{x\to x_0}\big(f(x)-f(x_0)\big)=\lim_{x\to x_0}\underbrace{\frac{f(x)-f(x_0)}{x-x_0}}_{\to\,f'(x_0)\in\mathbb{R}}\cdot\underbrace{(x-x_0)}_{\to\,0}=0$$
$$\Rightarrow\ \lim_{x\to x_0}f(x)=f(x_0)\qquad\square$$

> [!note] Osservazione — il viceversa è falso
> Il viceversa non è vero: esistono funzioni continue ma non derivabili.

**Esempio.** $f(x)=|x|$, $f:\mathbb{R}\to\mathbb{R}$, $x_0=0$. $f$ è continua in $\mathbb{R}$ ma
$$f'_+(0)=\lim_{h\to0^+}\frac{|h|}h=1\qquad f'_-(0)=\lim_{h\to0^-}\frac{|h|}h=-1$$
$\Rightarrow\nexists f'(0)$ e $f$ non è derivabile in $x_0=0$.

## Note collegate
- [[93_Continuita_in_un_Punto]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[123_Esempi_di_Derivata_e_Retta_Tangente]]
- [[127_Differenziabilita_e_Approssimazione_Lineare]]
- [[130_Classificazione_dei_Punti_di_Non_Derivabilita]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/continuita
