---
tags:
  - AM1
  - successioni
  - monotonia
  - teorema
data: 2026-09-30 e 2026-10-02
fonte: Lezione 6 e Lezione 7
---

# Successioni monotone

> [!warning] Definizione — Successione monotona
> Una successione $a_n$ si dice **monotona**:
> - **crescente** se $a_n \leq a_m \ \ \forall\, n<m$ ($n,m\in\mathbb{N}$)
> - **decrescente** se $a_n \geq a_m \ \ \forall\, n<m$
> - **strettamente crescente** se $a_n < a_m \ \ \forall\, n<m$
> - **strettamente decrescente** se $a_n > a_m \ \ \forall\, n<m$

**Esempi.** $a_n=n$ cresce; $a_n=\dfrac{1}{n}$ decresce.

## Teorema sul limite di successioni monotone e limitate

> [!abstract] Teorema
> Sia $a_n$ una successione monotona e limitata. Allora $\exists\, \lim_{n\to\infty} a_n = l\in\mathbb{R}$.
>
> Inoltre:
> - se $a_n$ è **crescente**: $\lim_{n\to\infty} a_n = l^-$, con $l=\sup_{n\in\mathbb{N}} a_n \in\mathbb{R}$
> - se $a_n$ è **decrescente**: $\lim_{n\to\infty} a_n = l^+$, con $l=\inf_{n\in\mathbb{N}} a_n \in\mathbb{R}$

**Osservazione.** Se $a_n$ crescente, basta chiedere $a_n$ limitata dall'alto. Se $a_n$ decrescente, basta chiedere $a_n$ limitata dal basso (dall'altro lato lo sono automaticamente).

**Dimostrazione.** Solo il caso $a_n$ limitata crescente (il caso decrescente è analogo).

Perché $a_n$ crescente, $a_n$ è automaticamente limitata dal basso: $a_0\leq a_n \ \ \forall\, n\in\mathbb{N}$.

Sia $l=\displaystyle\sup_{n\in\mathbb{N}} a_n \in \mathbb{R}\cup\{+\infty\}$. Esso esiste grazie all'assioma dell'estremo superiore, che $\mathbb{R}$ soddisfa.

Perché per ipotesi $a_n$ è limitata dall'alto, deve essere $l=\sup a_n\in\mathbb{R}$ ($l$ è un maggiorante di $\{a_n\}$).

Per definizione di estremo superiore:

① $l$ è maggiorante di $\{a_n\}$: $a_n\leq l \ \ \forall\, n\in\mathbb{N}$

② $\forall\, \varepsilon>0\ \exists\, N_0\in\mathbb{N}$ tale che $l-\varepsilon<a_{N_0}\leq l$ ($l-\varepsilon$ non è maggiorante)

Perché $a_n$ crescente, $\forall\, n\geq N_0$ $a_n\geq a_{N_0}$ ③

Segue, da ②③, che
$$\forall\, \varepsilon>0\ \exists\, N_0\in\mathbb{N} \text{ tale che } l-\varepsilon<a_{N_0}\leq a_n \leq l \qquad \forall\, n\geq N_0$$

$$\Rightarrow \quad \forall\, \varepsilon>0\ \exists\, N_0\in\mathbb{N} : \forall\, n\geq N_0 \quad l-\varepsilon<a_n\leq l$$

$$\Rightarrow \quad \text{per definizione} \quad \lim_{n\to\infty} a_n = l^-, \quad l=\sup_{n\in\mathbb{N}} a_n \qquad \blacksquare$$

![[LimiteDifettoComeSup.png]]

**Osservazione.** Questo teorema si poggia sull'assioma dell'estremo superiore, che $\mathbb{R}$ soddisfa (e $\mathbb{Q}$ no).

## Versione generale: successioni monotone non necessariamente limitate

> [!abstract] Teorema
> Sia $a_n$ una successione monotona. Allora $a_n$ ammette limite, cioè $\exists\, \lim_{n\to\infty} a_n = l\in\overline{\mathbb{R}}$.
>
> - se $a_n$ cresce, allora $\lim_{n\to\infty} a_n = l^-$, con $l=\sup_{n\in\mathbb{N}} a_n \in\overline{\mathbb{R}}$
> - se $a_n$ decresce, allora $\lim_{n\to\infty} a_n = l^+$, con $l=\inf_{n\in\mathbb{N}} a_n \in\overline{\mathbb{R}}$

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ regolare.

**Dimostrazione.**

**1) Caso $a_n$ limitata.** In questo caso il teorema precedente permette di concludere direttamente: $\exists\, l\in\mathbb{R}$ tale che $\lim a_n=l$, con le stesse conclusioni viste sopra.

**2) Caso $a_n$ illimitata.** Per fissare le idee, supponiamo $a_n$ crescente (se $a_n$ è decrescente la dimostrazione è analoga).

Perché $a_n$ crescente, $a_0\leq a_n\ \ \forall\, n\in\mathbb{N}$ ($a_n$ è limitata dal basso). Quindi $a_n$ deve essere illimitata dall'alto. In particolare
$$\sup_{n\in\mathbb{N}} a_n = +\infty$$
per definizione.

Quindi $\forall\, M>0\ \exists\, n_0\in\mathbb{N}$ tale che $a_{n_0}>M$. Perché $a_n$ crescente, $\forall\, n\geq n_0$ segue che $a_n\geq a_{n_0}$.

Quindi
$$\forall\, M>0\ \exists\, n_0\in\mathbb{N} \text{ tale che } \forall\, n\geq n_0 \quad a_n\geq a_{n_0}>M$$
$$\Rightarrow \quad \forall\, M>0\ \exists\, n_0\in\mathbb{N} : \forall\, n\geq n_0 \quad a_n>M$$

che è la definizione di $\lim_{n\to\infty} a_n = +\infty$, con $\sup a_n = +\infty$. $\blacksquare$

**Osservazione.** $a_n$ monotona $\Rightarrow$ $a_n$ regolare, ma non vale il viceversa: $a_n$ regolare $\not\Rightarrow$ $a_n$ monotona.

Ad esempio $a_n = \dfrac{(-1)^n}{n}$ è un controesempio: infatti $a_n$ non è monotona e $\lim_{n\to\infty} a_n = 0$.

### Note collegate
- [[00_MOC_Analisi_1]]
- [[23_Monotonia]] — monotonia per funzioni reali
- [[08_Estremo_Superiore_Inferiore]] — assioma di continuità, $\sup$ e $\inf$
- [[30_Limiti_di_Successioni]] — definizioni di convergenza e divergenza
- [[32_Successione_Convergente_e_Limitata]]
- [[27_Teorema_Monotone_Invertibili]] — teorema analogo per funzioni monotone e invertibilità

#AM1/successioni-e-limiti/successioni-monotone
