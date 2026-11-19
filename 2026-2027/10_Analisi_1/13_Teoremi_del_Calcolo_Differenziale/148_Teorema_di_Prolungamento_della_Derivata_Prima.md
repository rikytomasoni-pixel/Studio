---
tags:
  - AM1
  - derivate
  - teorema
  - prolungamento-derivata
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 20)"
---

# Teorema di prolungamento della derivata prima

> [!abstract] Teorema (di prolungamento della derivata prima)
> Sia $f:[a,b)\to\mathbb{R}$ continua in $[a,b)$ e derivabile in $(a,b)$. Supponiamo esista
> $$m=\lim_{x\to a^+}f'(x)\in\overline{\mathbb{R}}$$
> Allora esiste anche
> $$f'_+(a)=\lim_{h\to0^+}\frac{f(a+h)-f(a)}{h}=m\in\overline{\mathbb{R}}$$

In parole: se $f$ è continua in $a$ e la derivata ha limite per $x\to a^+$, quel limite è la derivata destra in $a$. Dimostrazione: [[149_Dimostrazione_del_Teorema_di_Prolungamento_della_Derivata]]. Varianti, controesempi: [[150_Osservazioni_sul_Prolungamento_della_Derivata]].

## Esempio: $f(x)=|x|^5$
$$f'(x)=5x^4\operatorname{sgn}x=5|x|x^3\qquad x\ne0$$
(si usa $x\cdot\operatorname{sgn}x=|x|$ per ogni $x\in\mathbb{R}$, vedi [[133_Derivate_con_Valore_Assoluto_e_Segno]]).

Poiché $\displaystyle\lim_{x\to0}f'(x)=0$, per il teorema (nella versione per $f'(x_0)$ di [[150_Osservazioni_sul_Prolungamento_della_Derivata]]) si ha $f'(0)=0$, quindi
$$f'(x)=5|x|x^3\qquad\forall x\in\mathbb{R}$$

## Note collegate
- [[149_Dimostrazione_del_Teorema_di_Prolungamento_della_Derivata]]
- [[150_Osservazioni_sul_Prolungamento_della_Derivata]]
- [[151_Discontinuita_della_Funzione_Derivata]]
- [[142_Teorema_di_Lagrange]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/prolungamento-derivata
