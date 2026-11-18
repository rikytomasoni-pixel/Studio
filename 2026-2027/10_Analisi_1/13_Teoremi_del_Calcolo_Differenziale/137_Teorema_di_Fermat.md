---
tags:
  - AM1
  - derivate
  - estremi
  - teorema
  - dimostrazione
data: 2026-11-13
lezione: 18
fonte: "AM1 L18 26-27.pdf (pag. 8-10)"
---

# Teorema di Fermat

> [!abstract] Teorema (di Fermat)
> Sia $f:(a,b)\to\mathbb{R}$ e $x_0\in(a,b)$. Allora, se $x_0$ è un punto di estremo per $f$ e se $f$ è derivabile in $x_0$,
> $$f'(x_0)=0$$

**Dimostrazione.** Proviamo il teorema solo nel caso in cui $x_0\in(a,b)$ sia un punto di **massimo** per $f$; la dimostrazione nel caso di punto di minimo è simile.

Essendo $x_0$ punto di massimo, se $|h|$ è sufficientemente piccolo si ha $f(x_0+h)\le f(x_0)$. Quindi:
- se $h>0$: $\displaystyle\frac{f(x_0+h)-f(x_0)}{h}\le0$ (numeratore $\le0$, denominatore $>0$);
- se $h<0$: $\displaystyle\frac{f(x_0+h)-f(x_0)}{h}\ge0$ (numeratore $\le0$, denominatore $<0$).

Essendo $f$ derivabile in $x_0$, esistono finiti
$$\lim_{h\to0^+}\frac{f(x_0+h)-f(x_0)}{h}=f'_+(x_0)=f'(x_0)\in\mathbb{R}\qquad\lim_{h\to0^-}\frac{f(x_0+h)-f(x_0)}{h}=f'_-(x_0)=f'(x_0)\in\mathbb{R}$$
Poiché tali limiti esistono, per il [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni|teorema di permanenza del segno]]
$$f'_+(x_0)=\lim_{h\to0^+}\frac{f(x_0+h)-f(x_0)}{h}\le0\qquad f'_-(x_0)=\lim_{h\to0^-}\frac{f(x_0+h)-f(x_0)}{h}\ge0$$
Dunque $f'_+(x_0)\le0$, $f'_-(x_0)\ge0$ e $f'_+(x_0)=f'(x_0)=f'_-(x_0)$, da cui
$$f'(x_0)=0\qquad\square$$

## Note collegate
- [[136_Massimi_e_Minimi_Locali_e_Globali]]
- [[138_Punti_Stazionari_e_Punti_Critici]]
- [[139_Ricerca_di_Massimi_e_Minimi_Assoluti_su_Intervallo_Chiuso]]
- [[141_Teorema_di_Rolle]]
- [[122_Rapporto_Incrementale_e_Derivata_in_un_Punto]]
- [[101_Teorema_di_Permanenza_del_Segno_per_Funzioni]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/fermat
