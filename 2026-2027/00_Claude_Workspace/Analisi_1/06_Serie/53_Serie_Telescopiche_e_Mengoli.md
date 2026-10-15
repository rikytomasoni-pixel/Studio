---
tags:
  - AM1
  - serie
  - serie-telescopiche
  - serie-di-mengoli
data: 2026-10-14
fonte: "AM1 L10 26-27.pdf (pag. 16-18)"
stato: da_verificare
immagini_mancanti: false
destinazione: "10_Analisi_1/06_Serie"
---

# Serie telescopiche e serie di Mengoli

## Serie telescopiche
$$\sum_{n=0}^\infty a_n\qquad\text{con}\qquad a_n=b_n-b_{n+1}$$
dove $b_n$ è una qualche successione.

$$S_N=\sum_{n=0}^Na_n=\sum_{n=0}^N(b_n-b_{n+1})=(b_0-\cancel{b_1})+(\cancel{b_1}-\cancel{b_2})+(\cancel{b_2}-\cancel{b_3})+\dots+(\cancel{b_{N-1}}-\cancel{b_N})+(\cancel{b_N}-b_{N+1})=b_0-b_{N+1}$$

> [!abstract] Conseguenza
> $\exists\,S=\lim_{N\to\infty}S_N=\sum_{n=0}^\infty a_n\in\overline{\mathbb{R}}$ **se e solo se** $\exists\,b^*=\lim_{N\to\infty}b_N\in\overline{\mathbb{R}}$.
> Inoltre, in tal caso,
> $$S=\sum_{n=0}^\infty a_n=b_0-b^*\in\overline{\mathbb{R}}$$

## Esempio: serie di Mengoli
$$\sum_{n=1}^\infty\frac1{n(n+1)}=1$$
$a_n=\dfrac1{n(n+1)}=\dfrac1n-\dfrac1{n+1}$, con $b_n=\dfrac1n$: serie telescopica.
$$S_N=\sum_{n=1}^Na_n=\sum_{n=1}^N\left(\frac1n-\frac1{n+1}\right)=1-\frac1{N+1}$$
$$\Rightarrow\sum_{n=1}^\infty\frac1{n(n+1)}=\lim_{N\to\infty}S_N=\lim_{N\to\infty}\left(1-\frac1{N+1}\right)=1$$

(Un'altra applicazione della stessa idea telescopica: [[55_Serie_Armonica]].)

## Note collegate
- [[52_Linearita_delle_Serie]]
- [[54_Condizione_Necessaria_di_Convergenza]]
- [[55_Serie_Armonica]]
- [[47_Serie_Introduzione_e_Somme_Parziali]]
- [[00_MOC_Analisi_1]]

#AM1/serie/serie-telescopiche-mengoli
