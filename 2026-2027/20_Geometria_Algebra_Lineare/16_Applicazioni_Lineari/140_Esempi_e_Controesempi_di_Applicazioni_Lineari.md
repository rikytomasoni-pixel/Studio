---
tags: [GAL, applicazioni-lineari, controesempi, lezione-17]
data: 2026-11-05
lezione: 17
fonte: "GAL 2026-2027 - 20261105 - LEZIONE 17.pdf (slide 149-150)"
---

# Esempi e controesempi di applicazioni lineari

## Controesempio 1: $f(x,y)=x+y+1$
$$f:\mathbb{R}^2\to\mathbb{R},\qquad f\left(\begin{bmatrix}x\\y\end{bmatrix}\right)=x+y+1$$
**D.** $f$ è un'applicazione lineare?

**R.** $f\left(\begin{bmatrix}0\\0\end{bmatrix}\right)=0+0+1=1\neq0\ \Rightarrow$ $f$ **NON** è un'applicazione lineare ([[139_Proprieta_delle_Applicazioni_Lineari]]: $L(\underline{0})\neq\underline{0}$).

## Controesempio 2: $f(x,y)=x^2+y^2$
$$f:\mathbb{R}^2\to\mathbb{R},\qquad f\left(\begin{bmatrix}x\\y\end{bmatrix}\right)=x^2+y^2$$
**D.** $f$ è un'applicazione lineare?

**R.** $f\left(\begin{bmatrix}0\\0\end{bmatrix}\right)=0^2+0^2=0$ ✓.

Verifico (?) l'omogeneità: $\forall\lambda\in\mathbb{R}$, $\forall\begin{bmatrix}x\\y\end{bmatrix}\in\mathbb{R}^2$
$$f\left(\lambda\begin{bmatrix}x\\y\end{bmatrix}\right)=f\left(\begin{bmatrix}\lambda x\\\lambda y\end{bmatrix}\right)=(\lambda x)^2+(\lambda y)^2=\lambda^2x^2+\lambda^2y^2=\lambda^2(x^2+y^2)$$
$$f\left(\lambda\begin{bmatrix}x\\y\end{bmatrix}\right)=\lambda^2f\left(\begin{bmatrix}x\\y\end{bmatrix}\right)\neq\lambda f\left(\begin{bmatrix}x\\y\end{bmatrix}\right)$$
$\Rightarrow$ $f$ **NON** è un'applicazione lineare.

> [!note] Osservazione
> Sulla slide la conclusione è scritta con "$L$ NON è un'applicazione lineare" (la funzione si chiama $f$). Qui $f(\underline{0})=0$ è soddisfatta ma la funzione non è comunque lineare: la condizione $L(\underline{0})=\underline{0}$ non basta.

## Esempi positivi
- $L_A(\underline{v})=A\underline{v}$ ([[137_Esempi_di_Applicazioni_Lineari_Matrici_Trasposizione_Traccia]])
- la trasposizione e la traccia (stessa nota)
- la derivata $D:\mathcal{C}^1(I)\to\mathcal{C}^0(I)$ ([[138_Derivata_come_Applicazione_Lineare]])

## Note collegate
- [[136_Applicazioni_Lineari_Definizione_17_1]]
- [[139_Proprieta_delle_Applicazioni_Lineari]]
- Indice: [[18_Indice_Lezione_17]] · [[00_MOC_GAL]]

#GAL/applicazioni-lineari/controesempi
