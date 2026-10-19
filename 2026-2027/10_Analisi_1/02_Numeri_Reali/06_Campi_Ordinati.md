---
tags:
  - AM1
  - numeri-reali
  - assiomi-di-R
  - campo
  - campo-ordinato
data: 2026-09-16
fonte: Lezione 2
---

# $\mathbb{R}$ e $\mathbb{Q}$ come campi ordinati

Su $\mathbb{R}$ e $\mathbb{Q}$ sono definite due operazioni, $+$ e $\cdot$ (e le loro operazioni inverse), con le seguenti proprietà.

## Assiomi della somma

> [!info] Assiomi $(S_1)$–$(S_4)$
> $(S_1)$ **Commutatività**
> $$a+b = b+a \qquad \forall\, a,b$$
> $(S_2)$ **Associatività**
> $$(a+b)+c = a+(b+c) \qquad \forall\, a,b,c$$
> $(S_3)$ **Esistenza dell'elemento neutro**: $\exists\, 0$ tale che
> $$a+0 = 0+a = a \qquad \forall\, a$$
> $(S_4)$ **Esistenza dell'elemento opposto**: $\forall\, a$ esiste un elemento, che indichiamo con $(-a)$, tale che
> $$a+(-a) = (-a)+a = 0$$

Si scrive $a-b$ invece di $a+(-b)$, $\forall\, a,b$.

## Assiomi del prodotto

> [!info] Assiomi $(P_1)$–$(P_4)$
> $(P_1)$ **Commutatività**
> $$a\cdot b = b\cdot a \qquad \forall\, a,b$$
> $(P_2)$ **Associatività**
> $$(a\cdot b)\cdot c = a\cdot (b\cdot c) \qquad \forall\, a,b,c$$
> $(P_3)$ **Esistenza dell'elemento neutro**: $\exists\, 1$ tale che
> $$a\cdot 1 = 1 \cdot a = a \qquad \forall\, a$$
> $(P_4)$ **Esistenza dell'elemento inverso**: per ogni $a\neq 0$ esiste un elemento,
> che indichiamo con $a^{-1}=\dfrac{1}{a}$, tale che
> $$a\cdot a^{-1} = a^{-1}\cdot a = 1$$

## Distributività e definizione di campo

> [!info] Assioma $(SP)$ — Distributività
> $$a(b+c) = ab + ac \qquad \forall\, a,b,c$$

> [!warning] Definizione — Campo
> Un insieme $X$ dotato di operazioni $+,\cdot$ (somma e prodotto) che soddisfano le proprietà $(S_1)$–$(S_4)$, $(P_1)$–$(P_4)$, $(SP)$ si chiama **campo**.

**Esempi:** $\mathbb{R}, \mathbb{Q}, \mathbb{C}$ sono campi. $\mathbb{N}, \mathbb{Z}$ **non** lo sono.

## Assiomi dell'ordine

Su $\mathbb{R}, \mathbb{Q}$ è definita anche una relazione d'ordine totale $\leq$, con le seguenti proprietà.

> [!info] Assiomi $(O_1)$–$(O_4)$
> $(O_1)$ **Riflessività**
> $$a\leq a \qquad \forall\, a$$
> $(O_2)$ **Antisimmetria**
> $$\forall\, a,b: \quad a\leq b,\ b\leq a \ \Rightarrow\ a=b$$
> $(O_3)$ **Transitività**
> $$\forall\, a,b,c: \quad a\leq b,\ b\leq c \ \Rightarrow\ a\leq c$$
> $(O_4)$ **Totalità della relazione d'ordine**
> $$\forall\, a,b \quad \text{vale} \quad a\leq b \ \text{ oppure } \ b\leq a$$

## Compatibilità tra ordine e operazioni

> [!info] Assiomi $(SO)$ e $(PO)$
> $(SO)$ $\ \forall\, a,b,c$, se $a\leq b$ allora
> $$a+c \leq b+c$$
> $(PO)$ $\ \forall\, a,b,\ \forall\, c>0$, se $a\leq b$ allora
> $$ac \leq bc$$

## Definizione di campo ordinato

> [!warning] Definizione — Campo ordinato
> Se $X$ è un insieme dotato di operazioni $+,\cdot$ (somma e prodotto) e di una relazione d'ordine totale $\leq$ che soddisfano $(S_1)$–$(S_4)$, $(P_1)$–$(P_4)$, $(O_1)$–$(O_4)$, $(SP)$, $(SO)$, $(PO)$, allora $X$ si dice **campo ordinato**.

**Esempi:** $\mathbb{R}, \mathbb{Q}$ sono campi ordinati. $\mathbb{C}$ è un campo, ma **non** può essere reso campo ordinato (vedi sotto).

## Alcune regole dedotte dagli assiomi

**Osservazione.** Le familiari regole di calcolo che utilizziamo abitualmente in $\mathbb{R}$ e $\mathbb{Q}$ possono essere dedotte da questi assiomi. Ad esempio:

$$a\cdot 0 = 0 \qquad \forall\, a$$
$$(-a) = (-1)\cdot a \qquad \forall\, a$$
$$1 > 0$$
$$a^2 \geq 0 \qquad \forall\, a$$
$$\boxed{a^2+1 \geq 1 > 0} \qquad \forall\, a$$

**Osservazione.** In particolare, $a^2+1\neq 0\ \ \forall\, a$ in un campo ordinato.

## Perché $\mathbb{C}$ non può essere ordinato

In $\mathbb{C}$ l'equazione
$$z^2+1=0$$
ha le due soluzioni $z=\pm i$. Ma in un campo ordinato dovrebbe valere $a^2+1\neq 0\ \forall a$ (vedi sopra). Quindi $\mathbb{C}$ non può essere reso campo ordinato.

### Note collegate
- [[00_MOC_Analisi_1]]
- [[01_Insiemi_Numerici]]
- [[07_Insiemi_Limitati_Max_Min]] — prosecuzione: insiemi in $X=\mathbb{R}$ o $\mathbb{Q}$
- [[08_Estremo_Superiore_Inferiore]] — assioma di continuità: $\mathbb{R}$ unico campo ordinato con la proprietà dell'estremo superiore
- [[13_Numeri_Complessi]] — $\mathbb{C}$ come campo non ordinato

#AM1/numeri-reali/campi-ordinati
