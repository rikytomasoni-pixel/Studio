---
tags:
  - AM1
  - taylor
  - resto-di-peano
  - dimostrazione
  - induzione
  - dimostrazione-richiesta
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 4-7)"
---

# Dimostrazione del teorema di Taylor con resto di Peano (D24)

> [!abstract] Tesi
> Se $f:(a,b)\to\mathbb{R}$ è derivabile $n$ volte in $x_0\in(a,b)$, $n\ge1$, allora
> $$\lim_{x\to x_0}\frac{f(x)-P_n(x)}{(x-x_0)^n}=0\qquad\text{cioè}\qquad f(x)=P_n(x)+o\big((x-x_0)^n\big)\ \ (x\to x_0)$$
> Enunciato: [[168_Teorema_di_Taylor_con_Resto_di_Peano]].

**Dimostrazione.** Per induzione su $n\in\mathbb{N}$, $n\ge1$.

### Base: $P(1)$
Se $f$ è derivabile una volta in $x_0$ allora
$$f(x)=P_1(x)+o(x-x_0)=f(x_0)+f'(x_0)(x-x_0)+o(x-x_0)\qquad x\to x_0\quad(*)$$
cioè $f$ è differenziabile in $x_0$ e vale $(*)$. Ciò è vero perché abbiamo già visto che
$$f\text{ derivabile in }x_0\iff f\text{ differenziabile in }x_0$$
e in tal caso vale $(*)$ ([[127_Differenziabilita_e_Approssimazione_Lineare]]). Quindi $P(1)$ è vera.

### Passo induttivo: $P(n-1)\Rightarrow P(n)$, $\forall n\ge2$
**Ipotesi** $P(n-1)$: per ogni funzione $g$ derivabile $(n-1)$ volte in $x_0\in(a,b)$ vale
$$\lim_{x\to x_0}\frac{g(x)-\sum_{k=0}^{n-1}\frac{g^{(k)}(x_0)}{k!}(x-x_0)^k}{(x-x_0)^{n-1}}=0$$

Sia $f$ derivabile $n$ volte in $x_0$, $n\ge2$. Essa è derivabile una volta in un intorno di $x_0$, quindi (con $P_n(x)=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$) il limite
$$\lim_{x\to x_0}\frac{f(x)-P_n(x)}{(x-x_0)^n}\ \ \Big[\tfrac00\Big]$$
è una forma indeterminata $\frac00$ a cui si può applicare [[152_Teorema_di_de_l_Hopital|de l'Hôpital]]:
$$\lim_{x\to x_0}\frac{f(x)-P_n(x)}{(x-x_0)^n}\overset{H}{=}\lim_{x\to x_0}\frac{f'(x)-P_n'(x)}{n(x-x_0)^{n-1}}=\lim_{x\to x_0}\frac{f'(x)-\sum_{j=0}^{n-1}\frac{(f')^{(j)}(x_0)}{j!}(x-x_0)^j}{n(x-x_0)^{n-1}}$$
per l'osservazione su $P_n'$ ([[169_Derivata_del_Polinomio_di_Taylor]]).

Poiché $f'$ è derivabile $(n-1)$ volte in $x_0$, per l'ipotesi induttiva $P(n-1)$ applicata a $g=f'$
$$\lim_{x\to x_0}\frac{f'(x)-\sum_{j=0}^{n-1}\frac{(f')^{(j)}(x_0)}{j!}(x-x_0)^j}{(x-x_0)^{n-1}}=0$$
Per algebra dei limiti e per il teorema di de l'Hôpital
$$\lim_{x\to x_0}\frac{f(x)-P_n(x)}{(x-x_0)^n}=\frac{0}{n}=0$$
Quindi $P(n-1)\Rightarrow P(n)$ vale $\forall n\ge2$ e per induzione $P(n)$ è vera $\forall n\ge1$. $\square$

## Note collegate
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[169_Derivata_del_Polinomio_di_Taylor]]
- [[152_Teorema_di_de_l_Hopital]]
- [[127_Differenziabilita_e_Approssimazione_Lineare]]
- [[173_Taylor_Peano_Unicita_e_Controesempio_senza_Derivate_Successive]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/peano
