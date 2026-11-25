---
tags:
  - AM1
  - derivate-successive
  - flesso
  - derivata-seconda
  - teorema
  - controesempio
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 13-15)"
---

# Flessi e derivata seconda

> [!abstract] Teorema
> Se $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, $f$ derivabile 2 volte in $x_0$ e $x_0$ è un punto di flesso per $f$, allora
> $$f''(x_0)=0$$

> [!warning] Il viceversa è falso
> $f''(x_0)=0\ \not\Rightarrow\ x_0$ è punto di flesso.

*— nessuna dimostrazione negli appunti —*

## Controesempio: $f(x)=x^4$

$f'(x)=4x^3$, $f''(x)=12x^2$ per ogni $x\in\mathbb{R}$. Quindi $f''(0)=0$, ma $f''(x)\ge0$ per ogni $x\in\mathbb{R}$, dunque (per il [[162_Test_di_Convessita|test di convessità]]) $f$ è **convessa** in $\mathbb{R}$ e ha **minimo stretto** in $x_0=0$ con $f(0)=0$: $x_0$ **non è punto di flesso**.

![[ControesempioNota165.png]]

## Funzioni non derivabili due volte che hanno un flesso: $f(x)=x^{5/3}$, $x_0=0$

Esistono funzioni **non** derivabili due volte in $x_0$ che hanno in $x_0$ un punto di flesso.

$$f'(x)=\frac53x^{2/3}\quad\forall x\in\mathbb{R}\qquad f''(x)=\frac{10}{9}x^{-1/3}\quad\forall x\in\mathbb{R}\setminus\{0\}$$

$$f''_+(0)=\lim_{x\to0^+}f''(x)=+\infty\qquad f''_-(0)=\lim_{x\to0^-}f''(x)=-\infty\qquad\Rightarrow\quad\nexists f''(0)$$

Tuttavia $x_0=0$ è un punto di flesso: $f$ ha retta tangente $y=0$ in $(0,0)$ e $f(x)>0$ se $x>0$, $f(x)<0$ se $x<0$.

![[disegnoNota165.png]]

> [!note] Osservazione (non presente negli appunti)
> L'uguaglianza tra $f''_\pm(0)$ e il limite di $f''(x)$ è giustificata dal [[148_Teorema_di_Prolungamento_della_Derivata_Prima|teorema di prolungamento della derivata]] applicato a $f'$.

## Note collegate
- [[163_Punti_di_Flesso]]
- [[164_Punti_di_Cambio_di_Concavita]]
- [[162_Test_di_Convessita]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[138_Punti_Stazionari_e_Punti_Critici]]
- [[157_Studio_del_Grafico_di_una_Funzione]]
- [[00_MOC_Analisi_1]]

#AM1/derivate-successive/flesso
