---
tags:
  - AM1
  - derivate
  - monotonia
  - controesempio
data: 2026-11-18
lezione: 19
fonte: "AM1 L19 26-27.pdf (pag. 2-4)"
---

# Test di monotonia: controesempi e osservazioni

Teorema: [[140_Test_di_Monotonia]]. Dimostrazione: [[144_Dimostrazione_del_Test_di_Monotonia]].

## Nei punti (3) e (4) non vale "se e solo se"

> [!note] Osservazione
> Esistono funzioni strettamente crescenti (decrescenti) e derivabili in $(a,b)$, intervallo in $\mathbb{R}$, tali che $f'(x)\ge0$ in $(a,b)$ ($f'(x)\le0$ in $(a,b)$), ma tali che $f'(x)=0$ per qualche $x\in(a,b)$.
>
> Nei punti (3) e (4) del test di monotonia non vale "se e solo se".

**Esempio.** $f(x)=x^3$ per ogni $x\in\mathbb{R}$, $f:\mathbb{R}\to\mathbb{R}$:
$$f'(x)=3x^2\ \ \forall x\in\mathbb{R},\qquad f'(x)\ge0\ \ \forall x\in\mathbb{R},\quad f'(0)=0$$
$f$ è strettamente crescente in $\mathbb{R}$ pur avendo $f'(0)=0$ (vedi anche [[138_Punti_Stazionari_e_Punti_Critici]]).

![[GraficoxCubo.png|303]]

## L'ipotesi "intervallo" non si può togliere

**Esempio.** L'ipotesi che $f$ sia definita su un **intervallo** non può essere omessa.
$$f(x)=\frac1x\qquad f:\underbrace{(-\infty,0)\cup(0,\infty)}_{\mathcal{D}(f)}\to\mathbb{R}$$
$$f'(x)=-\frac1{x^2}<0\qquad\forall x\in\mathcal{D}(f)$$

![[grafico 1suX.png]]

$f$ è strettamente decrescente in $(-\infty,0)$ e in $(0,\infty)$ (la sua restrizione agli intervalli $(-\infty,0)$ e $(0,\infty)$ è decrescente), ma **non è decrescente** in $\mathcal{D}(f)=(-\infty,0)\cup(0,\infty)$.

> [!note] Osservazione (non presente negli appunti)
> Infatti $-1<1$ ma $f(-1)=-1<1=f(1)$: nella definizione di funzione decrescente si richiede $x_1<x_2\Rightarrow f(x_1)\ge f(x_2)$ per **ogni** coppia di punti del dominio, anche presi da due intervalli diversi. Stesso fenomeno dell'esempio in [[143_Caratterizzazione_delle_Funzioni_Costanti_su_un_Intervallo]].

## Note collegate
- [[140_Test_di_Monotonia]]
- [[144_Dimostrazione_del_Test_di_Monotonia]]
- [[146_Test_di_Monotonia_e_Estremi_Locali]]
- [[143_Caratterizzazione_delle_Funzioni_Costanti_su_un_Intervallo]]
- [[23_Monotonia]]
- [[00_MOC_Analisi_1]]

#AM1/derivate/test-monotonia-controesempi
