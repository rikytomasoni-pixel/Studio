---
tags:
  - AM1
  - successioni
  - permanenza-del-segno
  - teorema
  - limiti
data: 2026-10-02
fonte: Lezione 7
---

# Teorema di permanenza del segno (per successioni)

> [!abstract] Teorema — Permanenza del segno
> **1)** Data $a_n$ successione, se esiste $\lim_{n\to\infty} a_n = l\in\overline{\mathbb{R}}$ e $l>0$ (nel senso $l\in(0,+\infty]$), allora
> $$a_n>0 \quad \text{definitivamente in } n\in\mathbb{N}$$
> Similmente, se esiste $\lim_{n\to\infty} a_n = l$ e $l<0$ (cioè $l\in[-\infty,0)$) allora $a_n<0$ definitivamente in $n\in\mathbb{N}$.
>
> **2)** Data una successione $a_n$, se esiste $l=\lim_{n\to\infty} a_n \in\overline{\mathbb{R}}$ e se $a_n\geq 0$ definitivamente in $n\in\mathbb{N}$, allora $l\geq 0$ (cioè $l\in[0,+\infty]$).
> Similmente, se esiste $\lim_{n\to\infty} a_n \in\overline{\mathbb{R}}$ e se $a_n\leq 0$ definitivamente in $n\in\mathbb{N}$, allora $l\leq 0$ (cioè $l\in[-\infty,0]$).

**Osservazioni.**
- Può essere $l=\lim_{n\to\infty} a_n = 0$ e $a_n<0$ definitivamente. Ad esempio $a_n=-\dfrac{1}{n}$ soddisfa $a_n<0\ \ \forall\, n\in\mathbb{N}, n\geq 1$, e $\lim_{n\to\infty} a_n=0$.
- Se $a_n>0$ ed esiste $\lim_{n\to\infty} a_n=l$, allora $l\geq 0$, ma può essere $l=0$. Ad esempio $a_n=\dfrac{1}{n}$ soddisfa $a_n>0\ \ \forall\, n\in\mathbb{N}, n\geq 1$, e $\lim_{n\to\infty} a_n=0$.

**Dimostrazione.**

**1)** Sia $l=\lim_{n\to\infty} a_n \in (0,+\infty]$.

Se $l=+\infty$: per definizione $\forall\, M>0\ \exists\, N\in\mathbb{N}$ tale che $\forall\, n\geq N$ $a_n>M>0 \Rightarrow a_n>0$ definitivamente in $n\in\mathbb{N}$.

Se $l\in(0,+\infty)$: per definizione $\forall\, \varepsilon>0\ \exists\, N\in\mathbb{N}$ tale che $\forall\, n\geq N$ $l-\varepsilon<a_n<l+\varepsilon$.

![[PermanenzaSegno.png]]

Scegliendo $\varepsilon=\dfrac{l}{2}$ nella definizione di limite, otteniamo $\exists\, N\in\mathbb{N}$ tale che $\forall\, n\geq N$
$$l-\dfrac{l}{2}<a_n \quad\Rightarrow\quad a_n>\dfrac{l}{2}>0 \quad\Rightarrow\quad a_n>0 \text{ definitivamente in } n\in\mathbb{N}$$

Similmente se $l<0$.

**2)** Sia $a_n\geq 0$ definitivamente in $n\in\mathbb{N}$ e $\exists\, l=\lim_{n\to\infty} a_n\in\overline{\mathbb{R}}$. Vogliamo provare $l\geq 0$.

Per assurdo sia $l<0$. Per la parte (1) appena dimostrata deve essere $a_n<0$ definitivamente in $n\in\mathbb{N}$. Assurdo, perché dovrebbe essere $a_n\geq 0$ e $a_n<0$ definitivamente in $n\in\mathbb{N}$.

Quindi $l\geq 0$. Similmente se $a_n\leq 0$ e $\exists\, l=\lim_{n\to\infty} a_n$. $\blacksquare$

### Note collegate
- [[00_MOC_Analisi_1]]
- [[30_Limiti_di_Successioni]] — definizione di limite
- [[34_Algebra_dei_Limiti]] — corollario che combina permanenza del segno e algebra dei limiti
- [[35_Teoremi_del_Confronto]]
- [[37_Algebra_Limiti_Infiniti]] — estensione dell'algebra dei limiti a $\pm\infty$ e forme indeterminate

#AM1/successioni-e-limiti/teorema-permanenza-del-segno
