---
tags:
  - AM1
  - derivate
  - de-l-hopital
  - controesempio
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 16)"
---

# Controesempio a de l'Hôpital: il limite delle derivate non esiste

Se $\nexists\displaystyle\lim\frac{f'}{g'}$ non si può concludere nulla su $\displaystyle\lim\frac fg$ ([[152_Teorema_di_de_l_Hopital]]).

**Esempio.**
$$\lim_{x\to+\infty}\frac{\overbrace{2x+\sin x}^{f}}{\underbrace{2x-\sin x}_{g}}\qquad\left[\tfrac\infty\infty\right]$$
Poiché $2x\pm\sin x\sim2x$ per $x\to+\infty$ ([[106_Asintotico_e_o_piccolo_per_Funzioni]]),
$$\lim_{x\to+\infty}\frac{2x+\sin x}{2x-\sin x}=\lim_{x\to+\infty}\frac{2x}{2x}=1$$
Tuttavia
$$\lim_{x\to+\infty}\frac{f'(x)}{g'(x)}=\lim_{x\to+\infty}\frac{2+\cos x}{2-\cos x}\ \ \nexists$$
Quindi il limite $\frac fg$ esiste (vale $1$) pur non esistendo il limite $\frac{f'}{g'}$: l'ipotesi 2 di de l'Hôpital non può essere tolta né "rovesciata".

## Note collegate
- [[152_Teorema_di_de_l_Hopital]]
- [[106_Asintotico_e_o_piccolo_per_Funzioni]]
- [[107_Proprieta_degli_Asintotici_per_Funzioni]]
- [[154_Esempi_di_Applicazione_de_l_Hopital]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/de-l-hopital-controesempio
