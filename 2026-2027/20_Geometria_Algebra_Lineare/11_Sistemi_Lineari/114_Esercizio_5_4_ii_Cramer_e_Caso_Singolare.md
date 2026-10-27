---
tags: [GAL, sistemi-lineari, esercizio, parametri, cramer, determinante]
data: 2026-10-27
lezione: esercizi
fonte: "Esercizio 5.4 (ii); svolgimento redatto da Claude, non presente negli appunti"
---

# Esercizio 5.4 (ii): Cramer e caso singolare

> [!question] Sistema
> $$\begin{cases}(a+5)x+y=1\\ 2x+2ay+az=a^2\\ -x+2y+z=a\end{cases}\qquad A=\begin{pmatrix}a+5&1&0\\ 2&2a&a\\ -1&2&1\end{pmatrix}$$

## 1. Determinante
Sviluppo lungo la prima riga:
$$\det A=(a+5)(2a-2a)-1\cdot(2+a)=-(a+2)$$

## 2. Caso $a\neq-2$
$\det A\neq0\Rightarrow r(A)=3$ ([[88_Teorema_sull_Invertibilita_della_Matrice]]) $\Rightarrow$ per il [[86_Teorema_di_Cramer]] esiste **un'unica** soluzione per ogni termine noto.

## 3. Caso $a=-2$
$$\begin{cases}3x+y=1\\ 2x-4y-2z=4\\ -x+2y+z=-2\end{cases}$$
La seconda equazione è $-2$ volte la terza: $-2(-x+2y+z)=2x-4y-2z$ e $-2\cdot(-2)=4$. I termini noti sono coerenti, quindi l'equazione è ridondante. Restano $3x+y=1$ e $-x+2y+z=-2$ (indipendenti): $r(A)=r(A|\underline{b})=2$, con $3-2=1$ parametro libero ([[82_Teorema_di_Rouche_Capelli]]): $\infty^1$ soluzioni.

> [!success] Risultato
> Soluzioni per **ogni** $a\in\mathbb{R}$: unica se $a\neq-2$, $\infty^1$ se $a=-2$.

> [!note] Osservazione (non presente negli appunti)
> $\det A=0$ non implica sistema impossibile: se la riga dipendente ha anche il termine noto coerente, il sistema resta compatibile.

## Note collegate
- [[112_Esercizio_5_4_Sistemi_con_Parametro]]
- [[116_Strategia_Determinante_per_Sistemi_con_Parametro]]
- [[86_Teorema_di_Cramer]]
- [[83_Esempio_Sistema_con_Parametro_k_e_Rouche_Capelli]]

#GAL/sistemi-lineari/esercizio-5-4
