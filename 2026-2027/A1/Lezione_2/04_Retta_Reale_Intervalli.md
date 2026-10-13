---
tags:
  - AM1
  - retta-reale
  - intervalli
  - densita
  - numeri-reali
data: 2026-09-16
fonte: Lezione 2
---

# Rappresentazione geometrica di $\mathbb{R}$: la retta reale

$\mathbb{R}$ può essere rappresentato geometricamente mettendo i suoi elementi in corrispondenza biunivoca con i punti di una retta orientata (si può fare anche con $\mathbb{Q}$, ma la corrispondenza **non** è biunivoca): ad ogni numero reale corrisponde un punto sulla retta e viceversa *(per $\mathbb{Q}$ il viceversa è falso)*.

**Costruzione:**
- si fissa arbitrariamente un punto sulla retta, cui si associa $0$;
- si fissa un secondo punto, distinto dal primo, cui si associa $1$;
- il segmento $\overline{01}$ è l'unità di misura;
- ad ogni $a\in\mathbb{R}$ si associa il punto sulla retta che è secondo estremo di un segmento avente primo estremo in $0$ e lunghezza $|a|$. Il punto è dallo stesso lato di $1$ se $a>0$, dal lato opposto se $a<0$.
![[Lunghezza absA.png]]
Geometricamente $|a|$ è la lunghezza del segmento di estremi $0$ e $a$. Più in generale, $|b-a|$ è la **distanza** di $a$ da $b$, cioè la lunghezza del segmento di estremi $a,b$, $\ \forall\, a,b\in\mathbb{R}$.

## Esistono punti della retta a cui non corrisponde alcun razionale

**Osservazione.** Esistono punti sulla retta cui non corrispondono numeri $r\in\mathbb{Q}$.
![[Rcomeretta.png]]
$\overline{OB}$ è la diagonale del quadrato di lato $1$, e $H$ è il punto sulla retta tale che $|\overline{OH}| = |\overline{OB}|$.

Per il **teorema di Pitagora**:
$$|\overline{OB}|^2 = 1^2+1^2 = 2$$

Se esistesse $r\in\mathbb{Q}$ associato ad $H$, secondo la costruzione di cui sopra dovrebbe essere $r = |\overline{OH}|$, quindi
$$r^2 = |\overline{OH}|^2 = |\overline{OB}|^2 = 2$$
il che è **assurdo**, poiché non esiste alcun numero razionale il cui quadrato sia $2$.

$$\Rightarrow \quad \nexists\, r\in\mathbb{Q} \text{ corrispondente ad } H \qquad \left(r=\sqrt{2}\in\mathbb{R},\ \text{ma } \sqrt2\notin\mathbb{Q}\right)$$

## Intervalli della retta reale

Dati $a,b\in\mathbb{R}$ con $a<b$:

> [!info] Intervalli limitati
> $$(a,b) = \{x\in\mathbb{R} : a<x<b\} \qquad a\ \circ\!\!-\!\!-\!\!-\!\!-\!\!-\!\!-\!\!\circ\ b$$
> $$[a,b) = \{x\in\mathbb{R} : a\leq x<b\} \qquad a\ \bullet\!\!-\!\!-\!\!-\!\!-\!\!-\!\!-\!\!\circ\ b$$
> $$(a,b] = \{x\in\mathbb{R} : a<x\leq b\} \qquad a\ \circ\!\!-\!\!-\!\!-\!\!-\!\!-\!\!-\!\!\bullet\ b$$
> $$[a,b] = \{x\in\mathbb{R} : a\leq x\leq b\} \qquad a\ \bullet\!\!-\!\!-\!\!-\!\!-\!\!-\!\!-\!\!\bullet\ b$$

Sono tutti **insiemi limitati**, e hanno tutti $\sup = b$ (massimo per $(a,b]$, $[a,b]$) e $\inf = a$ (minimo per $[a,b)$, $[a,b]$).

- $(a,b)$ è **aperto**; $[a,b]$ è **chiuso**;
- $(a,b]$, $[a,b)$ non sono né aperti né chiusi.

> [!info] Intervalli illimitati
> $$(-\infty,b) = \{x\in\mathbb{R} : x<b\} \qquad \longleftarrow\!\!-\!\!-\!\!-\!\!-\!\!\circ\ b$$
> $$(-\infty,b] = \{x\in\mathbb{R} : x\leq b\} \qquad \longleftarrow\!\!-\!\!-\!\!-\!\!-\!\!\bullet\ b$$
> $$(a,\infty) = \{x\in\mathbb{R} : x>a\} \qquad a\ \circ\!\!-\!\!-\!\!-\!\!-\!\!\longrightarrow$$
> $$[a,\infty) = \{x\in\mathbb{R} : x\geq a\} \qquad a\ \bullet\!\!-\!\!-\!\!-\!\!-\!\!\longrightarrow$$

- $(-\infty,b]$, $(-\infty,b)$ sono limitate dall'alto: $\inf = -\infty$, $\sup = b$ (massimo per $(-\infty,b]$).
- $(a,\infty)$, $[a,\infty)$ sono limitate dal basso: $\inf = a$ (minimo per $[a,\infty)$), $\sup = +\infty$.
- $(a,\infty)$, $(-\infty,b)$ sono **aperte**; $[a,\infty)$, $(-\infty,b]$ sono **chiuse**.

$$\mathbb{R} = (-\infty,\infty)$$

$\mathbb{R}$ è illimitato dall'alto e dal basso, è sia aperto che chiuso, con $\inf \mathbb{R} = -\infty$ e $\sup \mathbb{R} = +\infty$.

## Densità di $\mathbb{Q}$ in $\mathbb{R}$

> [!abstract] Teorema — Densità di $\mathbb{Q}$ in $\mathbb{R}$
> $\forall\, x,y\in\mathbb{R}$ tali che $x<y$, $\exists\, r\in\mathbb{Q}$ tale che
> $$x<r<y$$
> Si dice che $\mathbb{Q}$ è **denso** in $\mathbb{R}$.

> [!warning] Aggiunte presenti nella versione precedente ma non nel PDF manoscritto
> - Nella costruzione di $H$: «riportando con il compasso la lunghezza della diagonale sull'asse» (nel PDF compare solo il disegno dell'arco).
> - Dopo l'assurdo $r^2=2$: «fatto già noto, dimostrabile ad esempio per assurdo con un argomento di parità» (nel PDF non c'è).

### Note collegate
- [[00_MOC_A1]]
- [[03_Valore_Assoluto]] — $|a|$ e $|b-a|$
- [[02_Estremo_Superiore_Inferiore]] — $\sup$ e $\inf$
- [[03_Dimostrazione_per_Assurdo]] — $\nexists\, x\in\mathbb{Q}: x^2=2$
- [[00_Insiemi_Numerici]]
- [[02_Piano_di_Argand_Gauss]] — analogo geometrico per $\mathbb{C}$