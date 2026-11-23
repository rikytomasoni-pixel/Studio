---
tags:
  - AM1
  - taylor
  - polinomio-di-taylor
  - definizione
data: 2026-11-20
lezione: 20
fonte: "AM1 L20 26-27.pdf (pag. 19-20)"
---

# Polinomio di Taylor

Dato $f$ derivabile $n$ volte in $x_0$, il polinomio $P_n$ di grado al più $n$ con $P_n^{(k)}(x_0)=f^{(k)}(x_0)$ per $k=0,\dots,n$ (vedi [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]]) è

$$P_n(x)=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k=f(x_0)+f'(x_0)(x-x_0)+\frac{f''(x_0)}{2!}(x-x_0)^2+\frac{f'''(x_0)}{3!}(x-x_0)^3+\dots+\frac{f^{(n-1)}(x_0)}{(n-1)!}(x-x_0)^{n-1}+\frac{f^{(n)}(x_0)}{n!}(x-x_0)^n$$

*(negli appunti: "si dimostra allora che", senza dimostrazione)*

> [!abstract] Definizione (polinomio di Taylor)
> Se $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, $f$ derivabile $n$ volte in $x_0$, $n\ge0$, il polinomio
> $$P_n(x)=\sum_{k=0}^n\frac{f^{(k)}(x_0)}{k!}(x-x_0)^k$$
> si chiama **polinomio di Taylor di $f$ centrato in $x_0$ di ordine $n$**. Se $x_0=0$ si parla anche di **polinomio di Maclaurin**.

## Esempio: $f(x)=\sin x$, $x_0=0$, $n=3$

$f'(x)=\cos x$, $f''(x)=-\sin x$, $f'''(x)=-\cos x$, quindi
$$P_3(x)=0+1\cdot x+0+\frac{(-1)}{6}x^3=x-\frac{x^3}{6}$$
che coincide con lo sviluppo ottenuto con de l'Hôpital in [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]].

## Note collegate
- [[168_Teorema_di_Taylor_con_Resto_di_Peano]]
- [[166_Approssimazioni_Polinomiali_e_Sviluppo_del_Seno]]
- [[124_Funzione_Derivata_e_Derivate_di_Ordine_Superiore]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/polinomio
