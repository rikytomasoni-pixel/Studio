---
tags:
  - AM1
  - derivate
  - definizione
  - derivata-seconda
data: 2026-11-11
lezione: 17
fonte: "AM1 L17 26-27.pdf (pag. 12-14)"
---

# Funzione derivata e derivate di ordine superiore

> [!note] Osservazione — funzione derivata
> Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$ è derivabile in $x_0$ per ogni $x_0\in(a,b)$, risulta definita la **funzione derivata prima** di $f$
> $$f':(a,b)\subseteq\mathbb{R}\to\mathbb{R},\qquad x\in(a,b)\longmapsto f'(x)=\lim_{h\to0}\frac{f(x+h)-f(x)}{h}\in\mathbb{R}$$

> [!abstract] Definizione — derivata seconda
> Se $f:(a,b)\to\mathbb{R}$, $x_0\in(a,b)$, se $f$ è derivabile in un intorno $\mathcal{U}(x_0)=(x_0-\delta,x_0+\delta)$ di $x_0$ (incluso $x_0$) e se esiste **finito**
> $$\lim_{h\to0}\frac{f'(x_0+h)-f'(x_0)}{h}\in\mathbb{R}$$
> chiameremo tale limite **derivata seconda** di $f$ in $x_0$ e
> $$f''(x_0)=\lim_{h\to0}\frac{f'(x_0+h)-f'(x_0)}{h}\in\mathbb{R}$$

Notazioni: $f''(x_0)$, $\dfrac{d^2f}{dx^2}(x_0)$, $D^2f(x_0)$, $\ddot f(x_0)$.

Osservazione: $f''(x_0)=(f')'(x_0)$.

> [!abstract] Definizione — derivata $n$-esima
> Se $f:(a,b)\subseteq\mathbb{R}\to\mathbb{R}$, $x_0\in(a,b)$, se $f$ è derivabile $n-1$ volte in un intorno $\mathcal{U}(x_0)=(x_0-\delta,x_0+\delta)$ di $x_0$ (compreso $x_0$) con $n\ge2$, se esiste **finito**
> $$\lim_{h\to0}\frac{f^{(n-1)}(x_0+h)-f^{(n-1)}(x_0)}{h}\in\mathbb{R}$$
> diremo che $f$ è **derivabile $n$ volte in $x_0$** e chiameremo tale limite **derivata $n$-esima** di $f$ in $x_0$:
> $$f^{(n)}(x_0)=\lim_{h\to0}\frac{f^{(n-1)}(x_0+h)-f^{(n-1)}(x_0)}{h}\in\mathbb{R}$$

Osservazione: $f^{(n)}(x_0)=\big(f^{(n-1)}\big)'(x_0)$.

## Note collegate
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[128_Derivate_delle_Funzioni_Elementari]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/derivate-di-ordine-superiore
