---
tags:
  - AM1
  - taylor
  - limiti
  - esempio
  - o-piccolo
data: 2026-11-25
lezione: 21
fonte: "AM1 L21 26-27.pdf (pag. 13-15)"
---

# Esempio: calcolo di un limite con gli sviluppi di Taylor

$$\lim_{x\to0^+}\frac{\big[\log\big(e(1+2x)\big)\big]^2-e^{4x}+8x^2}{x^2\big(\sqrt{1+\pi x}-\cos x\big)}\ \ \Big[\tfrac00\Big]$$

Si sviluppano numeratore $N(x)$ e denominatore $D(x)$ fino al **primo termine non nullo**, usando [[172_Sviluppi_di_Maclaurin_di_e_alla_x_sin_cos|gli sviluppi notevoli]] per $x\to0^+$.

## Denominatore

- $(1+t)^\alpha=1+\alpha t+o(t)$ per $t\to0$, con $t=\pi x$ e $\alpha=\tfrac12$: $\sqrt{1+\pi x}=1+\dfrac\pi2x+o(x)$
- $\cos x=1-\dfrac{x^2}{2}+o(x^2)$

$$D=x^2\Big(1+\frac\pi2x+o(x)-1+\frac{x^2}{2}+o(x^2)\Big)=x^2\Big(\frac\pi2x+\frac{x^2}{2}+o(x)+o(x^2)\Big)=x^2\Big(\frac\pi2x+o(x)\Big)=\frac\pi2x^3+o(x^3)\sim\frac\pi2x^3$$

## Numeratore

- $e^t=1+t+\dfrac{t^2}{2}+\dfrac{t^3}{6}+o(t^3)$, con $t=4x\to0$:
  $$e^{4x}=1+4x+\frac{16x^2}{2}+\frac{64x^3}{6}+o(x^3)=1+4x+8x^2+\frac{32}{3}x^3+o(x^3)$$
- $\log(1+t)=t-\dfrac{t^2}{2}+\dfrac{t^3}{3}+o(t^3)$, con $t=2x\to0$:
  $$\big[\log(e(1+2x))\big]^2=\big[\log e+\log(1+2x)\big]^2=\Big[1+2x-\frac{4x^2}{2}+\frac{8x^3}{3}+o(x^3)\Big]^2=1+4x-\frac83x^3+o(x^3)$$
  (nel quadrato i termini in $x^2$ si cancellano: $+4x^2-4x^2$)

$$N=1+4x-\frac83x^3-1-4x-8x^2-\frac{32}{3}x^3+8x^2+o(x^3)=-\frac{40}{3}x^3+o(x^3)\sim-\frac{40}{3}x^3$$

## Risultato

$$\frac{N(x)}{D(x)}=\frac{-\frac{40}{3}x^3+o(x^3)}{\frac\pi2x^3+o(x^3)}\sim\frac{-\frac{40}{3}x^3}{\frac\pi2x^3}\ \longrightarrow\ -\frac{80}{3\pi}$$

> [!tip] Metodo
> Si sviluppa **tutto allo stesso ordine** (qui $x^3$) finché i termini di grado più basso non si cancellano; poi si usa $f\sim g$ ([[107_Proprieta_degli_Asintotici_per_Funzioni]]).

## Note collegate
- [[172_Sviluppi_di_Maclaurin_di_e_alla_x_sin_cos]]
- [[178_Algebra_degli_o_piccoli]]
- [[154_Esempi_di_Applicazione_de_l_Hopital]] (altri esempi di limiti)
- [[108_Limiti_Notevoli_di_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/taylor/limiti
